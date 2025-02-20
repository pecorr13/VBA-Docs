---
title: TextBox.Text property (Access)
keywords: vbaac10.chm11106
f1_keywords:
- vbaac10.chm11106
ms.prod: access
api_name:
- Access.TextBox.Text
ms.assetid: bb510c65-6d0d-468a-c5be-f325d86c2c7f
ms.date: 03/02/2019
ms.localizationpriority: medium
---


# TextBox.Text property (Access)

Use the **Text** property to set or return the text **Value** contained in a text box. Read/write **String**.


## Syntax

_expression_.**Text**

_expression_ A variable that represents a **[TextBox](Access.TextBox.md)** object.


## Remarks

You can set the **Text** property to the text that you want to display in the control. You can also use the **Text** property to read the text currently in the control.

> [!NOTE] 
> To set or return a control's **Text** property, the control must have the focus, or an error occurs. To move the focus to a control, you can use the **SetFocus** method or GoToControl action.

While the control has the focus, the **Text** property contains the text data currently in the control; the **Value** property contains the last saved data for the control. When you move the focus to another control, the control's data is updated, and the **Value** property is set to this new value. The **Text** property setting is then unavailable until the control gets the focus again. If you use the **Save Record** command on the **Records** menu to save the data in the control without moving the focus, the **Text** property and **Value** property settings will be the same.


## Example

The following example uses the **Text** property to enable a **Next** button named **btnNext** whenever the user enters text into a text box named **txtName**. Anytime the text box is empty, the **Next** button is disabled.

```vb
Sub txtName_Change() 
 btnNext.Enabled = Len(Me!txtName.Text & "")<>0 
End Sub
```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]
