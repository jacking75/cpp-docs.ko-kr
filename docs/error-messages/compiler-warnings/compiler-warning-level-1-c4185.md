---
title: 컴파일러 경고(수준 1) C4185
ms.date: 11/04/2016
f1_keywords:
- C4185
helpviewer_keywords:
- C4185
ms.assetid: 37e7063a-35b1-4e05-ae31-e811dced02b9
ms.openlocfilehash: c4cabeb206da8da9f9157a8f8eee65c1894ce024
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50475116"
---
# <a name="compiler-warning-level-1-c4185"></a>컴파일러 경고(수준 1) C4185

알 수 없는 #import 특성 'attribute'를 무시합니다.

attribute는 `#import`의 유효한 특성이 아닙니다. 무시됩니다.

## <a name="example"></a>예제

```
// C4185.cpp
// compile with: /W1 /c
#import "stdole2.tlb" no_such_attribute   // C4185
```