---
title: 보기 및 대화 상자 (c + +)에 ActiveX 컨트롤을 추가 합니다.
ms.date: 11/04/2016
f1_keywords:
- vc.controls.activex
helpviewer_keywords:
- dialog boxes [C++], adding ActiveX controls
- ActiveX controls [C++], adding to dialog boxes
ms.assetid: e1c2e3ae-e1b0-40d3-9766-623007073856
ms.openlocfilehash: 947318fb9f628c1184398c039c9697128b09c869
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50642509"
---
# <a name="viewing-and-adding-activex-controls-to-a-dialog-box-c"></a>보기 및 대화 상자 (c + +)에 ActiveX 컨트롤을 추가 합니다.

Visual Studio에서는 ActiveX 컨트롤을 대화 상자에 삽입할 수 있습니다.

### <a name="to-see-the-activex-controls-you-have-available"></a>사용 가능한 ActiveX 컨트롤을 확인하려면

1. 대화 상자 편집기에서 대화 상자를 엽니다.

2. 대화 상자 본문에서 아무 곳이나 마우스 오른쪽 단추로 클릭합니다.

3. 바로 가기 메뉴에서 **ActiveX 컨트롤 삽입**을 클릭합니다.

   [ActiveX 컨트롤 삽입 대화 상자](../windows/insert-activex-control-dialog-box.md) 가 표시되고 시스템에 있는 모든 ActiveX 컨트롤을 보여 줍니다. 대화 상자 아래쪽에 ActiveX 컨트롤 파일 경로가 표시됩니다.

### <a name="to-add-an-activex-control-to-a-dialog-box"></a>대화 상자에 ActiveX 컨트롤을 추가하려면

1. [ActiveX 컨트롤 삽입 대화 상자](../windows/insert-activex-control-dialog-box.md)에서 대화 상자에 추가할 컨트롤을 선택하고 **확인**을 클릭합니다.

   컨트롤이 대화 상자에 표시되고, 이 대화 상자에서 컨트롤을 편집하거나 다른 컨트롤처럼 컨트롤용 처리기를 만들 수 있습니다.

   > [!NOTE]
   > ActiveX 컨트롤을 [도구 상자 창](/visualstudio/ide/reference/toolbox)에 추가할 수 있습니다.

   > [!CAUTION]
   > 시스템에 일부 ActiveX 컨트롤을 배포하지 못할 수 있습니다. 컨트롤을 설치한 소프트웨어에 대한 사용권 계약을 참조하거나 소프트웨어 회사에 문의하세요.

   컨트롤을 배치할 수 있습니다는 **도구 상자** 창에 쉽게 액세스할 수 있도록 합니다. 자세한 내용은 [도구 상자](/visualstudio/ide/reference/toolbox)를 참조하세요.

관리 되는 프로젝트에 리소스를 추가 하는 방법에 대 한 정보를 참조 하세요 [데스크톱 앱의 리소스](/dotnet/framework/resources/index) 에 *.NET Framework Developer's Guide*합니다. 수동으로 관리 되는 프로젝트에 리소스 파일을 추가, 리소스 액세스, 정적 리소스 표시 및 속성에 리소스 문자열 할당에 대 한 내용은 참조 하세요 [데스크톱 앱에 대 한 리소스 파일 만들기](/dotnet/framework/resources/creating-resource-files-for-desktop-apps)합니다. 전역화 및 지역화 관리 되는 앱의 리소스에 대 한 내용은 참조 하세요 [Globalizing and Localizing.NET Framework Applications](/dotnet/standard/globalization-localization/index)합니다.

## <a name="requirements"></a>요구 사항

Win32

## <a name="see-also"></a>참고 항목

[대화 상자의 컨트롤](../windows/controls-in-dialog-boxes.md)<br/>
[MFC ActiveX 컨트롤](../mfc/mfc-activex-controls.md)<br/>
[ActiveX 컨트롤 컨테이너](../mfc/activex-control-containers.md)