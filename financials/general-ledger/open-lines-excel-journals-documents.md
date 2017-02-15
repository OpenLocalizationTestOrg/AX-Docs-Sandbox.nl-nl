---
title: Publish journal lines and documents from Excel | Microsoft Docs
description: This topic explains how to enter and publish lines for general journals from Microsoft Excel. It includes information about the various templates that you can use, depending on the type of transactions that you&quot;re entering.
author: twheeloc
manager: AnnBe
ms.date: 2016-03-08 17:50:05
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
keywords: LedgerJournalTable
audience: Application User
ms.reviewer: 101
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 62213
ms.assetid: 6da33290-c6b4-49ea-aa5d-92af929e3e3b
ms.region: Global
ms.author: kweekley
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: bc4962661e578fcb45d7025f8518a59dc76b30af


---

# <a name="publish-journal-lines-and-documents-from-excel"></a>Publish journal lines and documents from Excel

This topic explains how to enter and publish lines for general journals from Microsoft Excel. It includes information about the various templates that you can use, depending on the type of transactions that you're entering.

Users can enter and publish lines for financial journals from Microsoft Excel. After a user creates a journal, the **Open lines in Excel** button displays the templates that are available. Templates are designed to support specific scenarios, however not every combination of account type is supported in the journal. The following table shows the templates that are available and the account types which they support.
|                          |                                                                                                                         |                                                                                         |
|--------------------------|-------------------------------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------|
| **Template**             | **Supported account types**                                                                                             | **How to access the template**                                                          |
| Ledger journal lines     | Account: Ledger, Customer, Vendor, Bank Offset account: Ledger, Customer, Vendor, Bank Intercompany is supported.       | General journal                                                                         |
| Invoice register         | Account: Vendor Offset account: Ledger Intercompany isn't supported.                                                    | AP invoice register                                                                     |
| Invoice journal          | Accounts: Vendor Offset account: Ledger Intercompany is supported.                                                      | AP invoice journal                                                                      |
| Vendor invoice           |                                                                                                                         | Vendor invoice                                                                          |
| Customer invoice journal | Account: Customer Offset account: Ledger Intercompany is supported.                                                     | General journal                                                                         |
| Free text invoice        |                                                                                                                         | On the **Free text invoice** page, click **Open in Excel** (the Microsoft Office icon). |
| Fixed assets journal     | Asset to ledger, bank, customer, or vendor. Intercompany isn't supported.                                               | Fixed asset journal                                                                     |
| Vendor payment journal   | Account: Vendor Offset account: Ledger, Bank Intercompany is supported.                                                 | Vendor payment journal                                                                  |
| Customer payment journal | Account: Customer Offset account: Ledger, Bank Intercompany is supported.                                               | Customer payment journal                                                                |
| Project expense journal  | Account: Project, Ledger, Customer, Vendor Offset account: Project, Ledger, Customer, Vendor Intercompany is supported. | General journal Expense (under Project management and accounting)                       |

When the lines are published, they are validated to make sure that they comply with the rules that are set up in the financial journals. After the lines are published, users can edit or post the vouchers from Microsoft Dynamics 365 for Operations. To add financial dimensions to a template, additional changes are required. For additional information, see [Add dimensions to the Microsoft Excel template](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/financial-dimensions/dimensions-overview). After dimensions are added to the entity, they are available in the Excel designer and can be added to the template.

<a name="see-also"></a>See also
--------

[Dimensions in Excel](https://docs.microsoft.com/en-us/dynamics365/operations/dev-itpro/financial-dimensions/dimensions-overview)




<!--HONumber=Feb17_HO3-->


