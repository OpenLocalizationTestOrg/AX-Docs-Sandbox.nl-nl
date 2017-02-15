---
title: List Page form pattern | Microsoft Docs
description: This article provides information about the List Page form pattern. A list page presents a set of data on a UI that is optimized for browsing records, so that you can find and work with a specific record.
author: jasongre
manager: AnnBe
ms.date: 2015-12-02 23:17:39
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.reviewer: annbe
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 14241
ms.assetid: 6e2f73aa-d239-4ad3-9a8e-554897bb64c5
ms.region: Global
ms.author: jasongre
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: 010f2c095ac370dbad57a5db0bade970f199c64c


---

# <a name="list-page-form-pattern"></a>List Page form pattern

This article provides information about the List Page form pattern. A list page presents a set of data on a UI that is optimized for browsing records, so that you can find and work with a specific record. 

<a name="usage"></a>Usage
-----

A list page presents a set of data on a user interface that is optimized so that you can browse records, find the right record, and then take an action upon that record. The list page lets the user search, filter, and sort the data. FactBoxes on the right side of the grid show related data for the active record. Actions that are relevant to the record are located on the ActionPane at the top of the page. In the current version of Microsoft Dynamics AX, use of this pattern is discouraged when there is a 1:1 correspondence between the List Page and Details page. Current guidance is to use this pattern only in other situations, such as when list pages have no backing details pages or have multiple backing details page (for example, when project quotations and sales quotations are shown together in the same List Page).

## <a name="wireframe"></a>Wireframe
[![Wireframe](./media/listpage1-1024x576.png)](./media/listpage1.png)

## <a name="pattern-changes"></a>Pattern changes
Here are the main changes to this pattern since Microsoft Dynamics AX 2012:

-   FormTemplate/InteractionClass is now optional when you build new pages.
-   List Page and Details Master/Details Transaction are merged into a single form when there is a 1:1 correspondence between the List Page and Details Page.
    -   Improves performance when the user moves between the list and details.
    -   Allows for bulk editing in the initial list.
-   The **Preview** pane has been eliminated.

## <a name="model"></a>Model
### <a name="high-level-structure"></a>High-level structure

Design

ActionPane (ActionPane)

Custom Filter (Group)

Quick Filter (Quick Filter)

*OtherFilters ($Field) \[0..N\]*

Grid (Grid)

### <a name="core-components"></a>Core components

1.  Apply the ListPage pattern on **Form.Design**.
2.  Address BP Warnings:
    1.  **Design.Caption** isn't empty.
    2.  The form must be referenced by at least one menu item.
    3.  **TabPage.Caption** isn't empty.
    4.  **TabPage.DataSource** isn't empty.
    5.  The primary data source has **AllowEdit**=**No**, **AllowCreate**=**No**, and **AllowDelete**=**Yes**.
    6.  **Grid.DefaultAction** references the button that opens the child form.
    7.  **Grid.DefaultLabelAction** references a label to show in the grid context menu.

### <a name="related-patterns"></a>Related patterns

-   [Details Master](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/details-master-form-pattern)
-   [Details Transaction](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/details-transaction-form-pattern)
-   [Simple List](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/simple-list-form-pattern)

### <a name="commonly-used-subpatterns"></a>Commonly used subpatterns

-   [Custom Filter Group](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/custom-filter-group-subpattern)

## <a name="ux-guidelines"></a>UX guidelines
The verification checklist shows the steps for manually verifying that the form complies with UX guidelines. This checklist doesn't include any guidelines that will be enforced automatically through the development environment. Open the form in the browser, and walk through these steps. **Standard form guidelines:**

-   Standard form guidelines have been consolidated into the Microsoft Dynamics AX [General Form Guidelines](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/general-form-guidelines)document.

**List Page guidelines:**

-   Have fewer than 15 fields in the grid.
-   The first textual/data column should be displayed as a link that goes to the appropriate details form. To do this, make sure that the grid has a default action to enable the hyperlink for the first column.
-   A Quick Filter should appear above the list. By default, the QuickFilter should use the most likely field for a filter scenario.
-   There should not be any duplicate **New** and **Delete** buttons.
-   A link to the List page should be provided in the Main Menu.
-   Focus should be in the Quick Filter when the list page is opened.
-   **Page title area**:
    -   The page title should be in a plural form.
    -   For primary list pages, the title should be the name of the entity.
    -   For secondary list pages, the title should reflect an activity or status.
-   **Grid**:
    -   For transactional entities, the **ID** field should be the first column, followed by the master entity **ID** and **Name** fields.
    -   For master entities, the **Name** field should be the first column, followed by the **ID** field.
-   **ActionPane** guidelines have been consolidated into the Dynamics AX [General Form Guidelines ](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/general-form-guidelines)document in the ActionPane guidelines section.
-   **FactBox** guidelines have been consolidated into the [FactBox Form Patterns](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/factbox-form-patterns)document.

## <a name="examples"></a>Examples
Form: **SalesTableListPage** [![List Page example](./media/listpage2-1024x510.png)](./media/listpage2.png)

## <a name="appendix"></a>Appendix
### <a name="frequently-asked-questions"></a>Frequently asked questions

This section will have answers to frequently asked questions that are related to this guideline/pattern.

-   **What do I do with the Preview pane when I migrate the form?** You can do one of the following:
    -   Remove the **Preview** pane altogether if it no longer makes sense.
    -   Remove the large header, and leave the **Preview** pane as is.
    -   Split the **Preview** pane into multiple logical FactBoxes if the current one is too tall.
        -   For a transaction preview, the lines would go into their own FactBox and should be limited to five lines.
        -   For a transaction preview, rework the lines into a FactBox card pattern, where the lines are summarized into a count and a lines grid is shown in an enhanced preview when the user hovers over the count value.

### <a name="open-issues"></a>Open issues

-   **How to handle secondary list pages**
    -   Stay in navigation (no app changes needed).
    -   Create role-tailored views (after future framework support is added).

### <a name="ax-2012-content"></a>AX 2012 content

#### <a name="ax-2012-links"></a>AX 2012 links

-   [MSDN AX2012 List Page User Experience Guidelines](http://msdn.microsoft.com/EN-US/library/gg853328.aspx)
-   [MSDN AX2012 List Page Forms](http://msdn.microsoft.com/en-us/library/cc635077.aspx)

#### <a name="ax-2012-example"></a>AX 2012 example

[![AX 2012 example](./media/listpage3-1024x671.png)](./media/listpage3.png)




<!--HONumber=Feb17_HO3-->


