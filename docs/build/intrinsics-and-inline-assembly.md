---
title: 내장 및 인라인 어셈블리
ms.date: 11/04/2016
ms.assetid: 8affd4bb-279d-46f3-851f-8be0a9c5ed3f
ms.openlocfilehash: 033225259c0a33414fe45eba313bb1f1c94eb379
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50515104"
---
# <a name="intrinsics-and-inline-assembly"></a>내장 및 인라인 어셈블리

x64 컴파일러의 제약 조건 중 하나는 인라인 어셈블러를 지원하지 않는다는 것입니다. 즉, C 또는 C++로 작성할 수 없는 함수는 컴파일러에서 지원하는 내장 함수나 서브루틴으로 작성해야 합니다. 함수에 따라서는 성능에 큰 영향을 미칠 수도 있습니다. 성능에 중요한 부분을 차지하는 함수는 내장 함수로 구현해야 합니다.
컴파일러에서 지원하는 내장 함수에 대한 자세한 내용은 [컴파일러 내장 함수](../intrinsics/compiler-intrinsics.md)를 참조하십시오.

## <a name="see-also"></a>참고 항목

[x64 소프트웨어 규칙](../build/x64-software-conventions.md)
