---
title: 컴파일러 오류 C3032
ms.date: 11/04/2016
f1_keywords:
- C3032
helpviewer_keywords:
- C3032
ms.assetid: 6a92bd8e-319f-4a99-aef4-a9021f6f9928
ms.openlocfilehash: 8e103d36bf3e49cfbb0a3724c044794601aabcee
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50567247"
---
# <a name="compiler-error-c3032"></a>컴파일러 오류 C3032

'var': 'clause' 절의 변수는 불완전한 형식 'type'이 될 수 없습니다.

특정 절에 전달되는 형식은 컴파일러에 완벽하게 표시되어야 합니다.

다음 샘플에서는 C3032를 생성합니다.

```
// C3032.cpp
// compile with: /openmp /link vcomps.lib
#include "omp.h"

struct Incomplete;
extern struct Incomplete inc;

int main() {
   int i = 9;
   #pragma omp parallel private(inc)   // C3032
      ;

   #pragma omp parallel private(i)     // OK
      ;

}
```