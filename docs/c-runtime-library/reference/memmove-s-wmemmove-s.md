---
title: memmove_s, wmemmove_s
ms.date: 11/04/2016
apiname:
- wmemmove_s
- memmove_s
apilocation:
- msvcrt.dll
- msvcr80.dll
- msvcr90.dll
- msvcr100.dll
- msvcr100_clr0400.dll
- msvcr110.dll
- msvcr110_clr0400.dll
- msvcr120.dll
- msvcr120_clr0400.dll
- ucrtbase.dll
- api-ms-win-crt-string-l1-1-0.dll
apitype: DLLExport
f1_keywords:
- wmemmove_s
- memmove_s
helpviewer_keywords:
- wmemmove_s function
- memmove_s function
ms.assetid: a17619e4-1307-4bb0-98c6-77f8c68dab2d
ms.openlocfilehash: 7b60174c3a06e60301a3e9123434220227f4f426
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50561189"
---
# <a name="memmoves-wmemmoves"></a>memmove_s, wmemmove_s

한 버퍼를 다른 버퍼로 이동합니다. 이러한 함수는 [CRT의 보안 기능](../../c-runtime-library/security-features-in-the-crt.md)에 설명된 대로 강화된 보안 기능이 있는 [memmove, wmemmove](memmove-wmemmove.md)의 버전입니다.

## <a name="syntax"></a>구문

```C
errno_t memmove_s(
   void *dest,
   size_t numberOfElements,
   const void *src,
   size_t count
);
errno_t wmemmove_s(
   wchar_t *dest,
   size_t numberOfElements,
   const wchar_t *src,
   size_t count
);
```

### <a name="parameters"></a>매개 변수

*dest*<br/>
대상 개체입니다.

*numberOfElements*<br/>
대상 버퍼의 크기입니다.

*src*<br/>
소스 개체입니다.

*count*<br/>
바이트 수 (**memmove_s**) 또는 문자 (**wmemmove_s**) 복사 합니다.

## <a name="return-value"></a>반환 값

성공 시 0이고, 실패 시 오류 코드입니다.

### <a name="error-conditions"></a>오류 조건

|*dest*|*numberOfElements*|*src*|반환 값|내용을 *dest*|
|------------|------------------------|-----------|------------------|------------------------|
|**NULL**|any|any|**EINVAL**|수정 안 됨|
|any|any|**NULL**|**EINVAL**|수정 안 됨|
|any|< *개수*|any|**ERANGE**|수정 안 됨|

## <a name="remarks"></a>설명

복사본 *개수* 문자의 바이트 *src* 하 *dest*합니다. 소스 영역과 대상의 일부 영역이 겹치는 경우 **memmove_s** 겹치는 영역에서 원래 소스 바이트가 덮어쓰기 전에 복사 되는 확인 합니다.

하는 경우 *dest* 이거나 *src* 가 null 포인터인 경우 또는 이러한 함수에 설명 된 대로 잘못 된 매개 변수 처리기를 호출 대상 문자열이 너무 작은 경우 [매개 변수 유효성 검사](../../c-runtime-library/parameter-validation.md) . 실행을 계속 하도록 허용 된 경우 이러한 함수는 반환 **EINVAL** 설정 **errno** 하 **EINVAL**합니다.

## <a name="requirements"></a>요구 사항

|루틴에서 반환된 값|필수 헤더|
|-------------|---------------------|
|**memmove_s**|\<string.h>|
|**wmemmove_s**|\<wchar.h>|

호환성에 대한 자세한 내용은 [호환성](../../c-runtime-library/compatibility.md)을 참조하세요.

## <a name="example"></a>예제

```C
// crt_memmove_s.c
//
// The program demonstrates the
// memmove_s function which works as expected
// for moving overlapping regions.

#include <stdio.h>
#include <string.h>

int main()
{
   char str[] = "0123456789";

   printf("Before: %s\n", str);

   // Move six bytes from the start of the string
   // to a new position shifted by one byte. To protect against
   // buffer overrun, the secure version of memmove requires the
   // the length of the destination string to be specified.

   memmove_s((str + 1), strnlen(str + 1, 10), str, 6);

   printf_s(" After: %s\n", str);
}
```

### <a name="output"></a>출력

```Output
Before: 0123456789
After: 0012345789
```

## <a name="see-also"></a>참고자료

[버퍼 조작](../../c-runtime-library/buffer-manipulation.md)<br/>
[_memccpy](memccpy.md)<br/>
[memcpy, wmemcpy](memcpy-wmemcpy.md)<br/>
[strcpy_s, wcscpy_s, _mbscpy_s](strcpy-s-wcscpy-s-mbscpy-s.md)<br/>
[strcpy, wcscpy, _mbscpy](strcpy-wcscpy-mbscpy.md)<br/>
[strncpy_s, _strncpy_s_l, wcsncpy_s, _wcsncpy_s_l, _mbsncpy_s, _mbsncpy_s_l](strncpy-s-strncpy-s-l-wcsncpy-s-wcsncpy-s-l-mbsncpy-s-mbsncpy-s-l.md)<br/>
[strncpy, _strncpy_l, wcsncpy, _wcsncpy_l, _mbsncpy, _mbsncpy_l](strncpy-strncpy-l-wcsncpy-wcsncpy-l-mbsncpy-mbsncpy-l.md)<br/>
