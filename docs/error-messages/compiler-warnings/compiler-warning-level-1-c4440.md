---
title: 컴파일러 경고(수준 1) C4440
ms.date: 11/04/2016
f1_keywords:
- C4440
helpviewer_keywords:
- C4440
ms.assetid: 78b9642a-a93e-401e-9d92-372f6451bc5d
ms.openlocfilehash: ccd7c14cbd078d4740795d25ad772bdc78840a60
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50660058"
---
# <a name="compiler-warning-level-1-c4440"></a>컴파일러 경고(수준 1) C4440

호출 규칙 재정의 'calling_convention1'에서 'calling_convention2' 무시

호출 규칙을 변경 하려고가.

다음 샘플에서는 C4440 오류가 생성 됩니다.

```
// C4440.cpp
// compile with: /W1 /LD /clr
typedef void __clrcall F();
typedef F __cdecl *PFV;   // C4440
```