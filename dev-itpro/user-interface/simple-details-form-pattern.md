---
title: Simple Details form pattern | Microsoft Docs
description: This article describes the Simple Details form pattern. This pattern is used when only a simple set of fields must be presented to the user.
author: jasongre
manager: AnnBe
ms.date: 2015-12-03 01:08:23
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.reviewer: annbe
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 14791
ms.assetid: 8823aa29-7b3a-4169-80a4-bf44476aeafc
ms.region: Global
ms.author: jasongre
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: da24f5e2aa5d2d833aec723c7a7c2d1e50f0bf74


---

# <a name="simple-details-form-pattern"></a>Simple Details form pattern

This article describes the Simple Details form pattern. This pattern is used when only a simple set of fields must be presented to the user.

<a name="usage"></a>Usage
-----

The Simple Details pattern is used when only a simple set of fields must be presented to the user. Examples include the display of totals and customer balances. Typically, view mode is used for the Simple Details pattern. However, in cases where the form provides editable information, the edit mode should be synced to the parent form. Four patterns are described in this document:

-   **Simple Details w/Toolbar and Fields** – This is the basic Simple Details pattern, in which several fields are displayed in the form. The fields can optionally appear inside Groups.
-   **Simple Details w/Fast Tabs** – This is the Simple Details pattern that should be used when fields are organized into FastTabs.
-   **Simple Details w/Standard Tabs** – This is the Simple Details pattern that should be used when fields are organized into traditional tabs.
-   **Simple Details w/Panorama** – This is the Simple Details pattern that should be used when information is intended to be displayed in a panorama format.

## <a name="wireframe"></a>Wireframe
[![Wireframe](./media/simpledetails1-1024x578.png)](./media/simpledetails1.png)

## <a name="pattern-changes"></a>Pattern changes
There are no planned changes for the use of this pattern in the current version of Microsoft Dynamics AX.

## <a name="model"></a>Model
### <a name="simple-details-wtoolbar-and-fields--high-level-structure"></a>Simple Details w/Toolbar and Fields – High-level structure

Design

ActionPane (ActionPane)

Body (Group) – **Note:** A field subpattern is used.

### <a name="simple-details-wfasttabs--high-level-structure"></a>Simple Details w/FastTabs – High-level structure

Design

ActionPane (ActionPane)

*HeaderGroup (Group) \[Optional\]*

Body (Tab, Style=FastTabs)

BodyTabPages (TabPage repeats 1..N)

*FooterGroup (Group) \[Optional\]*

### <a name="simple-details-wstandard-tabs--high-level-structure"></a>Simple Details w/Standard Tabs – High-level structure

Design

ActionPane (ActionPane)

*HeaderGroup (Group) \[Optional\]*

Body (Tab, Style=Tabs)

BodyTabPages (TabPage repeats 1..N)

*FooterGroup (Group) \[Optional\]*

### <a name="simple-details-wpanorama--high-level-structure"></a>Simple Details w/Panorama – High-level structure

Design

ActionPane (ActionPane)

Body (Tab, Style=Panorama)

BodyTabPages (TabPage repeats 1..N)

*FooterGroup (Group) \[Optional\]*

### <a name="core-components"></a>Core components

1.  Apply the SimpleDetails pattern on **Form.Design**.
2.  Address BP Warnings:
    1.  **Design.Caption** isn't empty.
    2.  The form must be referenced by at least one menu item.
    3.  **TabPage.Caption** isn't empty.
    4.  MainMenu must not contain menu items that reference a SimpleDetails form.

### <a name="commonly-used-subpatterns"></a>Commonly used subpatterns

-   [Fields and Field Groups](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/fields-and-field-groups-subpattern)
-   [Toolbar and Fields](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/toolbar-and-fields-subpattern)
-   [Tabular Fields](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/tabular-fields-subpattern)
-   [Toolbar and List](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/toolbar-and-list-subpattern)

## <a name="ux-guidelines"></a>UX guidelines
The verification checklist shows the steps for manually verifying that the form complies with UX guidelines. This checklist doesn't include any guidelines that will be enforced automatically through the development environment. Open the form in the browser, and walk through these steps. **Standard form guidelines:**

-   Standard form guidelines have been consolidated into the Dynamics AX [General Form Guidelines](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/user-interface/general-form-guidelines)document.

**Simple Details** **guidelines:**

-   The form page should display a Form Caption that accurately describes the entity.
    -   The Form Caption should be in a singular form.

## <a name="examples"></a>Examples
### <a name="simple-details-wtoolbar-and-fields"></a>Simple Details w/Toolbar and Fields

Form: **AgreementLine** [![Simple Details w/Toolbar and Fields](./media/simpledetails2-1024x688.png)](./media/simpledetails2.png)

### <a name="simple-details-wfasttabs"></a>Simple Details w/FastTabs

Form: **PlanActivityServiceDetails** [![Simple Details w/FastTab](./media/simpledetails3-1024x587.png)](./media/simpledetails3.png)

### <a name="simple-details-wstandard-tabs"></a>Simple Details w/Standard Tabs

Form: **HcmEmploymentDateManager** (Click **Human Resources** &gt; **Common** &gt; **Workers** &gt; **Workers**, click **General** &gt; **Versions** &gt; **Employment History**, and then click **Date Manager**.) [![Simple Details w/Standard Tabs](./media/simpledetails4-1024x588.png)](./media/simpledetails4.png)

### <a name="simple-details-wpanorama"></a>Simple Details w/Panorama

Form: **PdsMRCEventTracker** [![Simple Details w/Panorama](./media/simpledetails5-1024x510.png)](./media/simpledetails5.png)

## <a name="appendix"></a>Appendix
### <a name="frequently-asked-questions"></a>Frequently asked questions

This section will have answers to frequently asked questions that are related to this guideline/pattern.

### <a name="open-issues"></a>Open issues

-   Investigate whether Simple Details forms that show a small amount of related content should have a different presentation than a full-page form.





<!--HONumber=Feb17_HO3-->


