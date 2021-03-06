---
title: isnan, _isnan, _isnanf
ms.date: 04/05/2018
apiname:
- _isnan
- _isnanf
- isnan
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
- api-ms-win-crt-math-l1-1-0.dll
apitype: DLLExport
f1_keywords:
- _isnan
- isnan
- math/isnan
- math/_isnan
- math/_isnanf
- _isnanf
helpviewer_keywords:
- NAN (not a number)
- _isnan function
- IEEE floating-point representation
- Not a Number (NANs)
- isnan function
ms.assetid: 391fbc5b-89a4-4fba-997e-68f1131caf82
ms.openlocfilehash: ce111569b7caee9d0c7b8f35352c395571ad08b1
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50650868"
---
# <a name="isnan-isnan-isnanf"></a>isnan, _isnan, _isnanf

부동 소수점 값이 NAN(숫자가 아님)인지를 테스트합니다.

## <a name="syntax"></a>구문

```C
int isnan(
   /* floating-point */ x
); /* C-only macro */

int _isnan(
   double x
);

int _isnanf(
   float x
); /* x64 only */

template <class T>
bool isnan(
   T x
) throw(); /* C++ only */
```

### <a name="parameters"></a>매개 변수

*x*<br/>
테스트할 부동 소수점 값입니다.

## <a name="return-value"></a>반환 값

C에서 **isnan** 매크로 및 **_isnan** 및 **_isnanf** 하는 경우 함수는 0이 아닌 값을 반환 인수 *x* nan이 고 그렇지 않으면 이러한 0을 반환 합니다.

C + +에서는 합니다 **isnan** 템플릿 함수가 반환 **true** 하는 경우 인수 *x* nan; 반환이 고, 그렇지 **false**합니다.

## <a name="remarks"></a>설명

C **isnan** 매크로 **_isnan** 하 고 **_isnanf** 부동 소수점 값을 테스트 하는 함수 *x*, 경우 0이 아닌 값을 반환 *x* 아닙니다 수 (NAN) 값입니다. NAN은 지정된 형식에 대해 부동 소수점 연산의 결과를 IEEE-754 부동 소수점 형식으로 나타낼 수 없는 경우 생성됩니다. 출력에 NAN이 나타나는 방법에 대한 자세한 내용은 [printf](printf-printf-l-wprintf-wprintf-l.md)를 참조하세요.

C + +로 컴파일된 경우 합니다 **isnan** 매크로 정의 하지 않은 **isnan** 템플릿 함수가 대신 정의 됩니다. 형식의 값을 반환 **bool** 정수 대신 합니다.

합니다 **_isnan** 하 고 **_isnanf** 함수는 Microsoft 전용입니다. 합니다 **_isnanf** 함수는 x64 용으로 컴파일된 경우에 사용할 수만 있습니다.

## <a name="requirements"></a>요구 사항

|루틴에서 반환된 값|필수 헤더(C)|필수 헤더(C++)|
|-------------|---------------------------|-------------------------------|
|**isnan**, **_isnanf**|\<math.h>|\<math.h> 또는 \<cmath>|
|**_isnan**|\<float.h>|\<float.h> 또는 \<cfloat>|

호환성에 대한 자세한 내용은 [호환성](../../c-runtime-library/compatibility.md)을 참조하세요.

## <a name="see-also"></a>참고자료

[부동 소수점 지원](../../c-runtime-library/floating-point-support.md)<br/>
[_finite, _finitef](finite-finitef.md)<br/>
[_fpclass, _fpclassf](fpclass-fpclassf.md)<br/>
