---
title: vector&lt;bool&gt;::reference::flip
ms.date: 11/04/2016
f1_keywords:
- vector/std::vector<bool>::reference::flip
helpviewer_keywords:
- reference::flip method
ms.assetid: ef940365-cbe4-4a87-a3e2-1f3cfa357e29
ms.openlocfilehash: 68172de6e50a599d5b1822b83787be3a3a94e037
ms.sourcegitcommit: afd6fac7c519dbc47a4befaece14a919d4e0a8a2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/10/2018
ms.locfileid: "51522547"
---
# <a name="vectorltboolgtreferenceflip"></a>vector&lt;bool&gt;::reference::flip

참조된 [vector\<bool>](../standard-library/vector-bool-class.md) 요소의 부울 값을 반전합니다.

## <a name="syntax"></a>구문

```cpp
void flip();
```

## <a name="example"></a>예제

```cpp
// vector_bool_ref_flip.cpp
// compile with: /EHsc /W4
#include <vector>
#include <iostream>

int main()
{
    using namespace std;
    cout << boolalpha;

    vector<bool> vb = { true, false, false, true, true };

    cout << "The vector is: " << endl << "    ";
    for (const auto& b : vb) {
        cout << b << " ";
    }
    cout << endl;

    vector<bool>::reference vbref = vb.front();
    vbref.flip();

    cout << "The vector with first element flipped is: " << endl << "    ";
    for (const auto& b : vb) {
        cout << b << " ";
    }
    cout << endl;
}
```

## <a name="output"></a>출력

```Output
The vector is:
    true false false true true
The vector with first element flipped is:
    false false false true true
```

## <a name="requirements"></a>요구 사항

**헤더:** \<vector>

**네임스페이스:** std

## <a name="see-also"></a>참고자료

[벡터\<bool >:: reference 클래스](../standard-library/vector-bool-reference-class.md)<br/>
[C++ 표준 라이브러리 참조](../standard-library/cpp-standard-library-reference.md)<br/>
