---
title: 컴파일러 오류 C2496
ms.date: 11/04/2016
f1_keywords:
- C2496
helpviewer_keywords:
- C2496
ms.assetid: 9a25237d-5bbb-4112-98f3-29cd99d3f89f
ms.openlocfilehash: 258012fdefed877558f122790954d830095d5026
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50578700"
---
# <a name="compiler-error-c2496"></a>컴파일러 오류 C2496

'identifier': 'selectany' 외부 링크가 있는 데이터 항목에만 적용 될 수 있습니다

합니다 [selectany](../../cpp/selectany.md) 외부적으로 표시 되 고 전역 데이터 항목에만 특성을 적용할 수 있습니다.

다음 샘플에서는 C2496 오류가 생성 됩니다.

```
// C2496.cpp
// compile with: /c
__declspec(selectany) int x1 = 1;
const __declspec(selectany) int x2 = 2;   // C2496
static __declspec(selectany) int x6 = 6;   // C2496

extern const __declspec(selectany) int x3 = 3;

__declspec(selectany) int x4;

// dynamic initialization of x5
int f();
__declspec(selectany) int x5 = f();

extern const int x7;
// OK - redeclaration of x7 that is extern
const __declspec(selectany) int x7 = 7;
```