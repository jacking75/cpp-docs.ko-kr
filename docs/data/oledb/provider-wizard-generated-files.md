---
title: 공급자 마법사가 생성하는 파일
ms.date: 10/18/2018
helpviewer_keywords:
- OLE DB providers, wizard-generated files
ms.assetid: 6e1ac94b-eb90-4abf-82b3-06944b947ebc
ms.openlocfilehash: c93618ebe9d3140864c2c47867ea970777c208b6
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50580936"
---
# <a name="provider-wizard-generated-files"></a>공급자 마법사가 생성하는 파일

합니다 **ATL OLE DB 공급자 마법사** 다음 파일을 생성 합니다. 다음 항목의 짧은 이름을 사용 *사용자 지정*, 하지만 정확한 파일 이름 공급자를 만들 때 선택에 따라 다릅니다.

|파일 이름|설명|
|---------------|-----------------|
|*사용자 지정*RS.cpp|포함 된 명령을 도우미 `Execute` 메서드 및 공급자 열 지도.|
|*사용자 지정*DS.h|데이터 원본 개체를 구현합니다. 이 헤더 파일에는 데이터 원본 속성에 대 한 속성 맵에 포함 되어 있습니다.|
|*사용자 지정*RS.h|명령 및 행 집합 개체를 구현합니다. 이 헤더 파일에는 행 집합 및 명령 속성에 대 한 속성 맵에 포함 되어 있습니다.|
|*사용자 지정*Sess.h|세션 개체를 구현합니다. 이 헤더 파일에는 세션 속성에 대 한 속성 맵에 포함 되어 있습니다.|
|*사용자 지정*.rgs|생성 된 등록 된 개체가 포함 된 **OLE DB 공급자 마법사**합니다.|

## <a name="see-also"></a>참고 항목

[OLE DB 공급자 만들기](../../data/oledb/creating-an-ole-db-provider.md)<br/>
