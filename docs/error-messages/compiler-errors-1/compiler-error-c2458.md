---
title: 컴파일러 오류 C2458
ms.date: 11/04/2016
f1_keywords:
- C2458
helpviewer_keywords:
- C2458
ms.assetid: ed21901f-1067-42f5-b275-19b480decf5c
ms.openlocfilehash: 8131b259f89c5cacd07d04edbf6c45adaa25b145
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50637855"
---
# <a name="compiler-error-c2458"></a>컴파일러 오류 C2458

'identifier': 정의 내 재정의

클래스, 구조체, 공용 구조체 또는 열거형 자체 선언에서 다시 정의 됩니다.

다음 샘플에서는 C2458 오류가 생성 됩니다.

```
// C2458.cpp
class C {
   enum i { C };   // C2458
};
```