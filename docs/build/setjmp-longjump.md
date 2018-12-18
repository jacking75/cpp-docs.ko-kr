---
title: setjmp longjump
ms.date: 11/04/2016
ms.assetid: b0e21902-095d-4198-8f9a-b6326525721a
ms.openlocfilehash: 765cef3f02bed09bed0278aaeecdcdbd55d86b67
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50427900"
---
# <a name="setjmplongjump"></a>setjmp/longjump

Setjmp.h나 setjmpex.h를 포함하는 경우 [setjmp](../c-runtime-library/reference/setjmp.md) 또는 [longjmp](../c-runtime-library/reference/longjmp.md)에 대한 모든 호출 결과로 소멸자와 finally 호출을 호출하는 해제가 발생합니다. 이는 setjmp.h를 포함해도 finally 절과 소멸자가 호출되지 않는 x86의 경우와 다른 점입니다.

`setjmp`에 대한 호출은 현재 스택 포인터, 비volatile 레지스터 및 MxCsr 레지스터를 유지합니다. `longjmp`에 대한 호출은 가장 최근의 `setjmp` 호출 사이트에 반환되고 스택 포인터, 비 volatile 레지스터 및 MxCsr 레지스터를 가장 최근의 `setjmp` 호출에서 유지한 상태로 다시 설정합니다.

## <a name="see-also"></a>참고 항목

[호출 규칙](../build/calling-convention.md)
