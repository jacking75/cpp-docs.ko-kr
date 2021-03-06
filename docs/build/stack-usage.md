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

RSP의 현재 주소를 넘는 모든 메모리 일시적인 것으로 간주 됩니다: OS, 또는 디버거 사용자 디버그 세션 또는 인터럽트 처리기 중이 메모리를 덮어쓸 수 있습니다. 따라서 RSP 항상 읽기 또는 스택 프레임으로 값을 쓰기를 시도 하기 전에 설정 해야 합니다.

이 섹션에서는 로컬 변수에 대 한 스택 공간이 할당에 설명 하며 **alloca** 내장 함수입니다.

- [스택 할당](../build/stack-allocation.md)

- [동적 매개 변수 스택 영역 생성](../build/dynamic-parameter-stack-area-construction.md)

- [함수 형식](../build/function-types.md)

- [malloc 맞춤](../build/malloc-alignment.md)

- [alloca](../build/alloca.md)

## <a name="see-also"></a>참고 항목

[x64 소프트웨어 규칙](../build/x64-software-conventions.md)