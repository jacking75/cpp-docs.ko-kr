---
title: 컴파일러 오류 C3665
ms.date: 11/04/2016
f1_keywords:
- C3665
helpviewer_keywords:
- C3665
ms.assetid: 893bb47e-8de1-43aa-af7d-fa47ad149ee9
ms.openlocfilehash: 30aaf67ac9f912059bb5726681e61feabc1e557d
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50644121"
---
# <a name="compiler-error-c3665"></a>컴파일러 오류 C3665

'소멸자': 재정의 지정자는 'keyword' 소멸자/종료자에서 허용 되지 않습니다

키워드는 소멸자 또는 종료자에서 허용 되지 않는 사용 되었습니다.

예를 들어, 소멸자 또는 종료자에는 새 슬롯을 요청할 수 없습니다.  자세한 내용은 [명시적으로 재정의](../../windows/explicit-overrides-cpp-component-extensions.md) 하 고 [소멸자 및 종료자](../../dotnet/how-to-define-and-consume-classes-and-structs-cpp-cli.md#BKMK_Destructors_and_finalizers)합니다.

다음 샘플에서는 C3665 오류가 생성 됩니다.

```
// C3665.cpp
// compile with: /clr
public ref struct R {
   virtual ~R() { }
   virtual void a() { }
};

public ref struct S : R {
   virtual ~S() new {}   // C3665
   virtual void a() new {}   // OK
};
```