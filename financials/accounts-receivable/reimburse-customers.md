---
title: Reimburse customers
description: This article explains how to create reimbursement transactions for a group of customers. If a customer has a credit balance, you can reimburse the customer for the amount of the balance.
author: twheeloc
manager: AnnBe
ms.date: 2015-12-02 23 - 14 - 54
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: LedgerJournalTransCustPaym, LedgerJournalTransVendPaym
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: AX 7.0.0, Operations
ms.custom: 14191
ms.assetid: 53533ee3-470e-458a-ac8b-3815aa4cb502
ms.search.region: Global
ms.author: kweekley
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: befc42e3cf2e961cb3e20465282590ceb0a1d6e5
ms.lasthandoff: 02/22/2017


---

# <a name="reimburse-customers"></a>Reimburse customers

This article explains how to create reimbursement transactions for a group of customers. If a customer has a credit balance, you can reimburse the customer for the amount of the balance. 

The following table shows the prerequisites that must be in place before you start.

| Prerequisite                                                            | Description                                                                                                                                                                                 |
|-------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Specify the minimum reimbursement amount for the legal entity.          | On the **Accounts receivable parameters** page, in the **General** area, in the **Minimum reimbursement** field, enter the minimum amount that can be reimbursed for customer overpayments. |
| Optional: Add a vendor account to each customer that can be reimbursed. | On the **Customers** page, on the **Miscellaneous details** FastTab, in the **Vendor account** field, select the vendor account for the customer.                                           |

When you create reimbursement transactions, a vendor invoice is created for the amount of the credit balance. The reimbursement process removes the credit balance for the customer account and creates a balance due for the vendor account that corresponds to the customer.

1.  In Accounts receivable, run the **Reimbursement** process.
2.  Follow one of these steps:
    -   To reimburse specific customer accounts, click **Select**, and specify the customer accounts in the query.
    -   To reimburse all customer accounts, click **OK**.

    The credit amounts are transferred to the vendor accounts of the customers and are processed as ordinary payments. If a customer doesn't have a vendor account, a one-time vendor account is automatically created for the customer.
3.  To view the reimbursement transactions that were created, use the **Reimbursement** page.
4.  In Accounts payable, create a payment for the vendor invoices that were created by the reimbursement process.



