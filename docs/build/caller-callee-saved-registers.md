---
title: 호출자-호출 수신자 저장 레지스터
ms.date: 11/04/2016
ms.assetid: 0533bd4b-d6bb-4ce1-8201-495e16870cbb
ms.openlocfilehash: f34fbfff8e6c61b5d568c073f6b7da2a12e34535
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50654703"
---
# <a name="callercallee-saved-registers"></a>호출자/호출 수신자 저장 레지스터

RAX, RCX, RDX, R8, R9, R10, R11 레지스터는 volatile로 간주되고, 전체 프로그램 최적화 같은 분석에 의해 안전성이 증명될 수 없는 한 함수를 호출할 때 소멸되는 것으로 취급해야 합니다.

RBX, RBP, RDI, RSI, RSP, R12, R13, R14 및 R15 레지스터는 비volatile로 간주되고, 이들 레지스터를 사용하는 함수에서 저장하고 복원해야 합니다.

## <a name="see-also"></a>참고 항목

[호출 규칙](../build/calling-convention.md)
