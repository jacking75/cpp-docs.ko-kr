---
title: 컴파일러 오류 C3132
ms.date: 11/04/2016
f1_keywords:
- C3132
helpviewer_keywords:
- C3132
ms.assetid: d54a3d12-336a-4ed0-ad4e-43cddac33b5e
ms.openlocfilehash: a4c6ce8005aecd094c57b3dbda5c95565deecb95
ms.sourcegitcommit: afd6fac7c519dbc47a4befaece14a919d4e0a8a2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/10/2018
ms.locfileid: "51519804"
---
# <a name="compiler-error-c3132"></a>컴파일러 오류 C3132

' 함수 매개 변수 ': '관리 되는 1 차원 배열' 형식의 형식 인수에 매개 변수 배열만 적용할 수

합니다 [ParamArray](https://msdn.microsoft.com/library/system.paramarrayattribute.aspx) 없는 1 차원 배열 매개 변수에 특성이 적용 되었습니다.

다음 샘플에서는 C3132 오류가 생성 됩니다.

```
// C3132.cpp
// compile with: /clr /c
using namespace System;
void f( [ParamArray] Int32[,] );   // C3132
void g( [ParamArray] Int32[] );   // C3132

void h( [ParamArray] array<Char ^> ^ MyArray );   // OK
```