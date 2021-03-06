---
title: Verwendung von TransactedReceiveScope
ms.date: 03/30/2017
ms.assetid: d455f1dc-bfc5-43d6-8ae9-bc3b3a3ea08a
ms.openlocfilehash: 635235504a08a151053026cf25c68750dc335eef
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2018
ms.locfileid: "33517305"
---
# <a name="use-of-transactedreceivescope"></a>Verwendung von TransactedReceiveScope
Dieses Beispiel veranschaulicht, wie eine Transaktion mit <xref:System.Activities.Statements.TransactionScope> von einem Client auf einen Server übertragen wird, um eine neue Transaktion auf dem Client und ein <xref:System.ServiceModel.Activities.TransactedReceiveScope>-Element zu erstellen, sodass eine Meldung mit einem Transaktionsfluss empfangen und die Lebensdauer der Transaktion auf dem Server mit einem Bereich versehen werden kann. Das Beispiel besteht aus zwei Projekten, die in den Rollen des Clients und des Server fungieren.  
  
## <a name="client-application"></a>Clientanwendung  
 Die Clientanwendung führt einen Workflow aus, der die verteilte Transaktions-ID ausgibt, eine Meldung an den Server sendet, die Transaktion übertragt, die Antwort empfängt, die verteilte Transaktions-ID erneut ausgibt und den Vorgang dann abschließt. Wenn die verteilte Transaktions-ID zu Beginn Daten ausgibt, handelt es sich um eine leere GUID, da die Transaktion nach wie vor lokal ist.  
  
## <a name="server-application"></a>Serveranwendung  
 Das Serverprojekt verhält sich ähnlich, der Workflow wird jedoch in <xref:System.ServiceModel.Activities.WorkflowServiceHost> gehostet, da ein Endpunkt auf die Meldung des Clients hin überwacht werden muss. Der Workflow basiert auf dem <xref:System.ServiceModel.Activities.TransactedReceiveScope>, der die übertragene Transaktion vom Client empfängt, die gesendete Meldung ausgibt, die verteilte Transaktions-ID ausgibt und die Antwort an den Client sendet. Die verteilte Transaktions-ID ist jetzt eine nicht leere GUID, und wenn dem Text des <xref:System.ServiceModel.Activities.TransactedReceiveScope> eine Aktivität hinzugefügt wurde, die Transaktionen verarbeiten kann, würde dieser unter der übertragenen Transaktion ausgeführt werden.  
  
#### <a name="to-run-the-sample"></a>So führen Sie das Beispiel aus  
  
1.  Öffnen Sie die Projektmappe "TransactedReceiveScope.sln" in [!INCLUDE[vs2010](../../../../includes/vs2010-md.md)].  
  
2.  Um die Projektmappe zu erstellen, drücken Sie STRG + UMSCHALT + B, oder wählen Sie **Projektmappe** aus der **erstellen** Menü.  
  
3.  Sobald die Erstellung erfolgreich war, mit der rechten Maustaste in der Projektmappe, und wählen Sie **Startprojekte festlegen**. Wählen Sie im Dialogfeld **mehrere Startprojekte** und sicherzustellen, dass die Aktion für beide Projekte **starten**.  
  
4.  Drücken Sie F5, oder wählen Sie **Debuggen** aus der **Debuggen** Menü. Alternativ können Sie STRG + F5 oder wählen Sie **Starten ohne Debugging** aus der **Debuggen** -Menü, um ohne Debuggen auszuführen.  
  
    > [!NOTE]
    >  Der Server muss vor dem Starten des Clients ausgeführt werden. Die Ausgabe im Konsolenfenster, das den Dienst hostet, gibt an, wenn dieser gestartet wird.  
  
> [!IMPORTANT]
>  Die Beispiele sind möglicherweise bereits auf dem Computer installiert. Suchen Sie nach dem folgenden Verzeichnis (Standardverzeichnis), bevor Sie fortfahren.  
>   
>  `<InstallDrive>:\WF_WCF_Samples`  
>   
>  Wenn dieses Verzeichnis nicht vorhanden ist, fahren Sie mit [Windows Communication Foundation (WCF) und Windows Workflow Foundation (WF) Samples for .NET Framework 4](http://go.microsoft.com/fwlink/?LinkId=150780) aller Windows Communication Foundation (WCF) herunterladen und [!INCLUDE[wf1](../../../../includes/wf1-md.md)] Beispiele. Dieses Beispiel befindet sich im folgenden Verzeichnis.  
>   
>  `<InstallDrive>:\WF_WCF_Samples\WF\Basic\Transactions\TransactedReceiveScope`