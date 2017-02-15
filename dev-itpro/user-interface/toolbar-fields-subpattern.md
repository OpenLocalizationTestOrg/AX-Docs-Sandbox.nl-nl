---
title: Toolbar and Fields subpattern | Microsoft Docs
description: This article provides information about the Toolbar and Fields subpattern. This container pattern is used to show actions above a subpattern of data fields. The toolbar should contain fewer than 10 actions.
author: jasongre
manager: AnnBe
ms.date: 2015-12-03 21:26:28
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.reviewer: annbe
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 15911
ms.assetid: c8065195-bfd1-4c1c-83be-0038d930868b
ms.region: Global
ms.author: jasongre
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: b0cdd23e56a169fe77d482efd60f8727ed73e9aa


---

# <a name="toolbar-and-fields-subpattern"></a>Toolbar and Fields subpattern

This article provides information about the Toolbar and Fields subpattern. This container pattern is used to show actions above a subpattern of data fields. The toolbar should contain fewer than 10 actions.

<a name="usage"></a>Usage
-----

This container pattern is used to show actions above a subpattern of data fields. The toolbar should contain fewer than 10 actions.

## <a name="wireframe"></a>Wireframe
[![ToolbarFields(1)](./media/toolbarfields1.png)](./media/toolbarfields1.png)

## <a name="model"></a>Model
### <a name="high-level-structure"></a>High-level structure

\[Container\]

Toolbar (ActionPane, Style=Strip)

ContentGroup (Group) – **Note:** A fields subpattern is used.

### <a name="core-components"></a>Core components

-   Apply the ToolbarFields subpattern to the container control.
-   Address BP Warnings:
    -   No additional BP checks are required beyond the AX6.3 BP checks that were carried forward.

### <a name="related-patterns"></a>Related patterns

-   [Toolbar and List](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/toolbar-and-list-subpattern)

### <a name="commonly-used-subpatterns"></a>Commonly used subpatterns

-   [Fields and Field Groups](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/fields-and-field-groups-subpattern)
-   [Tabular Fields](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/tabular-fields-subpattern)
-   [Dimension Expression Builder](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/financial-dimensions/dimension-expression-builder-subpattern)

## <a name="ux-guidelines"></a>UX guidelines
The verification checklist shows the steps for manually verifying that the form complies with UX guidelines. This checklist doesn't include any guidelines that will be enforced automatically through the development environment. Open the form in the browser, and walk through these steps. **Standard form guidelines:**

-   Standard form guidelines have been consolidated into the Microsoft Dynamics AX [General Form Guidelines](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/general-form-guidelines)document.

**Toolbar** **guidelines:**

-   Toolbar guidelines have been consolidated into the Dynamics AX [General Form Guidelines ](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/general-form-guidelines)document.

## <a name="examples"></a>Examples
### <a name="toolbar-and-fields"></a>Toolbar and Fields

Form: **HcmPosition** **(WorkerAssignmentTabPage)** [![ToolbarFields(2)](./media/toolbarfields2-1024x131.png)](./media/toolbarfields2.png)

## <a name="resources"></a>Resources
### <a name="typically-used-by-patterns"></a>Typically used by patterns

-   [Simple List and Details](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/simple-list-and-details-form-pattern)
-   [Table of Contents](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/table-of-contents-form-pattern)
-   [Details Master](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/details-master-form-pattern)
-   [Details Transaction](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/details-transaction-form-pattern)

## <a name="appendix"></a>Appendix
### <a name="frequently-asked-questions"></a>Frequently asked questions

This section will have answers to frequently asked questions that are related to this guideline/pattern.

### <a name="open-issues"></a>Open issues

-   **Should the ShowMoreLess group be part of the pattern, or should it be its own subpattern?**
    -   We will treat the **ShowMoreLess** group as a custom container pattern until there is enough demand to justify the addition of a new pattern.

### <a name="microsoft-dynamics-ax-2012-content"></a>Microsoft Dynamics AX 2012 content

**HcmPosition** ![ToolbarFields(3)](./media/toolbarfields3.png)




<!--HONumber=Feb17_HO3-->


