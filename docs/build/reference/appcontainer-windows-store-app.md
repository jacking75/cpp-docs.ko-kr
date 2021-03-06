---
title: /APPCONTAINER (UWP/Microsoft Store 앱)
ms.date: 11/04/2016
ms.assetid: 9a432db5-7640-460b-ab18-6f61fa7daf6f
ms.openlocfilehash: 306ffc7cda7cc6045b5decd6824fdc3848233824
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50541325"
---
# <a name="appcontainer-microsoft-store-app"></a>/APPCONTAINER (Microsoft Store 앱)

링커는 앱 컨테이너에서 실행 해야 하는 실행 가능 이미지를 만드는 지 여부를 지정 합니다.

## <a name="syntax"></a>구문

```
/APPCONTAINER[:NO]
```

## <a name="remarks"></a>설명

기본적으로 /APPCONTAINER는 해제 됩니다.

이 옵션을 appcontainer 프로세스 격리 환경에서 앱을 실행 해야 하는지 여부를 나타내는 실행 파일을 수정 합니다. Appcontainer 환경에서 실행 해야 하는 앱에 대해 /APPCONTAINER를 지정 합니다.-예를 들어, 유니버설 Windows 플랫폼 (UWP) 또는 Windows Phone 8.x 앱에 있습니다. (옵션을 자동 설정 됩니다 Visual Studio의 템플릿에서 유니버설 Windows 앱을 만들 때.) 데스크톱 앱의 경우 /APPCONTAINER:NO 지정 하거나 옵션을 생략 합니다.

/APPCONTAINER 옵션은 Windows 8에서 도입 되었습니다.

### <a name="to-set-this-linker-option-in-visual-studio"></a>Visual Studio에서 이 링커 옵션을 설정하려면

1. 프로젝트 **속성 페이지** 대화 상자를 엽니다. 자세한 내용은 [프로젝트 속성 작업](../../ide/working-with-project-properties.md)을 참조하세요.

1. **구성 속성** 노드를 확장합니다.

1. 확장 된 **링커** 노드.

1. 선택 된 **명령줄** 속성 페이지.

1. **추가 옵션**를 입력 `/APPCONTAINER` 또는 `/APPCONTAINER:NO`합니다.

## <a name="see-also"></a>참고 항목

[링커 옵션 설정](../../build/reference/setting-linker-options.md)<br/>
[링커 옵션](../../build/reference/linker-options.md)