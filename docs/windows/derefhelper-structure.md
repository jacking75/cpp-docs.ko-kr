---
title: DerefHelper 구조체
ms.date: 10/03/2018
ms.topic: reference
f1_keywords:
- async/Microsoft::WRL::Details::DerefHelper
helpviewer_keywords:
- DerefHelper structure
ms.assetid: 86ded58b-c3ee-4a4f-bb86-4f67b895d427
ms.openlocfilehash: 7e9de446fdf18b3cf92cc438e421287c8fcfc29f
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50450198"
---
# <a name="derefhelper-structure"></a>DerefHelper 구조체

WRL 인프라를 지원하며 사용자 코드에서 직접 사용할 수 없습니다.

## <a name="syntax"></a>구문

```cpp
template <typename T>
struct DerefHelper;

template <typename T>
struct DerefHelper<T*>;
```

### <a name="parameters"></a>매개 변수

*T*<br/>
템플릿 매개 변수입니다.

## <a name="remarks"></a>설명

에 대 한 역참조 포인터를 나타내는 `T*` 템플릿 매개 변수입니다.

**DerefHelper** 과 같은 식에 사용 됩니다. `ComPtr<Details::DerefHelper<ProgressTraits::Arg1Type>::DerefType> operationInterface;`합니다.

## <a name="members"></a>멤버

### <a name="public-typedefs"></a>공용 Typedefs

|이름|설명|
|----------|-----------------|
|`DerefType`|역참조 템플릿 매개 변수 식별자 `T*`합니다.|

## <a name="inheritance-hierarchy"></a>상속 계층

`DerefHelper`

## <a name="requirements"></a>요구 사항

**헤더:** async.h

**Namespace:** Microsoft::WRL::Details

## <a name="see-also"></a>참고 항목

[Microsoft::WRL::Details 네임스페이스](../windows/microsoft-wrl-details-namespace.md)