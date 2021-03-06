---
title: Korrelierter Rechner
ms.date: 03/30/2017
ms.assetid: c365166e-6552-49a4-bf17-9f4e597d4d41
ms.openlocfilehash: 77e13b3ca913d2432cfe5d4a95e83764effbb109
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2018
ms.locfileid: "33514140"
---
# <a name="correlated-calculator"></a>Korrelierter Rechner
In diesem Beispiel wird veranschaulicht, wie die Messagingaktivitäten (<xref:System.ServiceModel.Activities.Receive> und <xref:System.ServiceModel.Activities.SendReply>) im Designer auf Grundlage eines Parameters in der Meldung mit inhaltsbasierter Korrelation verwendet werden. In diesem Szenario befinden sich die Vorgänge des Rechners in einem parallelen Konvoi. Sowohl eine Instanz als auch eine Korrelation (basierend auf `CalculatorId`) werden erstellt, wenn die erste Meldung an den Workflow gesendet wird; nachfolgende Meldungen mit derselben `CalculatorId` werden an diese Instanz weitergeleitet, bis der Reset-Vorgang aufgerufen wird. Der Client wird als WPF-Anwendung implementiert, die einen codebasierten Clientproxy verwendet, um mit dem Dienst zu kommunizieren.  
  
#### <a name="to-use-this-sample"></a>So verwenden Sie dieses Beispiel  
  
1.  Starten Sie [!INCLUDE[vs2010](../../../../includes/vs2010-md.md)] mit erhöhten Rechten, und öffnen Sie die Projektmappendatei "For.sln".  
  
    1.  Navigieren Sie zu dem Ordner, der [!INCLUDE[vs2010](../../../../includes/vs2010-md.md)] enthält.  
  
    2.  Mit der rechten Maustaste Devenv.exe aus, und wählen Sie **als Administrator ausführen**.  
  
2.  Öffnen Sie die Projektmappendatei " CorrelatedCalculator.sln" in [!INCLUDE[vs2010](../../../../includes/vs2010-md.md)].  
  
3.  Drücken Sie STRG+UMSCHALT+B, um die Projektmappe zu erstellen.  
  
4.  Drücken Sie STRG+F5, um das Dienstprojekt auszuführen.  
  
5.  Sobald der Dienst bereit ist und Nachrichten überwacht, klicken Sie im Projektmappen-Explorer mit der rechten Maustaste auf das Clientprojekt, und führen Sie es aus.  
  
> [!IMPORTANT]
>  Die Beispiele sind möglicherweise bereits auf dem Computer installiert. Suchen Sie nach dem folgenden Verzeichnis (Standardverzeichnis), bevor Sie fortfahren.  
>   
>  `<InstallDrive>:\WF_WCF_Samples`  
>   
>  Wenn dieses Verzeichnis nicht vorhanden ist, fahren Sie mit [Windows Communication Foundation (WCF) und Windows Workflow Foundation (WF) Samples for .NET Framework 4](http://go.microsoft.com/fwlink/?LinkId=150780) aller Windows Communication Foundation (WCF) herunterladen und [!INCLUDE[wf1](../../../../includes/wf1-md.md)] Beispiele. Dieses Beispiel befindet sich im folgenden Verzeichnis.  
>   
>  `<InstallDrive>:\WF_WCF_Samples\WF\Scenario\Services\CorellatedCalculator`