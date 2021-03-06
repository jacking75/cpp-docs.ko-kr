---
title: _finite, _finitef
ms.date: 04/05/2018
apiname:
- _finite
- _finitef
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
- finite
- _finite
- _finitef
- math/_finite
- math/_finitef
- float/_finite
helpviewer_keywords:
- finite function
- _finite function
- _finitef function
ms.assetid: 5a7d7ca7-befb-4e1f-831d-28713c6eb805
ms.openlocfilehash: 7b1bce6f1b2da77ed9de255f49dd8d0160e33e31
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50431666"
---
# <a name="finite-finitef"></a>_finite, _finitef

부동 소수점 값이 유한인지 확인합니다.

## <a name="syntax"></a>구문

```C
int _finite(
   double x
);

int _finitef(
   float x
); /* x64 and ARM/ARM64 only */
```

### <a name="parameters"></a>매개 변수

*x*<br/>
테스트할 부동 소수점 값입니다.

## <a name="return-value"></a>반환 값

둘 다 **_finite** 하 고 **_finitef** 경우 0이 아닌 값을 반환 인수 *x* 는 유한 인 경우,-INF < *x* < + INF입니다. 인수가 무한이거나 NAN이면 0을 반환합니다.

## <a name="remarks"></a>설명

합니다 **_finite** 하 고 **_finitef** 함수는 Microsoft 전용입니다. 합니다 **_finitef** 함수는만 플랫폼을 x86, ARM 또는 ARM64 컴파일된 경우 사용할 수 있습니다.

## <a name="requirements"></a>요구 사항

|기능|필수 헤더(C)|필수 헤더(C++)|
|--------------|---------------------------|-------------------------------|
|**_finite**|\<float.h> 또는 \<math.h>|\<float.h>, \<math.h>, \<cfloat> 또는 \<cmath>|
|**_finitef**|\<math.h>|\<math.h> 또는 \<cmath>|

호환성에 대한 자세한 내용은 [호환성](../../c-runtime-library/compatibility.md)을 참조하세요.

## <a name="see-also"></a>참고자료

[부동 소수점 지원](../../c-runtime-library/floating-point-support.md)<br/>
[isnan, _isnan, _isnanf](isnan-isnan-isnanf.md)<br/>
[_fpclass, _fpclassf](fpclass-fpclassf.md)<br/>
