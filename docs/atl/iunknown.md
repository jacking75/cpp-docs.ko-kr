---
title: IUnknown
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IUnknown
helpviewer_keywords:
- COM interfaces, base interface
- IUnknown interface
ms.assetid: e6b85472-e54b-4b8c-b19f-4454d6c05a8f
ms.openlocfilehash: 760db28f4016ed529b45c72d25eaabf664642cd2
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50430045"
---
# <a name="iunknown"></a>IUnknown

[IUnknown](/windows/desktop/api/unknwn/nn-unknwn-iunknown) 마다 다른 COM 인터페이스의 기본 인터페이스입니다.  이 인터페이스는 세 가지 메서드를 정의 합니다. [QueryInterface](/windows/desktop/api/unknwn/nf-unknwn-iunknown-queryinterface(q_)), [AddRef](/windows/desktop/api/unknwn/nf-unknwn-iunknown-addref), 및 [릴리스](/windows/desktop/api/unknwn/nf-unknwn-iunknown-release). [QueryInterface](/windows/desktop/api/unknwn/nf-unknwn-iunknown-queryinterface(q_)) 인터페이스 사용자가 다른 인터페이스에 대 한 포인터에 대 한 개체를 요청할 수 있습니다. [AddRef](/windows/desktop/api/unknwn/nf-unknwn-iunknown-addref) 하 고 [릴리스](/windows/desktop/api/unknwn/nf-unknwn-iunknown-release) 인터페이스의 참조 횟수를 구현 합니다.

## <a name="see-also"></a>참고 항목

[COM 소개](../atl/introduction-to-com.md)<br/>
[IUnknown 및 인터페이스 상속](/windows/desktop/com/iunknown-and-interface-inheritance)

