---
title: 연산자 Windows::UI::Xaml::Interop::TypeName
ms.date: 12/30/2016
ms.assetid: a65a105e-7e3a-452f-932f-2cdaf00fbba5
ms.openlocfilehash: c77655ed7692c4cdccc311bc27c492126d62e54e
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50659215"
---
# <a name="operator-windowsuixamlinteroptypename"></a>연산자 Windows::UI::Xaml::Interop::TypeName

`Platform::Type` 을 [Windows::UI::Xaml::Interop::TypeName](https://msdn.microsoft.com/library/windows/apps/windows.ui.xaml.interop.typename.aspx)으로 변환할 수 있습니다.

## <a name="syntax"></a>구문

```cpp
Operator TypeName(Platform::Type^ type);
```

### <a name="return-value"></a>반환 값

[이 제공되면](https://msdn.microsoft.com/library/windows/apps/windows.ui.xaml.interop.typename.aspx) Windows::UI::Xaml::Interop::TypeName `Platform::Type^`을 반환합니다.

### <a name="remarks"></a>설명

`TypeName` 은 형식 정보를 나타내기 위한 언어 중립 Windows 런타임 구조체입니다. [Platform::Type](../cppcx/platform-type-class.md) 은 C++에서만 사용되며 ABI(응용 프로그램 이진 인터페이스) 전반에서 전달될 수 없습니다. 다음은 `TypeName`Navigate [함수에서](https://msdn.microsoft.com/library/windows/apps/hh702394.aspx) 을 사용하는 한 가지 방법입니다.

```
rootFrame->Navigate(TypeName(MainPage::typeid), e->Arguments);
```

### <a name="example"></a>예제

다음 예제에서는 `TypeName` 과 `Type`간을 변환하는 방법을 보여 줍니다.

```

// Convert from Type to TypeName
Windows::UI::Xaml::Interop::TypeName tn = TypeName(MainPage::typeid);

// Convert back from TypeName to Type
Type^ tx2 = (Type^)(tn);
```

## <a name="net-framework-equivalent"></a>.NET Framework의 해당 값

.NET Framework는 `TypeName` 프로젝트를 [System.Type](assetId:///System.Type?qualifyHint=False&autoUpgrade=True)으로 변환할 수 있습니다.

### <a name="requirements"></a>요구 사항

## <a name="see-also"></a>참고 항목

[연산자 Windows::UI::Xaml::Interop::TypeName](../cppcx/operator-windows-ui-xaml-interop-typename.md)<br/>
[Platform::Type 클래스](../cppcx/platform-type-class.md)