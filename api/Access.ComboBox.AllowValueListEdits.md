---
title: ComboBox.AllowValueListEdits property (Access)
keywords: vbaac10.chm11517
f1_keywords:
- vbaac10.chm11517
ms.prod: access
api_name:
- Access.ComboBox.AllowValueListEdits
ms.assetid: 558ba7aa-b3b2-4fe8-7338-8e9fbef19159
ms.date: 02/28/2019
ms.localizationpriority: medium
---


# ComboBox.AllowValueListEdits property (Access)

Gets or sets whether the **Edit List Items** command is available when the user right-clicks a combo box. Read/write **Boolean**.


## Syntax

_expression_.**AllowValueEditLists**

_expression_ A variable that represents a **[ComboBox](Access.ComboBox.md)** object.


## Remarks

The **AllowValueEditLists** property determines whether the **Edit List Items** command is available when the user right-clicks a combo box that's bound to a **Lookup** field.

If the **Lookup** field is bound to a list of values, the **Edit List Items** dialog box is displayed when the user chooses **Edit List Items**. The user can then add, delete, or edit the items to be displayed in the combo box.

If the **Lookup** field is bound to a table or query, the form specified by the **ListItemsEditForm** property is displayed when the user clicks **Edit List Items**. The user can use the form to add, delete, or edit the items to be displayed in the combo box.

The **AllowValueEditLists** property is not available for combo boxes on a report.




[!include[Support and feedback](~/includes/feedback-boilerplate.md)]