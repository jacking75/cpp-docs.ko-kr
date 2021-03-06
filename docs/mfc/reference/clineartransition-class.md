---
title: CLinearTransition 클래스
ms.date: 11/04/2016
f1_keywords:
- CLinearTransition
- AFXANIMATIONCONTROLLER/CLinearTransition
- AFXANIMATIONCONTROLLER/CLinearTransition::CLinearTransition
- AFXANIMATIONCONTROLLER/CLinearTransition::Create
- AFXANIMATIONCONTROLLER/CLinearTransition::m_dblFinalValue
- AFXANIMATIONCONTROLLER/CLinearTransition::m_duration
helpviewer_keywords:
- CLinearTransition [MFC], CLinearTransition
- CLinearTransition [MFC], Create
- CLinearTransition [MFC], m_dblFinalValue
- CLinearTransition [MFC], m_duration
ms.assetid: 7fcb2dba-beb8-4933-9f5d-3b7fb1585ef0
ms.openlocfilehash: b671057d0abc01f31d5625d5be0e9678207d8abe
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50432749"
---
# <a name="clineartransition-class"></a>CLinearTransition 클래스

선형 전환을 캡슐화합니다.

## <a name="syntax"></a>구문

```
class CLinearTransition : public CBaseTransition;
```

## <a name="members"></a>멤버

### <a name="public-constructors"></a>Public 생성자

|이름|설명|
|----------|-----------------|
|[CLinearTransition::CLinearTransition](#clineartransition)|선형 전환을 개체를 생성 하 고 기간 및 최종 값을 사용 하 여 초기화 합니다.|

### <a name="public-methods"></a>Public 메서드

|이름|설명|
|----------|-----------------|
|[CLinearTransition::Create](#create)|캡슐화 된 전환 COM 개체를 만들려면 전환 라이브러리를 호출 합니다. (재정의 [CBaseTransition::Create](../../mfc/reference/cbasetransition-class.md#create).)|

### <a name="public-data-members"></a>공용 데이터 멤버

|이름|설명|
|----------|-----------------|
|[CLinearTransition::m_dblFinalValue](#m_dblfinalvalue)|전환의 끝에 있는 애니메이션 변수의 값입니다.|
|[CLinearTransition::m_duration](#m_duration)|전환 기간입니다.|

## <a name="remarks"></a>설명

선형 전환 하는 동안 애니메이션 변수의 값 선형적으로 전환 초기 값에서 지정 된 마지막 값입니다. 모든 전환을 자동으로 취소 하므로 것이 좋습니다에 할당 된 새 연산자를 사용 합니다. 캡슐화 된 IUIAnimationTransition COM 개체는 NULL까지 CAnimationController::AnimateGroup에서 생성 됩니다. 이 COM 개체의 생성에 영향을 주지 않습니다 후 멤버 변수를 변경 합니다.

## <a name="inheritance-hierarchy"></a>상속 계층

[CObject](../../mfc/reference/cobject-class.md)

[CBaseTransition](../../mfc/reference/cbasetransition-class.md)

[CLinearTransition](../../mfc/reference/clineartransition-class.md)

## <a name="requirements"></a>요구 사항

**헤더:** afxanimationcontroller.h

##  <a name="clineartransition"></a>  CLinearTransition::CLinearTransition

선형 전환을 개체를 생성 하 고 기간 및 최종 값을 사용 하 여 초기화 합니다.

```
CLinearTransition(
    UI_ANIMATION_SECONDS duration,
    DOUBLE dblFinalValue);
```

### <a name="parameters"></a>매개 변수

*duration*<br/>
전환 기간입니다.

*dblFinalValue*<br/>
전환의 끝에 있는 애니메이션 변수의 값입니다.

##  <a name="create"></a>  CLinearTransition::Create

캡슐화 된 전환 COM 개체를 만들려면 전환 라이브러리를 호출 합니다.

```
virtual BOOL Create(
    IUIAnimationTransitionLibrary* pLibrary,
    IUIAnimationTransitionFactory* \*not used*\);
```

### <a name="parameters"></a>매개 변수

*pLibrary*<br/>
에 대 한 포인터를 [IUIAnimationTransitionLibrary 인터페이스](/windows/desktop/api/uianimation/nn-uianimation-iuianimationtransitionlibrary), 표준 전환의 라이브러리를 정의 하는 합니다.

### <a name="return-value"></a>반환 값

전환; 성공적으로 만들어졌을 경우 TRUE 그렇지 않으면 FALSE입니다.

##  <a name="m_dblfinalvalue"></a>  CLinearTransition::m_dblFinalValue

전환의 끝에 있는 애니메이션 변수의 값입니다.

```
DOUBLE m_dblFinalValue;
```

##  <a name="m_duration"></a>  CLinearTransition::m_duration

전환 기간입니다.

```
UI_ANIMATION_SECONDS m_duration;
```

## <a name="see-also"></a>참고 항목

[클래스](../../mfc/reference/mfc-classes.md)
