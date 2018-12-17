---
title: 프로토타입화되지 않은 함수
ms.date: 11/04/2016
ms.assetid: 34200b8c-5b52-4f0d-aff8-9f70d82868ed
ms.openlocfilehash: 38207be6111dadc338593e55b683b88e0480e1ca
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50633430"
---
# <a name="unprototyped-functions"></a>프로토타입화되지 않은 함수

완전히 프로토타입화되지 않은 함수에 대해 호출자는 정수 값을 정수로 전달하고 부동 소수점 값을 배정밀도로 전달합니다. 호출 수신자에게 정수 레지스터의 값이 필요한 경우 부동 소수점 값에 대해서만 정수 레지스터와 부동 소수점 레지스터에 모두 부동 소수점 값이 포함됩니다.

```
func1();
func2() {   // RCX = 2, RDX = XMM1 = 1.0, and R8 = 7
   func1(2, 1.0, 7);
}
```

## <a name="see-also"></a>참고 항목

[호출 규칙](../build/calling-convention.md)
