---
title: __svm_invlpga
ms.date: 11/04/2016
f1_keywords:
- __svm_invlpga
helpviewer_keywords:
- __svm_invlpga intrinsic
- INVLPGA instruction
ms.assetid: aa6578ce-8278-464b-8815-a0fc45330915
ms.openlocfilehash: 2d356cf7426c558c8ac0312eff02c0cb9de9c859
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50544302"
---
# <a name="svminvlpga"></a>__svm_invlpga

**Microsoft 전용**

컴퓨터의 translation lookaside buffer 주소 매핑 항목을 무효화합니다. 매개 변수는 가상 주소 및 무효화 페이지의 주소 공간 식별자를 지정 합니다.

## <a name="syntax"></a>구문

```
void __svm_invlpga(void *Va, int ASID);
```

#### <a name="parameters"></a>매개 변수

|매개 변수|설명|
|---------------|-----------------|
|*Va*|[in] 무효화할 페이지의 가상 주소입니다.|
|*ASID*|[in] 주소 공간 식별자 (ASID)를 무효화 하려면 페이지의입니다.|

## <a name="remarks"></a>설명

`__svm_invlpga` 함수는 `INVLPGA` 컴퓨터 명령에 해당합니다. 이 함수는 게스트 운영 체제 및 해당 응용 프로그램과 호스트 가상 머신 모니터의 상호 작용을 지원합니다. 자세한 내용은 문서를 검색 "AMD64 아키텍처 프로그래머 수동 볼륨 2: 시스템 프로그래밍"에서 24593, 3.11, 수정 버전 번호를 문서화 합니다 [AMD corporation](https://developer.amd.com/resources/developer-guides-manuals/) 사이트입니다.

## <a name="requirements"></a>요구 사항

|내장 함수|아키텍처|
|---------------|------------------|
|`__svm_invlpga`|x86, x64|

**헤더 파일** \<intrin.h >

**Microsoft 전용 종료**

## <a name="see-also"></a>참고 항목

[컴파일러 내장 함수](../intrinsics/compiler-intrinsics.md)