---
title: 부동 소수점 보조 프로세서 및 호출 규칙
ms.date: 11/04/2016
helpviewer_keywords:
- floating-point numbers [C++]
- floating-point coprocessor
ms.assetid: 3cc6615a-b308-4cf7-9570-83e192a832b3
ms.openlocfilehash: 7e9184d66bde26ab0e2b345f8f10c2e28619fd2b
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50625111"
---
# <a name="floating-point-coprocessor-and-calling-conventions"></a>부동 소수점 보조 프로세서 및 호출 규칙

를 작성 하는 어셈블리 루틴은 부동 소수점 보조 프로세서 부동 유지 해야 하면 소수점 제어 단어 및 반환 하는 경우가 아니면 보조 프로세서 스택을 정리를 **부동 소수점** 하거나 **double** 값 (함수가 ST(0)에 반환 해야 합니다.

## <a name="see-also"></a>참고자료

[호출 규칙](../cpp/calling-conventions.md)