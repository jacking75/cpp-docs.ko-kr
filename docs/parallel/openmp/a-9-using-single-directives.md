---
title: A.9   single 지시문 사용
ms.date: 11/04/2016
ms.assetid: 0c0f9495-5794-4db9-883b-a12e3a9f1328
ms.openlocfilehash: 51a2a3438ae5abc9d24c160a986c8ea04b77c4bf
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50501311"
---
# <a name="a9---using-single-directives"></a>A.9   single 지시문 사용

다음 예제는 `single` 지시문 ([2.4.3 섹션](../../parallel/openmp/2-4-3-single-construct.md) 15 페이지). 예제에서는 하나의 스레드만 (발생 하는 첫 번째 스레드는 일반적으로 `single` 지시문) 진행률 메시지를 출력 합니다. 사용자는 스레드를 실행 하도록 어떠한가 정도 해서는 `single` 섹션입니다. 다른 모든 스레드가 건너뜁니다 합니다 `single` 섹션 및 끝의 장애물에 중지를 `single` 생성 합니다. 다른 스레드가 실행 중인 스레드에 기다리지 않고 계속 진행할 수 있습니다는 `single` 섹션을 `nowait` 절에 지정할 수 있습니다는 `single` 지시문입니다.

```
#pragma omp parallel
{
    #pragma omp single
        printf_s("Beginning work1.\n");
    work1();
    #pragma omp single
        printf_s("Finishing work1.\n");
    #pragma omp single nowait
        printf_s("Finished work1 and beginning work2.\n");
    work2();
}
```