---
title: OneWayBindingElement
ms.date: 03/30/2017
ms.assetid: 5c7e17c3-39b9-4214-ae08-9e6141734305
ms.openlocfilehash: ee7cfed20234175ba54dd25dbbbab4615c1ed7af
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2018
ms.locfileid: "33485744"
---
# <a name="onewaybindingelement"></a>OneWayBindingElement
OneWayBindingElement  
  
## <a name="syntax"></a>Syntax  
  
```  
class OneWayBindingElement : BindingElement  
{  
  ChannelPoolSettings ChannelPoolSettings;  
  sint32 MaxAcceptedChannels;  
  boolean PacketRoutable;  
};  
```  
  
## <a name="methods"></a>Methoden  
 Die Klasse OneWayBindingElement definiert keine Methoden.  
  
## <a name="properties"></a>Eigenschaften  
 Die Klasse OneWayBindingElement verfügt über die folgenden Eigenschaften:  
  
### <a name="channelpoolsettings"></a>ChannelPoolSettings  
 Datentyp: ChannelPoolSettings  
  
 Zugriffstyp: Schreibgeschützt  
  
 Die Kanalpool-Einstellungen.  
  
### <a name="maxacceptedchannels"></a>MaxAcceptedChannels  
 Datentyp: sint32  
  
 Zugriffstyp: Schreibgeschützt  
  
 Die maximale Anzahl von akzeptierten Kanälen.  
  
### <a name="packetroutable"></a>PacketRoutable  
 Datentyp: Boolesch  
  
 Zugriffstyp: Schreibgeschützt  
  
 Ein Wert, der angibt, ob das Paket geroutet werden kann.  
  
## <a name="requirements"></a>Anforderungen  
  
|MOF|Deklariert in Servicemodel.mof.|  
|---------|-----------------------------------|  
|Namespace|Definiert in root\ServiceModel|  
  
## <a name="see-also"></a>Siehe auch  
 <xref:System.ServiceModel.Channels.OneWayBindingElement>
