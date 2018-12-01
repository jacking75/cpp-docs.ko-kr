---
title: Microsoft 확장명
ms.date: 11/04/2016
helpviewer_keywords:
- Microsoft extensions to C/C++
ms.assetid: 68654516-24ef-4f33-aae2-175f86cc1979
ms.openlocfilehash: d8104c2df2335e11dcb711108d566e0fdd069762
ms.sourcegitcommit: 6052185696adca270bc9bdbec45a626dd89cdcdd
ms.translationtype: MT
ms.contentlocale: ko-KR
ms.lasthandoff: 10/31/2018
ms.locfileid: "50592207"
---
# <a name="microsoft-extensions"></a>Microsoft 확장명

*asm-statement*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;**__asm** assembly-instruction; <sub>opt  </sub><br/>
&nbsp;&nbsp;&nbsp;&nbsp;**__asm** { assembly-instruction-list }; <sub>opt    </sub>

*assembly-instruction-list*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;*assembly-instruction* **;** <sub>opt</sub> <br/>
&nbsp;&nbsp;&nbsp;&nbsp;*assembly-instruction* **;** *assembly-instruction-list* **;** <sub>opt</sub>

*ms-modifier-list*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;*ms-modifier ms-modifier-list*<sub>opt</sub>

*ms-modifier*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;**__cdecl**<br/>
&nbsp;&nbsp;&nbsp;&nbsp;**__fastcall**<br/>
&nbsp;&nbsp;&nbsp;&nbsp;**__stdcall**<br/>
&nbsp;&nbsp;&nbsp;&nbsp;**__syscall** (이후 구현을 위해 예약 되어 있음)<br/>
&nbsp;&nbsp;&nbsp;&nbsp;**__oldcall** (이후 구현을 위해 예약 되어 있음)<br/>
&nbsp;&nbsp;&nbsp;&nbsp;**__unaligned** (이후 구현을 위해 예약 되어 있음)<br/>
&nbsp;&nbsp;&nbsp;&nbsp;*based-modifier*

*based-modifier*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;**__based (** *based-type* **)**

*based-type*:<br/>
&nbsp;&nbsp;&nbsp;&nbsp;*name*
