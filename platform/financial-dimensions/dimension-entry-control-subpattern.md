---
title: Dimension entry control subpattern
description: This article provides information about the Dimension Entry Control subpattern. This subpattern is used when you have a group or tab page that uses the Dimension Entry control (DEC).
author: jasongre
manager: AnnBe
ms.date: 2015-12-03 21 - 38 - 48
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.reviewer: annbe
ms.search.scope: AX 7.0.0, Operations
ms.custom: 15951
ms.assetid: 6baee22e-2a86-428c-b9e2-178581c57830
ms.search.region: Global
ms.author: jasongre
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 57c837c4aaa2a12b406e30b21b3f33d99fdeb7fa
ms.lasthandoff: 02/22/2017


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


