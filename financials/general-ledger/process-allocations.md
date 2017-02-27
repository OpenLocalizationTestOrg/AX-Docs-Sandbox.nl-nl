---
title: Process allocations
description: This article provides information about allocations, the options for processing them in Microsoft Dynamics 365 for Operations, and how they can be used in budget planning. Allocations are used to distribute amounts across multiple ledger account combinations. They help guarantee that expenses or revenue is charged to the correct object in accounting.
author: twheeloc
manager: AnnBe
ms.date: 2015-12-04 18 - 16 - 59
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: AccountingDistribution, LedgerAllocationRule, MainAccount
audience: Application User
ms.reviewer: annbe
ms.search.scope: AX 7.0.0, Operations
ms.custom: 17361
ms.assetid: 04c8548a-0af9-492b-954b-946b4f8ca023
ms.search.region: Global
ms.author: peakerbl
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: da75ab9b9cf439feec5410ce266aa84b9593690c
ms.lasthandoff: 02/22/2017


---

# <a name="process-allocations"></a>Process allocations

This article provides information about allocations, the options for processing them in Microsoft Dynamics 365 for Operations, and how they can be used in budget planning. Allocations are used to distribute amounts across multiple ledger account combinations. They help guarantee that expenses or revenue is charged to the correct object in accounting.

Microsoft Dynamics 365 for Operations provides the following capabilities to support this process:

-   Manually allocate transaction amounts by using the Split action in accounting distributions, or by applying financial dimension default templates to a document. For more information, see [Accounting distributions.](accounting-distributions.md)
-   Automatically allocate transactions amounts based on allocation terms defined on individual main account. Allocation account entries will be generated for each journal based on the percentage and destination ledger account whenever an accounting entry meets the criteria defined as the source ledger account.
-   Automatically allocate ledger balances or fixed amounts based on ledger allocation rules. The ledger allocation rules are processed on a periodic basis using allocation journals. For more information, see [Ledger allocation rules](http://ax.help.dynamics.com/en/wiki/about-allocation-rules/).

###  <a name="allocations-in-budget-planning"></a>Allocations in budget planning

Ledger allocation rules can be used for budget plans. When you use ledger allocation rules in budget planning, the allocation rules work the same way they would in the ledger, but the source data and destination data comes from the budget plan. You can manually select ledger allocation rules to use for budget plans. Alternatively, you can use an allocation schedule that runs as part of a workflow process.

|                                                                         |
|-------------------------------------------------------------------------|
| **Note**                                                                |
| You can’t use intercompany ledger allocation rules for budget planning. |




