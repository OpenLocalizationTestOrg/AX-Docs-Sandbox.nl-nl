---
title: Take a discount that is more than the calculated discount for a vendor payment | Microsoft Docs
description: This article walks you through a scenario where a cash discount is taken for an amount that is more than the discount that was originally available on the invoice. This scenario might occur if an organization comes to an agreement with the vendor to pay a smaller amount on the invoice.
author: twheeloc
manager: AnnBe
ms.date: 2015-12-02 23:20:58
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
keywords: LedgerJournalTransVendPaym, VendOpenTrans
audience: Application User
ms.reviewer: twheeloc
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 14281
ms.assetid: ece69f0e-e1b9-4064-9015-d01b51db7ee7
ms.region: Global
ms.author: kweekley
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: c8855b5341ea6bd0d03029bdd20aff39469f94e0


---

# <a name="take-a-discount-that-is-more-than-the-calculated-discount-for-a-vendor-payment"></a>Take a discount that is more than the calculated discount for a vendor payment

This article walks you through a scenario where a cash discount is taken for an amount that is more than the discount that was originally available on the invoice. This scenario might occur if an organization comes to an agreement with the vendor to pay a smaller amount on the invoice. 

Vendor 3051 gives Fabrikam a cash discount of 4 percent if an invoice is paid in seven days. On June 29, April enters an invoice for 1,000.00. The vendor lets April take a discount of 60.00 instead of the default discount of 40.00 that is available for the invoice. April records a one-off payment by using the Accounts payable payment journal. She enters the vendor for the payment and then opens the **Settle transactions** page. She marks the invoice and changes the value in the **Cash discount amount** field to **60.00**.
| Mark     | Use cash discount | Voucher   | Account | Date      | Due date  | Invoice | Amount in transaction currency | Currency | Amount to settle |
|----------|-------------------|-----------|---------|-----------|-----------|---------|--------------------------------|----------|------------------|
| Selected | Normal            | Inv-10040 | 3051    | 6/29/2015 | 7/29/2015 | 10040   | 1,000.00                       | USD      | 940.00           |

Discount information appears at the bottom of the **Settle transactions** page.
|                              |           |
|------------------------------|-----------|
| Cash discount date           | 7/12/2015 |
| Cash discount amount         | 60.00     |
| Use cash discount            | Normal    |
| Cash discount taken          | 0.00      |
| Cash discount amount to take | 60.00     |

April posts the payment journal. The invoice is fully settled by using a payment of 940.00 and a discount of 60.00.




<!--HONumber=Feb17_HO3-->


