---
title: 이미지 영역 선택(아이콘에 대한 이미지 편집기)
ms.date: 11/04/2016
f1_keywords:
- vc.editors.image.editing
helpviewer_keywords:
- Image editor [C++], image selection
- Image editor [C++], selecting images
- images [C++], selecting
- cursors [C++], selecting areas of
ms.assetid: 8b6ce4ad-eba1-4ece-86ba-cea92c3edff2
ms.openlocfilehash: 5e2522d23b30a91639e887a8761871e3df8139f4
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50565115"
---
# <a name="selecting-an-area-of-an-image-image-editor-for-icons"></a>이미지 영역 선택(아이콘에 대한 이미지 편집기)

잘라내기, 복사, 지우기, 크기를 조정, 반전, 또는 이동 하려는 이미지의 영역을 정의 하려면 선택 도구를 사용할 수 있습니다. 사용 하 여 합니다 **사각형 선택** 도구를 정의 하 고 이미지의 사각형 영역을 선택할 수 있습니다. 사용 하 여 합니다 **부정형** 도구 잘라내기, 복사 또는 다른 작업에 대 한 선택 하려는 영역의 윤곽선을 자유롭게 그릴 수 있습니다.

> [!NOTE]
> 참조를 **사각형 선택** 하 고 **부정형** 도구에 나온 [이미지 편집기 도구 모음](../windows/toolbar-image-editor-for-icons.md) 합니다 에각단추와연결된도구팁을보거나**이미지 편집기** 도구 모음입니다.

선택 영역에서 사용자 지정 브러시도 만들 수 있습니다. 자세한 내용은 [사용자 지정 브러시 만들기](../windows/creating-a-custom-brush-image-editor-for-icons.md)합니다.

### <a name="to-select-an-area-of-an-image"></a>이미지 영역 선택

1. 에 **이미지 편집기** 도구 모음 (또는 합니다 **이미지** 메뉴에서 **도구** 명령), 원하는 선택 도구를 클릭 합니다.

2. 선택 하려는 이미지 영역의 한쪽 모퉁이 삽입 지점을 이동 합니다. 십자 모양 커서를 이미지 위로 가져갈 때 표시 됩니다.

3. 선택 하려는 영역의 반대쪽 모퉁이에 커서를 끕니다. 사각형을 보여 줍니다는 픽셀 선택 됩니다. 아래의 사각형을 포함 하 여 사각형 내에서 모든 픽셀 선택 영역에 포함 됩니다.

4. 마우스 단추를 놓습니다. 선택 영역 테두리 선택된 영역을 포함합니다.

### <a name="to-select-an-entire-image"></a>전체 이미지를 선택 합니다.

1. 현재 선택 영역 외부의 이미지를 클릭 합니다. 선택 영역 테두리 포커스 변경 및 다시 한 번에 전체 이미지를 포함 합니다.

관리 되는 프로젝트에 리소스를 추가 하는 방법에 대 한 정보를 참조 하세요 [데스크톱 앱의 리소스](/dotnet/framework/resources/index) 에 *.NET Framework Developer's Guide*합니다. 수동으로 관리 되는 프로젝트에 리소스 파일을 추가, 리소스 액세스, 정적 리소스 표시 및 속성에 리소스 문자열 할당에 대 한 내용은 참조 하세요 [데스크톱 앱에 대 한 리소스 파일 만들기](/dotnet/framework/resources/creating-resource-files-for-desktop-apps)합니다. 전역화 및 지역화 관리 되는 앱의 리소스에 대 한 내용은 참조 하세요 [Globalizing and Localizing.NET Framework Applications](/dotnet/standard/globalization-localization/index)합니다.

## <a name="requirements"></a>요구 사항

없음

## <a name="see-also"></a>참고 항목

[액셀러레이터 키](../windows/accelerator-keys-image-editor-for-icons.md)<br/>
[그래픽 리소스 편집](../windows/editing-graphical-resources-image-editor-for-icons.md)<br/>
[아이콘에 대한 이미지 편집기](../windows/image-editor-for-icons.md)