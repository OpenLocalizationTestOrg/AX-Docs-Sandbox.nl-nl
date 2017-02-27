---
title: Bank statement and payment reconciliation overview for the EU
description: This topic provides an overview of the functionality that you can use to reconcile payment information from banks in formats that are used by European countries.
author: ShylaThompson
manager: AnnBe
ms.date: 2017-01-23 22 - 06 - 44
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: BankAccountTable, CustPaymMode, VendPaymMode
audience: Application User
ms.search.scope: Operations
ms.custom: 267994
ms.assetid: 2bfb8ecc-e850-43cb-9a96-deb11716a391
ms.search.region: Belgium, Norway, Sweden, Switzerland
ms.author: v-lenest
ms.dyn365.ops.intro: 01-11-2016
ms.dyn365.ops.version: Version 1611
translationtype: Human Translation
ms.sourcegitcommit: a4efe875c495e7747566a77ba62b0dad741b15c5
ms.openlocfilehash: d6e321bee6aad874204c717ec3e13d83cb0307c9
ms.lasthandoff: 02/22/2017


---

# <a name="bank-statement-and-payment-reconciliation-overview-for-the-eu"></a>Bank statement and payment reconciliation overview for the EU

This topic provides an overview of the functionality that you can use to reconcile payment information from banks in formats that are used by European countries.

In Microsoft Dynamics 365 for Operations, you can import transactions from banks and settle these transactions against existing transactions. In Europe, you can do this for the following scenarios:

-   Importing bank statements
-   Importing payments.
-   Importing return files.

## <a name="bank-statements"></a>Bank statements
A *bank statement* or *account statement* is a summary of financial transactions that have occurred over a given period on a bank account held by a company with a financial institution. In Dynamics 365 for Operations you can import a bank statement. It is important to settle imported transactions with existing transactions as well as verify the opening and ending balance of the bank accounts. The following list includes the supported European formats.

-   Advanced bank reconciliation European file formats. For more information, see [Advanced bank reconciliation overview](advanced-bank-reconciliation-overview.md).
-   ISO 20022 camt.053 bank statement message file format
-   CODA bank statement file format. For more information, see [CODA bank statement](bel-coda-bank-statement-import.md).

## <a name="customer-and-vendor-payments-import-and-return-messages"></a>Customer and vendor payments import and return messages
In addition to a bank statement, banks can provide specific messages, containing information about customer and vendor payments, which can be imported into Dynamics 365 for Operations and reconciled with customer and vendor transactions. When a company needs to receive information about incoming customer payments transactions from the bank, the import formats can be used. For companies that use direct debit and credit transfer, the return messages can be received to update the status of payments that were previously exported. The difference between import formats and return formats is that returns are targeted mostly to update already created payment journal lines (they can be created when direct debit or credit transfer were initiated) instead of creating new lines. Some complex import formats can also include return scenarios. The following example shows how this division should be implemented.

##### <a name="import-formats"></a>Import formats

-   ISO 20022 camt.054 bank notification message
-   [Nets import format](nor-nets-import-format.md) - Complex feature for Norwegian payment formats
-   ESR customer payments import
-   Import payment formats for Sweden - BankGirot Max and BankGirot OCR formats

##### <a name="return-formats"></a>Return formats

-   ISO 20022 pain.002 payment status report
-   (DNK) BetalingsserviceBasis-returformat – Return format for customer Betalingsservice export format
-   [Import payment formats for Sweden](sweden-payment-formats-import.md) - Bankgirot Autogiro returns
-   (SWE) BankGirot return – Vendor payments return format, which corresponds to Bankgirot export format



