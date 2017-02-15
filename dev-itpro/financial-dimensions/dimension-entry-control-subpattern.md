---
title: Dimension entry control subpattern | Microsoft Docs
description: This article provides information about the Dimension Entry Control subpattern. This subpattern is used when you have a group or tab page that uses the Dimension Entry control (DEC).
author: jasongre
manager: AnnBe
ms.date: 2015-12-03 21:38:48
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.reviewer: annbe
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 15951
ms.assetid: d5c4ae07-3f5c-4165-a934-66a46d989a54
ms.region: Global
ms.author: jasongre
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: 5895b007b0f147d75cad152ea9c1ea2e9cf894ed


---

# <a name="dimension-entry-control-subpattern"></a>Dimension entry control subpattern

This article provides information about the Dimension Entry Control subpattern. This subpattern is used when you have a group or tab page that uses the Dimension Entry control (DEC). 

<a name="usage"></a>Usage
-----

The Dimension Entry Control pattern is used when you have a group or tab page that uses the Dimension Entry control (DEC).

## <a name="wireframe"></a>Wireframe
[![decWireframe](./media/decwireframe.png)](./media/decwireframe.png)  

## <a name="model"></a>Model
### <a name="high-level-structure"></a>High-level structure

TabPage | Group *TopFieldGroup (Group) \[Optional\]* – **Note:** A field subpattern is used. *DECGroup (Group) \[0..N\]* Dimension Entry Control *Dimension Entry Control \[0..N\]* *BottomFieldGroup (Group) \[Optional\]* – **Note:** A field subpattern is used.

### <a name="core-components"></a>Core components

-   Apply the Dimension Entry Control subpattern to the TabPage control.

## <a name="ux-guidelines"></a>UX guidelines
None.

## <a name="examples"></a>Examples
Form: **CustTable (TabFinancialDimensions)** [![decExample](./media/decexample.png)](./media/decexample.png)    

## <a name="appendix"></a>Appendix
### <a name="frequently-asked-questions"></a>Frequently asked questions

This section will have answers to frequently asked questions that are related to this guideline/pattern.

### <a name="open-issues"></a>Open issues

None.




<!--HONumber=Feb17_HO3-->


