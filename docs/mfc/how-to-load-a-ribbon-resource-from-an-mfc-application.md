---
title: '방법: MFC 응용 프로그램에서 리본 리소스 로드'
ms.date: 11/04/2016
helpviewer_keywords:
- ribbon resource [MFC], loading
ms.assetid: 1c76bb8f-6345-414a-9f3f-128815ceadc5
ms.openlocfilehash: 14ba37952d6f8849c51b36901a6bc17404f938e2
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50515156"
---
# <a name="how-to-load-a-ribbon-resource-from-an-mfc-application"></a>방법: MFC 응용 프로그램에서 리본 리소스 로드

응용 프로그램에서 리본 리소스를 사용하려면 응용 프로그램을 수정하여 리본 리소스를 로드합니다.

### <a name="to-load-a-ribbon-resource"></a>리본 리소스를 로드하려면

1. `Ribbon Control` 클래스에서 `CMainFrame` 개체를 선언합니다.

```
    CMFCRibbonBar m_wndRibbonBar;
```

1. `CMainFrame::OnCreate`에서 리본 컨트롤을 만들고 초기화합니다.

```
    if (!m_wndRibbonBar.Create (this))
{
    return -1;
}

    if (!m_wndRibbonBar.LoadFromResource(IDR_RIBBON))
{
    return -1;
}
```

## <a name="see-also"></a>참고 항목

[리본 디자이너(MFC)](../mfc/ribbon-designer-mfc.md)

