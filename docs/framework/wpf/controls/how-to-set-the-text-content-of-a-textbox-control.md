---
title: 'Gewusst wie: Festlegen des Textinhalts eines TextBox-Steuerelements'
ms.date: 03/30/2017
dev_langs:
- csharp
- vb
helpviewer_keywords:
- text content [WPF], setting
- TextBox control [WPF], setting text content
ms.assetid: bcd25fc7-a52f-4453-b802-2c8d2b335ab8
ms.openlocfilehash: 37d636a5e35e9c52ca35ae558b60b5f32d63cabe
ms.sourcegitcommit: 3d5d33f384eeba41b2dff79d096f47ccc8d8f03d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2018
ms.locfileid: "33551725"
---
# <a name="how-to-set-the-text-content-of-a-textbox-control"></a>Gewusst wie: Festlegen des Textinhalts eines TextBox-Steuerelements
Dieses Beispiel zeigt, wie die <xref:System.Windows.Controls.TextBox.Text%2A> den anfänglichen Textinhalt festzulegende Eigenschaft ein <xref:System.Windows.Controls.TextBox> Steuerelement.  
  
 **Hinweis** zwar die [!INCLUDE[TLA#tla_xaml](../../../../includes/tlasharptla-xaml-md.md)] Version des Beispiels können die `<TextBox.Text>` Tags, um den Text der einzelnen Schaltflächen <xref:System.Windows.Controls.TextBox> Inhalt aus, es ist nicht notwendig da die <xref:System.Windows.Controls.TextBox> gilt die <xref:System.Windows.Markup.ContentPropertyAttribute> -Attribut auf die <xref:System.Windows.Controls.TextBox.Text%2A> Eigenschaft. Weitere Informationen finden Sie unter [XAML Overview (WPF)](../../../../docs/framework/wpf/advanced/xaml-overview-wpf.md).  
  
## <a name="example"></a>Beispiel  
 [!code-xaml[TextBox_MiscCode#_TextBoxSetTextXAML](../../../../samples/snippets/csharp/VS_Snippets_Wpf/TextBox_MiscCode/CSharp/Window1.xaml#_textboxsettextxaml)]  
  
## <a name="example"></a>Beispiel  
 [!code-csharp[TextBox_MiscCode#_TextBoxSetText](../../../../samples/snippets/csharp/VS_Snippets_Wpf/TextBox_MiscCode/CSharp/Window1.xaml.cs#_textboxsettext)]
 [!code-vb[TextBox_MiscCode#_TextBoxSetText](../../../../samples/snippets/visualbasic/VS_Snippets_Wpf/TextBox_MiscCode/VisualBasic/Window1.xaml.vb#_textboxsettext)]  
  
## <a name="see-also"></a>Siehe auch  
 [Übersicht über TextBox](../../../../docs/framework/wpf/controls/textbox-overview.md)  
 [Übersicht über RichTextBox](../../../../docs/framework/wpf/controls/richtextbox-overview.md)
