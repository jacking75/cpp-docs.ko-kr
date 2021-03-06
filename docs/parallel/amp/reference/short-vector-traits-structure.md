---
title: short_vector_traits 구조체
ms.date: 11/04/2016
f1_keywords:
- short_vector_traits
- AMP_SHORT_VECTORS/short_vector_traits
- AMP_SHORT_VECTORS/Concurrency::graphics::short_vector_traits::short_vector_traits
- AMP_SHORT_VECTORS/Concurrency::graphics::short_vector_traits::size Constant
ms.assetid: cd9492da-9e02-4a6e-9d50-b61252cdb460
ms.openlocfilehash: fd86228417234f705d3f765624cd942c982df875
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50456188"
---
# <a name="shortvectortraits-structure"></a>short_vector_traits 구조체

short_vector_traits는 기본 벡터 길이 및 짧은 벡터 형식의 스칼라 형식 또는 스칼라 형식 검색할 수 있게 합니다.

## <a name="syntax"></a>구문

```
template<
    typename T
>
struct short_vector_traits;
template<>
struct short_vector_traits<unsigned int>;
template<>
struct short_vector_traits<uint_2>;
template<>
struct short_vector_traits<uint_3>;
template<>
struct short_vector_traits<uint_4>;
template<>
struct short_vector_traits<int>;
template<>
struct short_vector_traits<int_2>;
template<>
struct short_vector_traits<int_3>;
template<>
struct short_vector_traits<int_4>;
template<>
struct short_vector_traits<float>;
template<>
struct short_vector_traits<float_2>;
template<>
struct short_vector_traits<float_3>;
template<>
struct short_vector_traits<float_4>;
template<>
struct short_vector_traits<unorm>;
template<>
struct short_vector_traits<unorm_2>;
template<>
struct short_vector_traits<unorm_3>;
template<>
struct short_vector_traits<unorm_4>;
template<>
struct short_vector_traits<norm>;
template<>
struct short_vector_traits<norm_2>;
template<>
struct short_vector_traits<norm_3>;
template<>
struct short_vector_traits<norm_4>;
template<>
struct short_vector_traits<double>;
template<>
struct short_vector_traits<double_2>;
template<>
struct short_vector_traits<double_3>;
template<>
struct short_vector_traits<double_4>;
```

#### <a name="parameters"></a>매개 변수

`T`

## <a name="members"></a>멤버

### <a name="public-typedefs"></a>공용 Typedefs

|이름|설명|
|----------|-----------------|
|`value_type`||

### <a name="public-constructors"></a>Public 생성자

|이름|설명|
|----------|-----------------|
|[short_vector_traits:: short_vector_traits 생성자](#ctor)||

### <a name="public-constants"></a>공용 상수

|이름|설명|
|----------|-----------------|
|[short_vector_traits:: size 상수](#size)||

## <a name="inheritance-hierarchy"></a>상속 계층

`short_vector_traits`

## <a name="requirements"></a>요구 사항

**헤더:** amp_short_vectors.h

**Namespace:** concurrency:: graphics

##  <a name="ctor"></a>  short_vector_traits:: short_vector_traits 생성자

```
short_vector_traits();
```

##  <a name="size"></a>  short_vector_traits::size Constant

```
static int const size = 1;
```

## <a name="see-also"></a>참고 항목

[Concurrency::graphics 네임스페이스](concurrency-graphics-namespace.md)
