---
title: Section.OnRetreat property (Access)
keywords: vbaac10.chm12206,vbaac10.chm4105
f1_keywords:
- vbaac10.chm12206,vbaac10.chm4105
ms.prod: access
api_name:
- Access.Section.OnRetreat
ms.assetid: 0da552f0-72bc-3886-2708-a8c4180f4903
ms.date: 03/23/2019
ms.localizationpriority: medium
---


# Section.OnRetreat property (Access)

Sets or returns the value of the **On Retreat** box in the Properties window of a report section. Read/write **String**.


## Syntax

_expression_.**OnRetreat**

_expression_ A variable that represents a **[Section](Access.Section.md)** object.


## Remarks

This property is helpful for programmatically changing the action that Microsoft Access takes when an event is triggered. For example, between event calls you may want to change an expression's parameters, or switch from an event procedure to an expression or macro, depending on the circumstances under which the event was triggered. 

The **Retreat** event occurs when Access returns to a previous report section during report formatting.

The **OnRetreat** value will be one of the following, depending on the selection chosen in the Choose Builder window (accessed by choosing the **Build** button next to the **On Retreat** box in the report section's Properties window):

- If you choose Expression Builder, the value will be =_expression_, where _expression_ is the expression from the Expression Builder window.
    
- If you choose Macro Builder, the value is the name of the macro. 
    
- If you choose Code Builder, the value will be [Event Procedure]. 
    
If the **On Retreat** box is blank, the property value is an empty string.


## Example

The following example prints the value of the **OnRetreat** property in the Immediate window for the "GroupHeader0" section in the **Purchase Order** report.

```vb
Debug.Print Reports("Purchase Order").Section("GroupHeader0").OnRetreat
```



[!include[Support and feedback](~/includes/feedback-boilerplate.md)]