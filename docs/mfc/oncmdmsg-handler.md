---
title: OnCmdMsg 처리기
ms.date: 11/04/2016
f1_keywords:
- OnCmdMsg
helpviewer_keywords:
- messages, routing
- handlers [MFC]
- command routing [MFC], OnCmdMsg handler
- handlers, OnCmdMessage [MFC]
- OnCmdMessage method [MFC]
ms.assetid: 8df07024-506f-47e7-bba9-1c3bc5ad8ab6
ms.openlocfilehash: 37b3d5ffa3e6492c8c00b8b22eba58d09fad51f2
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50643172"
---
# <a name="oncmdmsg-handler"></a>OnCmdMsg 처리기

각 명령 대상 호출 명령 라우팅을 위해는 `OnCmdMsg` 시퀀스에서 다음 명령 대상의 멤버 함수입니다. 명령을 사용 하 여 대상으로 `OnCmdMsg` 명령을 처리할 수 있는지 여부를 확인 하 고 처리할 수 없는 경우 다른 명령 대상으로 라우팅합니다.

각 명령 대상 클래스 보다 우선 합니다 `OnCmdMsg` 멤버 함수입니다. 재정의 통해 특정 다음 대상에 각 클래스 경로 명령입니다. 프레임 창 예를 들어 항상 명령을 라우팅합니다 현재 자식 창 또는 보기를 표에 표시 된 것 처럼 [표준 명령 경로](../mfc/command-routing.md)합니다.

기본값 `CCmdTarget` 구현의 `OnCmdMsg` 명령 대상 클래스의 메시지 맵을 사용 하 여 수신한 각 명령 메시지에 대 한 처리기 함수에 대 한 검색-동일한 방식으로 표준 메시지 검색 됩니다. 일치 하는 항목을 찾으면 해당 처리기를 호출 합니다. 메시지 맵을 검색 방법은 [방법의 프레임 워크 검색 메시지 맵](../mfc/how-the-framework-searches-message-maps.md)합니다.

## <a name="see-also"></a>참고 항목

[프레임워크가 처리기를 호출하는 방법](../mfc/how-the-framework-calls-a-handler.md)

