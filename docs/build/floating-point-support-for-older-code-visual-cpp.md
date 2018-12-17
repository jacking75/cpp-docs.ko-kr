---
title: 이전 코드를 위한 부동 소수점 지원(Visual C++)
ms.date: 11/04/2016
ms.assetid: a2a26b96-7bc2-418a-981a-51aa1a0294a2
ms.openlocfilehash: 2340a4d136dee3438a47ce06793ed9274035250d
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50509645"
---
# <a name="floating-point-support-for-older-code-visual-c"></a>이전 코드를 위한 부동 소수점 지원(Visual C++)

MMX와 부동 소수점 스택 레지스터(MM0-MM7/ST0-ST7)는 컨텍스트를 전환해도 유지됩니다. 이러한 레지스터에 대한 명시적인 호출 규칙은 없습니다. 이러한 레지스터는 커널 모드 코드에서만 사용하도록 엄격하게 제한되어 있습니다.

## <a name="see-also"></a>참고 항목

[호출 규칙](../build/calling-convention.md)
