---
title: 컴파일러 오류 C3611
ms.date: 11/04/2016
f1_keywords:
- C3611
helpviewer_keywords:
- C3611
ms.assetid: 42f3e320-41de-420a-bd05-8924cab765aa
ms.openlocfilehash: 08e9b969c9eb03dd0259813487bfeb04bfaa5ca9
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50590245"
---
# <a name="compiler-error-c3611"></a>컴파일러 오류 C3611

'function': 봉인 된 함수는 순수 지정자를 사용할 수 없습니다

봉인 된 함수를 잘못 선언 되었습니다.  자세한 내용은 [봉인](../../windows/sealed-cpp-component-extensions.md)합니다.

## <a name="example"></a>예제

다음 샘플 C3611를 생성합니다.

```
// C3611.cpp
// compile with: /clr /c

ref struct V {
   virtual void Test() sealed = 0;   // C3611
   virtual void Test2() sealed;   // OK
   virtual void Test3() = 0;   // OK
};
```