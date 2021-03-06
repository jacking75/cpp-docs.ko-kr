---
title: A.20   barrier 지시문 바인딩
ms.date: 11/04/2016
ms.assetid: a3fdcc26-6873-429b-998e-de451401483b
ms.openlocfilehash: cf6f20a8539c47ca529af93e65f3a5fe244228d8
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50652948"
---
# <a name="a20---binding-of-barrier-directives"></a>A.20   barrier 지시문 바인딩

지시문 바인딩 규칙에 대 한 호출을 **장벽** 지시문에 가장 가까운 바깥쪽 바인딩할 `parallel` 지시문입니다. 지시문 바인딩에 대 한 자세한 내용은 참조 하세요. [섹션 2.8](../../parallel/openmp/2-8-directive-binding.md) 32 페이지입니다.

다음 예제에서는 식에서 호출 *주* 하 *sub2* 규격이 때문에 **장벽** (에서 *sub3*) 병렬 영역에 바인딩합니다 *sub2*합니다. 호출 *주* 하 *sub1* 규격이 때문에 **장벽** 서브루틴의 병렬 영역에 바인딩합니다 *sub2*합니다.  식에서 호출 *주* 하 *sub3* 규격이 때문에 **장벽** 바인딩할 수 없으면 모든 병렬 영역 및 무시 됩니다. 또한 합니다 **장벽** 팀에서 만든 모든 스레드 및 바깥쪽 병렬 영역에서 스레드 동기화 *sub1*합니다.

```
int main()
{
    sub1(2);
    sub2(2);
    sub3(2);
}

void sub1(int n)
{
    int i;
    #pragma omp parallel private(i) shared(n)
    {
        #pragma omp for
        for (i=0; i<n; i++)
            sub2(i);
    }
}

void sub2(int k)
{
     #pragma omp parallel shared(k)
     sub3(k);
}

void sub3(int n)
{
    work(n);
    #pragma omp barrier
    work(n);
}
```