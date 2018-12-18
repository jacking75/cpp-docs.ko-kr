---
title: 구조체 맞춤 예제
ms.date: 11/19/2018
helpviewer_keywords:
- structure alignment
- examples [C++], structure alignment
ms.assetid: 03d137bf-5cc4-472e-9583-6498f2534199
ms.openlocfilehash: 7c4b3ae29674e9c4fc27e8e175867339001b9a0d
ms.sourcegitcommit: 9e891eb17b73d98f9086d9d4bfe9ca50415d9a37
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 11/20/2018
ms.locfileid: "52175342"
---
# <a name="examples-of-structure-alignment"></a>구조체 맞춤 예제

다음 네 개의 예제에서는 각각 정렬된 구조체 또는 공용 구조체를 선언하고 관련된 그림에서는 메모리에 있는 해당 구조체 또는 공용 구조체의 레이아웃을 보여 줍니다. 그림의 각 열은 메모리의 바이트를 나타내고 열의 숫자는 해당 바이트의 치환을 나타냅니다. 각 그림의 두 번째 행에 있는 이름은 선언에 있는 변수의 이름에 해당합니다. 회색으로 표시된 열은 지정된 맞춤을 달성하기 위해 필요한 여백입니다.

## <a name="example-1"></a>예제 1

```C
// Total size = 2 bytes, alignment = 2 bytes (word).

_declspec(align(2)) struct {
    short a;      // +0; size = 2 bytes
}
```

![AMD 변환 예제 1 구조체 레이아웃이](../build/media/vcamd_conv_ex_1_block.png "AMD 변환 예제 1 구조 레이아웃")

## <a name="example-2"></a>예제 2

```C
// Total size = 24 bytes, alignment = 8 bytes (quadword).

_declspec(align(8)) struct {
    int a;       // +0; size = 4 bytes
    double b;    // +8; size = 8 bytes
    short c;     // +16; size = 2 bytes
}
```

![AMD 변환 예제 2 구조체 레이아웃이](../build/media/vcamd_conv_ex_2_block.png "AMD 변환 예제 2 구조 레이아웃")

## <a name="example-3"></a>예제 3

```C
// Total size = 22 bytes, alignment = 4 bytes (doubleword).

_declspec(align(4)) struct {
    char a;       // +0; size = 1 byte
    short b;      // +2; size = 2 bytes
    char c;       // +4; size = 1 byte
    int d;        // +8; size = 4 bytes
}
```

![AMD 변환 예제 2 구조체 레이아웃이](../build/media/vcamd_conv_ex_3_block.png "AMD 변환 예제 2 구조 레이아웃")

## <a name="example-4"></a>예제 4

```C
// Total size = 8 bytes, alignment = 8 bytes (quadword).

_declspec(align(8)) union {
    char *p;      // +0; size = 8 bytes
    short s;      // +0; size = 2 bytes
    long l;       // +0; size = 4 bytes
}
```

![AMD 변환 예제 4에 대 한 공용 구조체 layouit](../build/media/vcamd_conv_ex_4_block.png "AMD 변환 예제 4에 대 한 공용 구조체 layouit")

## <a name="see-also"></a>참고 항목

[형식 및 저장소](../build/types-and-storage.md)<br/>
