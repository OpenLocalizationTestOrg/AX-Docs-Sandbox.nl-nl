---
title: Tabular Fields subpattern | Microsoft Docs
description: This article provides information about the Tabular Fields subpattern. This subpattern is used to show information efficiently in a tabular format.
author: jasongre
manager: AnnBe
ms.date: 2015-12-03 00:51:07
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.reviewer: annbe
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 14761
ms.assetid: 358fa6af-9272-4853-96a1-ef82bb4ed2c1
ms.region: Global
ms.author: jasongre
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: 3695249a45de1575e7f797e9ea6640d45f6aff5f


---

# <a name="tabular-fields-subpattern"></a>Tabular Fields subpattern

This article provides information about the Tabular Fields subpattern. This subpattern is used to show information efficiently in a tabular format. 

<a name="usage"></a>Usage
-----

This subpattern is used to show information efficiently in a tabular format. The fields are arranged in a table that contains rows and columns, and that optionally contains column headers, row labels, a caption, and a footer. The Tabular Fields subpattern can be applied on the following controls:

-   TabPage control
-   Group control

## <a name="wireframes"></a>Wireframes
### <a name="tabularfields1mediatabularfields1pngmediatabularfields1pngstructural-wireframe"></a>[![TabularFields(1)](./media/tabularfields1.png)](./media/tabularfields1.png)Structural wireframe

[![TabularFields(2)](./media/tabularfields2.png)](./media/tabularfields2.png)

## <a name="pattern-changes"></a>Pattern changes
In previous releases of Microsoft Dynamics AX, there was no formally accepted way to model this pattern. Therefore, this pattern was modeled in many inconsistent ways that must be modified to match the current pattern. The most common way to model this pattern was to use groups for columns. However, groups are now used for the rows. The primary reason for this change was to better match the HTML/CSS constructs, and it also helps keep the tab sequence and semantics of a table.

## <a name="model"></a>Model
### <a name="high-level-structure"></a>High-level structure

TabularFields (Group\*)

CaptionGroup (Group)

*TableCaption (StaticText) \[Optional\]*

TableHeaderRow (Group)

*Column0Label (StaticText) \[Optional\]* – **Note:** This static text fills col0, row0 with a blank.

ColumnLabels (StaticText) \[1..N\] – **Note:** These are the normal column headers.

TableRows (Group) \[1..N\]

*RowLabel (StaticText) \[Optional\]*

RowValues ($Field) \[1..N\] OR SecondaryColumnLabel (StaticText) \[1..N\]

TableFooterGroup (Group)

*Column0Label (StaticText) \[Optional\]* – **Note:** This static text fills col0, footer with a blank.

*RowValues ($Field) \[0..N\]* – **Note:** All the footer fields are in view mode.

Note that the four groups in the top-level tabular fields are mandatory structural elements. However, the contents of all those groups exception the Rows (Group) are optional. Additionally, note that Tabular Fields can also be used on a TabPage control. The structure is the same as the structure that is shown here.

### <a name="core-components"></a>Core components

Apply the Tabular Fields pattern on the top-level group or tab page. Address the pattern errors and problems.

## <a name="ux-guidelines"></a>UX guidelines
No manual verification is required.

## <a name="examples"></a>Examples
Form: **LedgerJournalTransVendPaym** **(Balances)** (**Accounts payable** &gt; **Journals** &gt; **Payment journal** &gt; **Lines**) [![TabularFields(3)](./media/tabularfields3.png)](./media/tabularfields3.png)

## <a name="resources"></a>Resources
### <a name="typically-used-by-patterns"></a>Typically used by patterns

-   [Simple List and Details](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/simple-list-and-details-form-pattern)
-   [Table of Contents](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/table-of-contents-form-pattern)
-   [Details Master](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/details-master-form-pattern)
-   [Details Transaction](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/details-transaction-form-pattern)

## <a name="appendix"></a>Appendix
### <a name="frequently-asked-questions"></a>Frequently asked questions

This section will have answers to frequently asked questions that are related to this guideline/pattern.

-   **Why are we changing how the tabular field layout is created?**
    -   To accomplish the layout in HTML, we must align with the way that HTML layout works. HTML layout groups by rows, not by columns.

### <a name="open-issues"></a>Open issues

-   None





<!--HONumber=Feb17_HO3-->


