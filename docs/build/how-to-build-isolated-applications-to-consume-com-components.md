---
title: '방법: COM 구성 요소를 사용하는 격리된 응용 프로그램 빌드'
ms.date: 11/04/2016
helpviewer_keywords:
- isolated applications [C++]
ms.assetid: 04587547-1174-44ab-bd99-1292358fba20
ms.openlocfilehash: ba35c016996604e2b433083c2de7b9ddc807d52c
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50587540"
---
# <a name="how-to-build-isolated-applications-to-consume-com-components"></a>방법: COM 구성 요소를 사용하는 격리된 응용 프로그램 빌드

격리 된 응용 프로그램은 프로그램에서 기본 제공 하는 매니페스트를가 하는 응용 프로그램. COM 구성 요소를 사용 하는 격리 된 응용 프로그램을 만들 수 있습니다.

### <a name="to-add-com-references-to-manifests-of-isolated-applications"></a>격리 된 응용 프로그램의 매니페스트를 COM 참조를 추가 하려면

1. 격리 된 응용 프로그램에 대 한 프로젝트 속성 페이지를 엽니다.

1. 확장을 **구성 속성** 노드를 차례로 확장 합니다 **매니페스트 도구** 노드.

1. 선택 합니다 **격리 COM** 속성 페이지 및 설정 합니다 **구성 요소 파일 이름** 속성을 격리 된 응용 프로그램에서 사용 하는 COM 구성 요소의 이름입니다.

1. **확인**을 클릭합니다.

### <a name="to-build-manifests-into-isolated-applications"></a>격리 된 응용 프로그램에 매니페스트를 빌드

1. 격리 된 응용 프로그램에 대 한 프로젝트 속성 페이지를 엽니다.

1. 확장을 **구성 속성** 노드를 차례로 확장 합니다 **매니페스트 도구** 노드.

1. 선택 된 **입력 및 출력** 속성 페이지 및 설정 합니다 **매니페스트 포함** 속성이 **예**합니다.

1. **확인**을 클릭합니다.

1. 솔루션을 빌드합니다.

## <a name="see-also"></a>참고 항목

[격리된 응용 프로그램](/windows/desktop/SbsCs/isolated-applications)<br/>
[Side-by-side-어셈블리에 대 한](/windows/desktop/SbsCs/about-side-by-side-assemblies-)