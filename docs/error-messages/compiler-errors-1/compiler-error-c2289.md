---
title: 컴파일러 오류 C2289
ms.date: 11/04/2016
f1_keywords:
- C2289
helpviewer_keywords:
- C2289
ms.assetid: cb41a29e-1b06-47dc-bfce-8d73bd63a0df
ms.openlocfilehash: 9fe9b765af72a8864e3e899cafcf648a9facb67e
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50528130"
---
# <a name="compiler-error-c2289"></a>컴파일러 오류 C2289

동일한 형식 한정자를 두 번 이상 사용했습니다.

형식 선언 또는 정의에서 형식 한정자(`const`, `volatile`, `signed`또는 `unsigned`)를 두 번 이상 사용하여 ANSI 호환성(**/Za**)에서 오류가 발생합니다.

다음 샘플에서는 C2286을 생성합니다.

```
// C2289.cpp
// compile with: /Za /c
volatile volatile int i;   // C2289
volatile int j;   // OK
```