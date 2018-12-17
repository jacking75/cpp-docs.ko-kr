---
title: 이미지 형식
ms.date: 11/04/2016
ms.assetid: 3ca3654b-42fe-4253-9f2e-723644041aa0
ms.openlocfilehash: 71456af35960114ab64b076ebb9c0f9102613744
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50509943"
---
# <a name="image-format"></a>이미지 형식

실행 가능 이미지 형식은 PE32+입니다. 실행 가능 이미지(DLL 및 EXE)의 최대 크기는 2기가바이트로 제한되어 있으므로 정적 이미지 데이터를 처리하기 위해 32비트 치환된 상대 주소를 사용할 수 있습니다. 이 데이터에는 가져오기 주소 테이블, 문자열 제약 조건, 정적 전역 데이터 등이 포함됩니다.

## <a name="see-also"></a>참고 항목

[x64 소프트웨어 규칙](../build/x64-software-conventions.md)
