---
title: 컴파일러 오류 C2053
ms.date: 11/04/2016
f1_keywords:
- C2053
helpviewer_keywords:
- C2053
ms.assetid: 13324c85-13a8-4996-bd42-a31bfe7ff80f
ms.openlocfilehash: be5517ce77872fe395a52c5b1e0070612e205a3d
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50571225"
---
# <a name="compiler-error-c2053"></a>컴파일러 오류 C2053

'identifier': 와이드 문자열이 일치 하지 않습니다.

와이드 문자열은 호환 되지 않는 형식에 할당 됩니다.

다음 샘플에서는 C2053 오류가 생성 됩니다.

```
// C2053.c
int main() {
   char array[] = L"Rika";   // C2053
}
```