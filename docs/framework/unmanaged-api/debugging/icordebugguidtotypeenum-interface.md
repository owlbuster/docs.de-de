---
title: ICorDebugGuidToTypeEnum-Schnittstelle
ms.custom: 
ms.date: 03/30/2017
ms.prod: .net-framework
ms.reviewer: 
ms.suite: 
ms.technology: dotnet-clr
ms.tgt_pltfrm: 
ms.topic: reference
api_name: ICorDebugGuidToTypeEnum
api_location: mscordbi.dll
api_type: COM
f1_keywords: ICorDebugGuidToTypeEnum
helpviewer_keywords: ICorDebugGuidToTypeEnum interface [.NET Framework debugging]
ms.assetid: aa32b12b-05fc-4ea8-a904-adae25034269
topic_type: apiref
caps.latest.revision: "6"
author: rpetrusha
ms.author: ronpet
manager: wpickett
ms.openlocfilehash: e419c61d2918a1f17c0739c9782472f25dfe8cfa
ms.sourcegitcommit: bd1ef61f4bb794b25383d3d72e71041a5ced172e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/18/2017
---
# <a name="icordebugguidtotypeenum-interface"></a>ICorDebugGuidToTypeEnum-Schnittstelle
Stellt einen Enumerator, der definiert die Zuordnung zwischen einem Satz von GUIDs und die zugehörigen Typen, die von Instanzen ICorDebugType dargestellt werden. Diese Schnittstelle erbt die Methoden von ICorDebugEnum-Schnittstelle.  
  
## <a name="methods"></a>Methoden  
  
|Methode|Beschreibung|  
|------------|-----------------|  
|[Icordebugguidtotypeenum:: Next](../../../../docs/framework/unmanaged-api/debugging/icordebugguidtotypeenum-next-method.md)|Ruft die angegebene Anzahl von [CorDebugGuidToTypeMapping](../../../../docs/framework/unmanaged-api/debugging/cordebugguidtotypemapping-structure.md) Instanzen, die GUIDs für die Typinformationen zugeordnet.|  
  
## <a name="remarks"></a>Hinweise  
 Ein `ICorDebugGuidToTypeEnum` -Schnittstellenobjekt abgerufen werden kann, durch Aufrufen der [icordebugappdomain3:: Getcachedwinrttypes](../../../../docs/framework/unmanaged-api/debugging/icordebugappdomain3-getcachedwinrttypes-method.md) Methode. Ein Debugger kann diese Schnittstelle aufrufen [Weiter](../../../../docs/framework/unmanaged-api/debugging/icordebugguidtotypeenum-next-method.md) -Methode abrufen [CorDebugGuidToTypeMapping](../../../../docs/framework/unmanaged-api/debugging/cordebugguidtotypemapping-structure.md) verwalteten Darstellungen von Objekten, die Zuordnungen von darstellen [!INCLUDE[wrt](../../../../includes/wrt-md.md)] geladene Typen der die Anwendungsdomäne für den Aufruf von verwendet die [icordebugappdomain3:: Getcachedwinrttypes](../../../../docs/framework/unmanaged-api/debugging/icordebugappdomain3-getcachedwinrttypes-method.md) Methode.  
  
## <a name="requirements"></a>Anforderungen  
 **Plattformen:**[!INCLUDE[wrt](../../../../includes/wrt-md.md)]  
  
 **Header:** CorDebug.idl, CorDebug.h  
  
 **Bibliothek:** CorGuids.lib  
  
 **.NET Framework-Versionen:**[!INCLUDE[net_current_v45plus](../../../../includes/net-current-v45plus-md.md)]  
  
## <a name="see-also"></a>Siehe auch  
 [Debugschnittstellen](../../../../docs/framework/unmanaged-api/debugging/debugging-interfaces.md)