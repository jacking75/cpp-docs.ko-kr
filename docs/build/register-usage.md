---
title: 레지스터 사용
ms.date: 11/04/2016
ms.assetid: ce58e2cf-afd3-4068-980e-28a209298265
ms.openlocfilehash: fa04318ad4af298f300fbbbad8c01d0df9500ec7
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50629985"
---
# <a name="register-usage"></a>레지스터 사용

부동 소수점에 사용 가능한 16 XMM/YMM 뿐만 아니라 16 범용 레지스터 (이 하 정수 레지스터)에 대 한 아키텍처를 제공 하는 x64를 등록 합니다. 휘발성 레지스터는 호출자가 호출 중에 제거되는 것으로 가정하는 스크래치 레지스터입니다. 함수 호출 중에 값을 유지하려면 비휘발성 레지스터가 필요합니다. 호출 수신자는 비휘발성 레지스터(사용하는 경우)를 저장해야 합니다.

## <a name="register-volatility-and-preservation"></a>등록 변동성 및 보존

다음 테이블에서는 함수 호출에서 각 레지스터가 사용되는 방법을 설명합니다.

||||
|-|-|-|
|레지스터|상태|기능|
|RAX|휘발성|반환 값 레지스터|
|RCX|휘발성|첫 번째 정수 인수|
|RDX|휘발성|두 번째 정수 인수|
|R8|휘발성|세 번째 정수 인수|
|R9|휘발성|네 번째 정수 인수|
|R10:R11|휘발성|호출자가 필요에 따라 보존해야 하며 syscall/sysret 명령에 사용됨|
|R12:R15|비휘발성|호출 수신자가 보존해야 함|
|RDI|비휘발성|호출 수신자가 보존해야 함|
|RSI|비휘발성|호출 수신자가 보존해야 함|
|RBX|비휘발성|호출 수신자가 보존해야 함|
|RBP|비휘발성|프레임 포인터로 사용 가능(호출 수신자가 보존해야 함)|
|RSP|비휘발성|스택 포인터|
|XMM0, YMM0|휘발성|첫 번째 FP 인수(`__vectorcall` 사용 시에는 첫 번째 벡터 형식 인수)|
|XMM1, YMM1|휘발성|두 번째 FP 인수(`__vectorcall` 사용 시에는 두 번째 벡터 형식 인수)|
|XMM2, YMM2|휘발성|세 번째 FP 인수(`__vectorcall` 사용 시에는 세 번째 벡터 형식 인수)|
|XMM3, YMM3|휘발성|네 번째 FP 인수(`__vectorcall` 사용 시에는 네 번째 벡터 형식 인수)|
|XMM4, YMM4|휘발성|호출자가 필요에 따라 보존해야 함(`__vectorcall` 사용 시에는 다섯 번째 벡터 형식 인수)|
|XMM5, YMM5|휘발성|호출자가 필요에 따라 보존해야 함(`__vectorcall` 사용 시에는 여섯 번째 벡터 형식 인수)|
|XMM6:XMM15, YMM6:YMM15|비휘발성(XMM), 휘발성(YMM의 위쪽 절반)|호출 수신자가 유지 되어야 합니다. YMM 레지스터는 호출자가 필요에 따라 보존해야 함|

함수 종료 시 및 C 런타임 라이브러리 호출 및 Windows 시스템 호출 함수 항목에는 CPU에서 방향 플래그 플래그 레지스터는 지울 수 해야 합니다.

## <a name="see-also"></a>참고자료

- [x64 소프트웨어 규칙](../build/x64-software-conventions.md)
- [__vectorcall](../cpp/vectorcall.md)
- [방향 플래그](../c-runtime-library/direction-flag.md)
