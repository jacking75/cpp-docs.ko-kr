---
title: 컴파일러 오류 C2523
ms.date: 11/04/2016
f1_keywords:
- C2523
helpviewer_keywords:
- C2523
ms.assetid: 7951b700-8f37-45a0-beb4-a79ae0ced72e
ms.openlocfilehash: 88a55a469fb8bc08d2ae73209c2e98a99dbc1df0
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50482020"
---
# <a name="compiler-error-c2523"></a>컴파일러 오류 C2523

' 클래스:: ~ identifier': 소멸자/종료자 태그 일치 하지 않습니다.

소멸자 이름은 앞에 물결표 클래스 이름 이어야 합니다 (`~`). 생성자와 소멸자는 클래스와 동일한 이름을 가진 멤버만 있습니다.

다음 샘플에서는 C2523 오류가 생성 됩니다.

```
// C2523.cpp
// compile with: /c
class A {
   ~B();    // C2523
   ~A();   // OK
};
```