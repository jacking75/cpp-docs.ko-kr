---
title: 컴파일러 오류 C3468
ms.date: 11/04/2016
f1_keywords:
- C3468
helpviewer_keywords:
- C3468
ms.assetid: cfd320db-2f6e-4e0d-ba02-e79ece87e1e0
ms.openlocfilehash: 185bd35bb732f592c75912fe69d4491252fe9d0b
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50476117"
---
# <a name="compiler-error-c3468"></a>컴파일러 오류 C3468

'type': 어셈블리에만 형식을 전달할 수 있습니다.

'`file`'은 어셈블리가 아닙니다.

어셈블리의 형식만 전달할 수 있습니다.

자세한 내용은 [형식 전달 (C + + /cli CLI)](../../windows/type-forwarding-cpp-cli.md)합니다.

## <a name="example"></a>예제

다음 샘플에서는 모듈을 만듭니다.

```
// C3468.cpp
// compile with: /LN /clr
public ref class R {};
```

## <a name="example"></a>예제

다음 샘플에서는 C3468을 생성합니다.

```
// C3468_b.cpp
// compile with: /clr /c
#using "C3468.netmodule"
[ assembly:TypeForwardedTo(R::typeid) ];   // C3468
```