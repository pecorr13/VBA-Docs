---
title: Shape.Height property (Publisher)
keywords: vbapb10.chm2228281
f1_keywords:
- vbapb10.chm2228281
ms.prod: publisher
api_name:
- Publisher.Shape.Height
ms.assetid: 2796ae7e-f4b9-4d79-ff98-d5807286b41e
ms.date: 06/13/2019
ms.localizationpriority: medium
---


# Shape.Height property (Publisher)

Returns or sets a **Variant** that represents the height (in [points](../language/glossary/vbe-glossary.md#point)) of a specified table row or shape. Read/write.


## Syntax

_expression_.**Height**

_expression_ A variable that represents a **[Shape](Publisher.Shape.md)** object.


## Remarks

The valid range for the **Height** property depends on the size of the application workspace and the position of the object within the workspace. 

For centered objects on non-banner page sizes, the **Height** property may be 0.0 to 50.0 inches. For centered objects on banner page sizes, the **Height** property may be 0.0 to 241.0 inches.

[!include[Support and feedback](~/includes/feedback-boilerplate.md)]