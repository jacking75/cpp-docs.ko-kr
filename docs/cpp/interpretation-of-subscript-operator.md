---
title: 첨자 연산자의 해석
ms.date: 08/27/2018
helpviewer_keywords:
- subscript operator [C++], interpretation of
- arrays [C++], subscripting
- interpreting subscript operators [C++]
- operators [C++], interpretation of subscript
ms.assetid: 8852ca18-9d5b-43f7-b8bd-abc89364fbf2
ms.openlocfilehash: 1c3d5bca66cb294503805fd5b7691331ac380ae5
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50446607"
---
# <a name="interpretation-of-subscript-operator"></a>첨자 연산자의 해석

다른 연산자와 달리 첨자 연산자 (**\[]**) 사용자가 다시 정의할 수 있습니다. 첨자 연산자의 기본 동작은 다음 메서드를 사용하여 배열 이름과 첨자를 결합하는 것입니다.

\*((*배열 이름과*) + (*첨자*))

포인터 형식을 비롯한 모든 추가에서와 마찬가지로 형식 크기를 조정하기 위해 크기 조정이 자동으로 수행됩니다. 따라서 결과 값이 *첨자* 의 원점부터 바이트 *배열 이름*; 대신 것이 *첨자*번째 배열 요소입니다. (이 변환에 대 한 자세한 내용은 참조 하세요. [가감 연산자](../cpp/additive-operators-plus-and.md).)

다차원 배열에서도 다음 메서드를 사용하여 주소가 파생됩니다.

((*배열 이름과*) + (*첨자*1 \* *max*2 \* *max*3 \* ... \* *max*n) + (*첨자*2 \* *max*3 \* ... \* *max*n)... + + *첨자*n))

## <a name="see-also"></a>참고자료

[배열](../cpp/arrays-cpp.md)<br/>
