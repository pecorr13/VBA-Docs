---
title: ChartBorder.Weight property (PowerPoint)
keywords: vbapp10.chm685004
f1_keywords:
- vbapp10.chm685004
ms.prod: powerpoint
api_name:
- PowerPoint.ChartBorder.Weight
ms.assetid: 71750026-1df0-1a1b-bb43-b0c6891d66be
ms.date: 06/08/2017
ms.localizationpriority: medium
---


# ChartBorder.Weight property (PowerPoint)

Returns or sets the weight of the border. Read/write **[XlBorderWeight](PowerPoint.XlBorderWeight.md)**.


## Syntax

_expression_.**Weight**

_expression_ A variable that represents a '[ChartBorder](PowerPoint.ChartBorder.md)' object.


## Example




> [!NOTE] 
> Although the following code applies to Microsoft Word, you can readily modify it to apply to PowerPoint.

The following example sets the border weight for the value axis of the first chart in the active document to medium.




```vb
With ActiveDocument.InlineShapes(1)

    If .HasChart Then

        .Chart.Axes(xlValue).Border.Weight = xlMedium

    End If

End With
```


## See also


[ChartBorder Object](PowerPoint.ChartBorder.md)

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]