---
title: '&lt;Code&gt; (Visual Basic)'
ms.date: 07/20/2015
helpviewer_keywords:
- code XML tag
- <code> XML tag
ms.assetid: 925e5342-be05-45f2-bf66-7398bbd6710e
ms.openlocfilehash: 9ec9d23f1f62358dc272f9764f88e3bb2ba41f78
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2018
---
# <a name="ltcodegt-visual-basic"></a>&lt;Code&gt; (Visual Basic)
Gibt an, dass der Text mehrere Codezeilen.  
  
## <a name="syntax"></a>Syntax  
  
```xml  
<code>content</code>  
```  
  
#### <a name="parameters"></a>Parameter  
 `content`  
 Der Text, der als Code zu markieren.  
  
## <a name="remarks"></a>Hinweise  
 Verwenden der `<code>` -Tag, um mehrere Zeilen als Code anzugeben. Mit [\<c>](../../../visual-basic/language-reference/xmldoc/c.md) wird angegeben, dass Text in einer Beschreibung als Code gekennzeichnet werden soll.  
  
 Dokumentationskommentare werden zu einer Datei verarbeitet, indem sie mit [/doc](../../../visual-basic/reference/command-line-compiler/doc.md) kompiliert werden.  
  
## <a name="example"></a>Beispiel  
 Dieses Beispiel verwendet die \<Code >-Tag, um den Beispielcode für die Verwendung der `ID` Feld.  
  
 [!code-vb[VbVbcnXmlDocComments#2](../../../visual-basic/language-reference/xmldoc/codesnippet/VisualBasic/code_1.vb)]  
  
## <a name="see-also"></a>Siehe auch  
 [XML-Kommentartags](../../../visual-basic/language-reference/xmldoc/recommended-xml-tags-for-documentation-comments.md)
