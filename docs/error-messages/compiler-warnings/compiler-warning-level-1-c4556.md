---
title: 컴파일러 경고(수준 1) C4556
ms.date: 08/27/2018
f1_keywords:
- xml
- C4556
helpviewer_keywords:
- C4556
ms.assetid: e4c0e296-b747-4db1-9608-30b8b74feac2
ms.openlocfilehash: 53261b97249340ce56ce6ae0f5cc0eab7e97a107
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50538491"
---
# <a name="compiler-warning-level-1-c4556"></a>컴파일러 경고(수준 1) C4556

> 직접 실행 내장 인수 값 '*값*'범위를 벗어났습니다'*lowerbound* - *자체도*'

## <a name="remarks"></a>설명

내장 함수는 하드웨어 명령을 일치합니다. 하드웨어 명령에는 고정된 비트 상수를 인코딩할 수 있습니다. 하는 경우 *값* 는 범위를 벗어났거나 인코딩할 수 없으므로 적절 합니다. 컴파일러는 추가 된 비트를 자릅니다.

## <a name="example"></a>예제

다음 샘플에서는 C4556 오류가 생성 됩니다.

```cpp
// C4556.cpp
// compile with: /W1
// processor: x86 IPF
#include <xmmintrin.h>

void test()
{
   __m64 m;
   _m_pextrw(m, 5);   // C4556
}

int main()
{
}
```