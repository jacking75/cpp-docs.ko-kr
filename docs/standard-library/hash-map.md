---
title: '&lt;hash_map&gt;'
ms.date: 01/18/2018
f1_keywords:
- <hash_map>
- std::<hash_map>
helpviewer_keywords:
- hash_map header
ms.openlocfilehash: 5a7ea891a314d69b8bc3378edce9fa0de2d89ace
ms.sourcegitcommit: afd6fac7c519dbc47a4befaece14a919d4e0a8a2
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/10/2018
ms.locfileid: "51520324"
---
# <a name="lthashmapgt"></a>&lt;hash_map&gt;

> [!NOTE]
> 이 헤더는 사용되지 않습니다. 대신 [ \<unordered_map >](unordered-map.md)합니다.

컨테이너 템플릿 클래스 hash_map 및 hash_multimap과 지원 템플릿을 정의합니다.

## <a name="syntax"></a>구문

```
#include <hash_map>
```

### <a name="operators"></a>연산자

|Hash_map 버전|Hash_multimap 버전|설명|
|-----------------------|----------------------------|-----------------|
|[operator!=(hash_map)](hash-map-operators.md#op_neq)|[operator!=(hash_multimap)](hash-map-operators.md#op_neq_mm)|연산자의 좌변에 있는 hash_map 또는 hash_multimap 개체가 우변에 있는 hash_map 또는 hash_multimap 개체와 같지 않은지 테스트합니다.|
|[operator==(hash_map)](hash-map-operators.md#op_eq_eq)|[operator==(hash_multimap)](hash-map-operators.md#op_eq_eq_mm)|연산자의 좌변에 있는 hash_map 또는 hash_multimap 개체가 우변에 있는 hash_map 또는 hash_multimap 개체와 같은지 테스트합니다.|

### <a name="specialized-template-functions"></a>특별 템플릿 함수

|Hash_map 버전|Hash_multimap 버전|설명|
|-----------------------|----------------------------|-----------------|
|[swap(hash_map)](hash-map-class.md#swap)|[swap(hash_multimap)](hash-multimap-class.md#swap)|두 hash_map 또는 hash_multimap의 요소를 교환합니다.|

### <a name="classes"></a>클래스

|클래스|설명|
|-|-|
|[hash_compare 클래스](hash-compare-class.md)|해시 연관 컨테이너에서 사용할 수 있는 개체를 설명-hash_map, hash_multimap, hash_set 또는 hash_multiset-기본값으로 `Traits` 를 주문 하 고 포함 된 요소의 해시 매개 변수 개체입니다.|
|[value_compare 클래스](value-compare-class.md)|키 값 비교를 통해 hash_map의 요소를 비교하여 hash_map 내의 상대 순서를 확인할 수 있는 함수 개체를 제공합니다.|
|[hash_map 클래스](hash-map-class.md)|각 요소가 값이 고유하고 연결된 데이터 값인 정렬 키가 있는 쌍인 컬렉션에서 데이터를 신속하게 저장하고 검색하는 데 사용됩니다.|
|[hash_multimap 클래스](hash-multimap-class.md)|각 요소가 값이 고유하고 연결된 데이터 값이 아니어도 되는 정렬 키가 있는 쌍인 컬렉션에서 데이터를 신속하게 저장하고 검색합니다.|

## <a name="requirements"></a>요구 사항

**헤더:** \<hash_map>

**네임스페이스:** stdext

## <a name="see-also"></a>참고자료

[헤더 파일 참조](cpp-standard-library-header-files.md)<br/>
[C++ 표준 라이브러리의 스레드 보안](thread-safety-in-the-cpp-standard-library.md)<br/>
[C++ 표준 라이브러리 참조](cpp-standard-library-reference.md)
