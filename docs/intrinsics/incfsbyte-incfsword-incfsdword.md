---
title: __incfsbyte, __incfsword, __incfsdword
ms.date: 11/04/2016
f1_keywords:
- __incfsword
- __incfsbyte_cpp
- __incfsbyte
- __incfsdword
- __incfsword_cpp
- __incfsdword_cpp
helpviewer_keywords:
- __incfsword intrinsic
- __incfsdword intrinsic
- __incfsbyte intrinsic
ms.assetid: 820457fb-e35e-42d3-bcb6-725da3281c64
ms.openlocfilehash: f9f0bef89b32e1901c2f6b173baa90153b25a71d
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50577894"
---
# <a name="incfsbyte-incfsword-incfsdword"></a>__incfsbyte, __incfsword, __incfsdword

**Microsoft 전용**

값의 시작을 기준으로 오프셋으로 지정 된 메모리 위치에 추가 된 `FS` 세그먼트입니다.

## <a name="syntax"></a>구문

```
void __incfsbyte(
   unsigned long Offset
);
void __incfsword(
   unsigned long Offset
);
void __incfsdword(
   unsigned long Offset
);
```

#### <a name="parameters"></a>매개 변수

*오프셋*<br/>
[in] 시작 부분 으로부터의 오프셋 `FS`합니다.

## <a name="requirements"></a>요구 사항

|내장 함수|아키텍처|
|---------------|------------------|
|`__incfsbyte`|x86|
|`__incfsword`|x86|
|`__incfsdword`|x86|

## <a name="remarks"></a>설명

이러한 내장 함수 에서만 커널 모드에서 사용할 수 있으며 루틴은 내장 함수로 사용할 수 있습니다.

**Microsoft 전용 종료**

## <a name="see-also"></a>참고 항목

[__addfsbyte, \__addfsword, \__addfsdword](../intrinsics/addfsbyte-addfsword-addfsdword.md)<br/>
[__readfsbyte, \__readfsdword, \__readfsqword, \__readfsword](../intrinsics/readfsbyte-readfsdword-readfsqword-readfsword.md)<br/>
[__writefsbyte, \__writefsdword, \__writefsqword, \__writefsword](../intrinsics/writefsbyte-writefsdword-writefsqword-writefsword.md)<br/>
[컴파일러 내장 함수](../intrinsics/compiler-intrinsics.md)