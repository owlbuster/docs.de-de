---
title: IN (Entity SQL)
ms.date: 03/30/2017
ms.assetid: 51662950-ee01-4857-b7b9-311dd8515966
ms.openlocfilehash: 1f3be5717c27a691e073cee46df757d0166fe78a
ms.sourcegitcommit: 11f11ca6cefe555972b3a5c99729d1a7523d8f50
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/03/2018
ms.locfileid: "32761700"
---
# <a name="in-entity-sql"></a>IN (Entity SQL)
Bestimmt, ob ein Wert mit irgendeinem Wert in einer Auflistung übereinstimmt.  
  
## <a name="syntax"></a>Syntax  
  
```  
value [ NOT ] IN expression  
```  
  
## <a name="arguments"></a>Argumente  
 `value`  
 Jeder gültige Ausdruck, der den auf Übereinstimmung zu prüfenden Wert zurückgibt.  
  
 [ NOT ]  
 Legt fest, dass das `Boolean`-Ergebnis von IN negiert werden soll.  
  
 `expression`  
 Jeder gültige Ausdruck, der die auf Übereinstimmung zu prüfende Auflistung zurückgibt. Alle Ausdrücke müssen vom selben Typ oder vom gleichen Basistyp bzw. abgeleiteten Typ sein wie `value`.  
  
## <a name="return-value"></a>Rückgabewert  
 `true`, wenn der Wert in der Auflistung gefunden wurde, null, wenn der Wert oder die Auflistung NULL ist, anderenfalls `false`. Mit NOT IN wird das Ergebnis von IN negiert.  
  
## <a name="example"></a>Beispiel  
 Die folgende Entity SQL-Abfrage verwendet den IN-Operator, um zu bestimmen, ob ein Wert mit irgendeinem Wert in einer Auflistung übereinstimmt. Diese Abfrage beruht auf dem "AdventureWorks Sales"-Modell. Führen Sie folgende Schritte aus, um diese Abfrage zu kompilieren und auszuführen:  
  
1.  Verwenden Sie das Verfahren unter [How to: Execute a Query that Returns StructuralType Results](../../../../../../docs/framework/data/adonet/ef/how-to-execute-a-query-that-returns-structuraltype-results.md).  
  
2.  Übergeben Sie die folgende Abfrage als Argument an die `ExecuteStructuralTypeQuery` -Methode:  
  
 [!code-csharp[DP EntityServices Concepts 2#IN](../../../../../../samples/snippets/csharp/VS_Snippets_Data/dp entityservices concepts 2/cs/entitysql.cs#in)]  
  
## <a name="see-also"></a>Siehe auch  
 [Entity SQL-Referenz](../../../../../../docs/framework/data/adonet/ef/language-reference/entity-sql-reference.md)
