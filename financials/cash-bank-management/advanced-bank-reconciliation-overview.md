---
title: Advanced bank reconciliation overview
description: This article describes the flow for the advanced bank reconciliation process. The advanced bank reconciliation feature lets you import bank statements that can be automatically reconciled from within bank transactions.
author: ShylaThompson
manager: AnnBe
ms.date: 2015-12-11 21 - 23 - 46
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: BankReconciliationMatchRule
audience: Application User
ms.reviewer: ShylaThompson
ms.search.scope: AX 7.0.0, Operations
ms.custom: 22104
ms.assetid: b0705653-1fa6-4d94-9728-bcf9fb387ad1
ms.search.region: Global
ms.author: leguo
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 26b626af83b7fc1ed174a3db271b1a308bf92cbe
ms.lasthandoff: 02/22/2017


---

# <a name="advanced-bank-reconciliation-overview"></a>Advanced bank reconciliation overview

This article describes the flow for the advanced bank reconciliation process. The advanced bank reconciliation feature lets you import bank statements that can be automatically reconciled from within bank transactions.

The advanced bank reconciliation feature lets you import bank statements. The imported bank statement can then be automatically reconciled from within bank transactions. Here are the steps in the advanced bank reconciliation flow.

1.  Set up a bank statement import.
    -   Import bank statements through the data entity framework.
    -   Three typical bank statement formats are built in: ISO20022, BAI2, and MT940.
    -   The functionality can be extended to any format.

2.  Set up a number sequence to use for advanced bank reconciliation, and define the bank reconciliation matching rules.
    -   A reconciliation matching rule is a set of criteria that are used to filter bank statement lines and Microsoft Dynamics 365 for Operations bank transaction lines during the reconciliation process. Depending on your business practice, you can set up more than one matching rule to automate and optimize your reconciliation process.

3.  Reconcile bank statements with Dynamics 365 for Operations bank transactions.
    -   Perform automatic matching and creation of reconciliation journals.
    -   View bank statements and Dynamics 365 for Operations bank transactions side by side.
    -   Automatically post Dynamics 365 for Operations bank transactions if they appear on a bank statement but don't appear in Dynamics 365 for Operations.
    -   Generate a reconciliation statement.




