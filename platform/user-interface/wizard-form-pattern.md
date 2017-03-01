---
title: Wizard form pattern
description: This article provides information about the Wizard form pattern. A wizard is a special form of user assistance that takes the user through a task by using an ordered series of tab pages.
author: jasongre
manager: AnnBe
ms.date: 2015-12-03 00 - 02 - 08
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.reviewer: annbe
ms.search.scope: AX 7.0.0, Operations
ms.custom: 14671
ms.assetid: 564b88d7-85f5-488a-bbbe-19eff7194321
ms.search.region: Global
ms.author: jasongre
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 7be9fc293960bd6b10976cb829cdf661658ec228
ms.lasthandoff: 02/22/2017


---

# <a name="wizard-form-pattern"></a>Wizard form pattern

This article provides information about the Wizard form pattern. A wizard is a special form of user assistance that takes the user through a task by using an ordered series of tab pages.

<a name="usage"></a>Usage
-----

A wizard is a special form of user assistance that takes the user through a task by using an ordered series of tab pages. Wizards are especially useful for complex or infrequent tasks that the user might have difficulty learning or doing, or for tedious, frequently performed tasks.

## <a name="wireframe"></a>Wireframe
[![Wireframe](./media/wizard1-1024x574.png)](./media/wizard1.png)

## <a name="pattern-changes"></a>Pattern changes
Here are the main changes to this pattern since Microsoft Dynamics AX 2012:

-   The secondary instruction for a wizard step was previously defined in the Help Text property of that step’s Tab Page. This instruction will now be modeled on the Tab Page as a Static Text control.

## <a name="model"></a>Model
### <a name="high-level-structure"></a>High-level structure

Design (Style=Wizard; Caption=&lt;wizard title&gt;)

WizardContent (Tab)

WizardContentPage (TabPage) *\[repeats 1..N times, can be named anything; Caption set to page title\]*

MainInstruction (StaticText)

Body (Group)

### <a name="core-components"></a>Core components

1.  Apply the Wizard pattern on **Form.Design**.
2.  Address BP Warnings:
    1.  **Design.Caption** isn't empty.
    2.  The form must be referenced by at least one menu item.
    3.  **TabPage.Caption** isn't empty (for all wizard content pages).
    4.  **MainInstruction.Text** isn't empty (for all wizard content pages).

### <a name="commonly-used-subpatterns"></a>Commonly used subpatterns

-   [Fields and Field Groups](fields-field-groups-subpattern.md)
-   [Toolbar and List](toolbar-list-subpattern.md)
-   [Toolbar and Fields](toolbar-fields-subpattern.md)
-   [List Panel](list-panel-subpattern.md)

## <a name="ux-guidelines"></a>UX guidelines
The verification checklist shows the steps for manually verifying that the form complies with UX guidelines. This checklist doesn't include any guidelines that will be enforced automatically through the development environment. Open the form in the browser, and walk through these steps. **Standard form guidelines:**

-   Standard form guidelines have been consolidated into the Microsoft Dynamics AX [General Form Guidelines](general-form-guidelines.md)document.

**Wizard** **guidelines:**

-   Each tab page should have a title.
-   Each tab page should have a main instruction.
-   Content should be subdivided into logical groups per page.
-   A wizard should have **&lt;Next&gt;** and **&lt;Previous&gt;** buttons on the appropriate pages.
-   The user should also be able to cancel the wizard, and cancellation should return to the state that existed before the wizard was started.
-   Only one question should be asked per wizard page (tab page).
-   When a set of choices is presented to the user, radio buttons should be used to make the alternatives clear, even if a check box or combo box is otherwise acceptable.
-   Wizard forms must **not** have these elements:
    -   FactBoxes
    -   FastTabs

## <a name="examples"></a>Examples
Form: **WrkCtrBulkResReqEditWizard** [![wizardExample](./media/wizardexample.png)](./media/wizardexample.png)[](./media/wizard2.png)

## <a name="appendix"></a>Appendix
### <a name="frequently-asked-questions"></a>Frequently asked questions

This section will have answers to frequently asked questions that are related to this guideline/pattern.

### <a name="open-issues"></a>Open issues

-   None

### <a name="ax-2012-content"></a>AX 2012 content

#### <a name="ax-2012-links"></a>AX 2012 links

-   [MSDN Wizards in Microsoft Dynamics AX \[AX2012\]](http://msdn.microsoft.com/en-us/library/aa622644.aspx)
-   [MSDN Guidelines for Wizard Development \[AX2012\]](http://msdn.microsoft.com/EN-US/library/aa853845.aspx)

#### <a name="ax-2012-example"></a>AX 2012 example

[![AX 2012 example](./media/wizard3.png)](./media/wizard3.png)


