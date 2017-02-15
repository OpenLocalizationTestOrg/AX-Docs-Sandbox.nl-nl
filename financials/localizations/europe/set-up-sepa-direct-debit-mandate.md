---
title: Set up SEPA direct debit mandate | Microsoft Docs
description: 
author: twheeloc
manager: AnnBe
ms.date: 2016-03-07 21:16:37
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.reviewer: 101
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 59491
ms.assetid: ba45f59d-db66-409d-ae4f-51cd1fdc87f6
ms.region: Global
ms.author: mfalkner
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: f509d3c197cfdcb1548e26219fa0960dc376c011


---

# <a name="set-up-sepa-direct-debit-mandate"></a>Set up SEPA direct debit mandate



A Single Euro Payment Area (SEPA) direct debit lets a creditor collect funds from a customer's bank account, provided that the customer has granted a signed mandate to the creditor. The mandate that the customer signs authorizes the creditor to collect a payment and instructs the customer's bank to pay the collection. The following illustration shows the process for setting up SEPA direct debit mandates. The numbers correspond to the procedures later in this topic. ![Set up process for SEPA direct debit mandates](https://i-technet.sec.s-msft.com/dynimg/IC677310.gif "Set up process for SEPA direct debit mandates")

## <a name="prerequisites"></a>Prerequisites
The following table shows the prerequisites that must be in place before you start.

| Category       | Prerequisite                                                                                                                                              |
|----------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| Country/region | The primary address for the legal entity must be in the following countries/regions: Austria, Belgium, Germany, Spain, France, Italy, or the Netherlands. |

## <a name="1-set-up-a-number-sequence-for-direct-debit-mandates"></a>1. Set up a number sequence for direct debit mandates
Each direct debit mandate must have a unique number. Use the **Number sequences** page to create a number sequence for direct debit mandates. You will use this identifier to assign the number sequence to the direct debit mandate system on the **Accounts receivable parameters** page.

## <a name="2-set-up-accounts-receivable-parameters-for-direct-debit-mandates"></a>2. Set up Accounts receivable parameters for direct debit mandates
Use the **Accounts receivable parameters** page to set up parameters for direct debit mandates. To set up the parameters, on the **Direct debit** tab, change the default parameters as you require. Then, on the **Number sequences** tab, update the **Direct debit mandate ID** field with the number sequence that you set up earlier.

## <a name="3-set-up-a-method-of-payment-for-direct-debit-mandates"></a>3. Set up a method of payment for direct debit mandates
You must set up a method of payment for direct debit mandates. You use this method of payment to query for invoices to generate direct debit payments for. Use the **Methods of payment** page to set up the method of payment. To set up a method of payment for direct debit mandates, you must follow these additional steps for a method of payment:

-   In the **Payment type** field, select **Electronic payment**.
-   Optional: If you expect each of your customers to have multiple mandates, in the **Period** field, select **Invoice**. A separate payment will be created for each invoice, and each payment will use the mandate that is specified for the invoice.
-   Select the **Require mandate** option to create payments by using direct debit mandates. The **Require mandate** option is available only if you select **Electronic payment** in the **Payment type** field.





<!--HONumber=Feb17_HO3-->


