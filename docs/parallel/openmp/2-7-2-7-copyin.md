---
title: 2.7.2.7 copyin
ms.date: 11/04/2016
ms.assetid: 76cfb9f8-bf65-4585-adbf-fd933f5606b4
ms.openlocfilehash: 20db32530ee60967245497cdfb12a0fce103f7b7
ms.sourcegitcommit: afd6fac7c519dbc47a4befaece14a919d4e0a8a2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/10/2018
ms.locfileid: "51519531"
---
# <a name="2727-copyin"></a>2.7.2.7 copyin

합니다 **copyin** 에 동일한 값을 할당 하는 메커니즘을 제공 하는 절 **threadprivate** 병렬 영역을 실행 하는 팀에서 각 스레드에 대 한 변수입니다. 에 지정 된 각 변수를 **copyin** 병렬 영역 부분에 스레드 전용 복사본에 할당 하 여 처럼 절, 팀의 마스터 스레드에의 변수 값 복사 됩니다. 구문의 합니다 **copyin** 절은 다음과 같습니다.

```

copyin(
variable-list
)
```

제한 된 **copyin** 절은 다음과 같습니다.

- 에 지정 된 변수를 **copyin** 절에는 액세스 가능 하며 명확한 복사 할당 연산자는 있어야 합니다.

- 에 지정 된 변수를 **copyin** 절 이어야 합니다는 **threadprivate** 변수입니다.