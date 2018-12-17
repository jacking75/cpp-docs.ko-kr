---
title: 스택 사용
ms.date: 11/04/2016
ms.assetid: 383f0072-0438-489f-8829-cca89582408c
ms.openlocfilehash: 5ee9da50a03e1137ed6543cd349481148c9127d6
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50452223"
---
# <a name="stack-usage"></a>스택 사용

RSP의 현재 주소를 벗어난 모든 메모리는 volatile로 간주됩니다. 운영 체제나 디버거는 사용자 디버그 세션을 진행하는 동안 또는 중단 처리기에서 이 메모리를 덮어쓸 수 있습니다. 따라서 값을 스택 프레임에서 읽거나 스택 프레임에 쓰기 전에 항상 RSP를 설정해야 합니다.

이 단원에서는 지역 변수에 대한 스택 공간 할당 및 **alloca** 내장 함수에 대해 설명합니다


- [스택 할당](../build/stack-allocation.md)

- [동적 매개 변수 스택 영역 생성](../build/dynamic-parameter-stack-area-construction.md)

- [함수 형식](../build/function-types.md)

- [malloc 맞춤](../build/malloc-alignment.md)

- [alloca](../build/alloca.md)

## <a name="see-also"></a>참고 항목
[x64 소프트웨어 규칙](../build/x64-software-conventions.md)
