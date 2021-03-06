---
title: (C + +)를 편집 하는 리소스에 영향을 받는 파일
ms.date: 06/18/2018
helpviewer_keywords:
- resource editing
- resources [C++], editing
ms.assetid: d0820df1-ba84-40ac-bce9-29ea5ee7e3f8
ms.openlocfilehash: 891794f42f3df1ab23d64c253ab4df8291e3ddcf
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50663306"
---
# <a name="files-affected-by-resource-editing-c"></a>(C + +)를 편집 하는 리소스에 영향을 받는 파일

Visual Studio 환경은 리소스 편집 세션 중 다음 표에 표시된 파일에서 작동합니다.

|파일 이름|설명|
|---------------|-----------------|
|Resource.h|개발 환경에서 생성된 헤더 파일로, 기호 정의를 포함합니다. (소스 제어에이 파일을 포함 합니다.)|
|Filename.aps|현재 리소스 스크립트 파일의 이진 버전으로, 빠른 로드를 위해 사용됩니다.<br /><br /> 리소스 편집기에서 .rc 또는 resource.h 파일을 직접 읽지 않습니다. 리소스 컴파일러는 리소스 편집기에서 사용되는 이러한 파일을 .aps 파일로 컴파일합니다. 이 파일은 컴파일 단계이며 기호화된 데이터만 저장합니다. 일반적인 컴파일 프로세스에서처럼 기호화되지 않은 정보(예: 주석)는 컴파일 프로세스 중에 삭제됩니다. .aps 파일이 .rc 파일과 동기화되지 않을 때마다 .rc 파일이 다시 생성됩니다. 예를 들어 저장하면 리소스 편집기에서 .rc 파일 및 resource.h 파일을 덮어씁니다. 리소스 자체의 모든 변경 내용은 .rc 파일에 통합된 상태로 유지되지만 주석은 .rc 파일을 덮어쓰면 항상 손실됩니다. 주석을 유지 하는 방법에 대 한 자세한 내용은 [컴파일 타임에 리소스 포함](../windows/how-to-include-resources-at-compile-time.md)합니다. (일반적으로 있습니다 포함 되지 않습니다.aps 파일이 소스 제어에.)|
|.rc|현재 프로젝트의 리소스에 대한 스크립트가 포함된 리소스 스크립트 파일입니다. 저장할 때마다 .aps 파일이 이 파일을 덮어씁니다. (소스 제어에이 파일을 포함 합니다.)|

## <a name="requirements"></a>요구 사항

Win32

## <a name="see-also"></a>참고 항목

[리소스 파일](../windows/resource-files-visual-studio.md)