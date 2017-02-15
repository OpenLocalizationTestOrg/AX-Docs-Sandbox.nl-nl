---
title: Create a budget from transaction accounts and total accounts | Microsoft Docs
description: This article provides an overview of the process for creating budgets based on total accounts. It also explains how to turn on budget control for total accounts, if budget control is required.
author: twheeloc
manager: AnnBe
ms.date: 2015-12-01 16:44:37
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
keywords: BudgetControlConfiguration, BudgetPlanGenerate
audience: Application User
ms.reviewer: twheeloc
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 13051
ms.assetid: 8e93ced2-1d8c-4630-8fe0-7eb635731d86
ms.region: Global
ms.author: sigitac
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: fdf82ae1c7b7a18c1e46473ef7a1ceb5714f39da


---

# <a name="create-a-budget-from-transaction-accounts-and-total-accounts"></a>Create a budget from transaction accounts and total accounts

This article provides an overview of the process for creating budgets based on total accounts. It also explains how to turn on budget control for total accounts, if budget control is required.

Both budget plan and budget register entry documents allow for budgeting on main accounts that have a main account type of **Total**. Actuals can be posted only to transactional main accounts. For the **Generate budget plan from General ledger** periodic process, on the **Source** tab, you can specify the **Total** main account type as a criterion. In this case, each total main account will be included in the target budget plan, and the amount will equal the total amount of the range of selected main accounts. You can activate budget control for main accounts of the **Total** type. This functionality is supported through the use of budget groups. For each total main account, the budget that should be controlled for a budget group must be created on the **Budget control configuration **page. The criteria that you specify must include the total main account and the range of accounts. To speed up the process of creating budget groups, you can take advantage of the Budget control groups data entity. When a budget is used in reporting, such as on a financial statement, the budget sum for the total account consists of the following amounts:

-   The budgets that are created from each transaction ledger account in the interval of the total account.
-   The budget amount that is entered directly on the total account.

Therefore, you can create separate budgets for the most significant transaction accounts in the interval of the total account, and then add the available budget amount to the total account.




<!--HONumber=Feb17_HO3-->


