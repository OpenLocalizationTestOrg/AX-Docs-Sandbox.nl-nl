---
title: Currency revaluation in a consolidation company
description: 
author: rschloma
manager: AnnBe
ms.date: 2016-03-08 17 - 49 - 53
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations
ms.custom: 62183
ms.assetid: 2762baaf-0c10-4ff7-8713-c506d6c29b98
ms.search.region: Global
ms.author: hminzner
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: c8db360ea2b7ab3ba35ef0fb9e0d380645202316
ms.lasthandoff: 02/22/2017


---

# <a name="currency-revaluation-in-a-consolidation-company"></a>Currency revaluation in a consolidation company



When you consolidate data from one accounting currency to another, you must still run currency revaluation if there is a change in exchange rates, so that your account balances  are correctly revalued. When you originally consolidate the data, use the **Currency translation** tab to select the initial exchange rates to for translation during the consolidation process. After a new exchange rate is entered (for example, in the next month), you must revalue the account balances. The unrealized gains or losses are then updated accordingly, based on the new exchange rate and date. The following example illustrates the accounting entries that are created during the process.

## <a name="company-setup"></a>Company setup
-   **Source/operating company (USMF)** – US dollars (USD) are used as the accounting and reporting currency.
-   **Consolidated company (CON)** – Euros (EUR) are used as the accounting and reporting currency.
    -   **Realized gain **– Ledger account 801500
    -   **Realized loss** – Ledger account 801600
    -   **Unrealized gain** – Ledger account 801600
    -   **Unrealized loss** – Ledger account 801400

## <a name="original-transactions"></a>Original transactions
### <a name="cash-receipt-transactions-in-usmf"></a>Cash receipt transactions in USMF

| Date       | Ledger account               | Currency | Amount |
|------------|------------------------------|----------|--------|
| 10/11/2015 | 110110 – Cash                | USD      | 500    |
| 10/11/2015 | 130100 – Accounts Receivable | USD      | -500   |

## <a name="exchange-rates"></a>Exchange rates
| From currency | To currency | Start date | Exchange rate |
|---------------|-------------|------------|---------------|
| EUR           | USD         | 10/1/2015  | 200           |
| EUR           | USD         | 11/1/2015  | 150           |
| EUR           | USD         | 12/1/2012  | 100           |

## <a name="perform-the-consolidation-for-october-2015"></a>Perform the consolidation for October 2015
### <a name="balances-in-the-consolidation-company"></a>Balances in the consolidation company

| Ledger account | Currency | Amount | Calculation    |
|----------------|----------|--------|----------------|
| 110110         | EUR      | 250    | 500 USD × 50%  |
| 130100         | EUR      | -250   | -500 USD × 50% |

## <a name="perform-currency-revaluation-for-the-accounts-from-october-1-2015-through-november-30-2015"></a>Perform currency revaluation for the accounts from October 1, 2015, through November 30, 2015
### <a name="balances-in-the-consolidation-company"></a>Balances in the consolidation company

| Ledger account | Currency | Amount  | Calculation                        |
|----------------|----------|---------|------------------------------------|
| 110110         | EUR      | 333.33  | Original amount of 500 × 66.6667%  |
| 130100         | EUR      | -333.33 | Original amount of -500 × 66.6667% |
| 801400         | EUR      | 83.33   | 333.33 – 250                       |
| 801600         | EUR      | -83.33  | -333.33 – (-250)                   |

You will see additional transactions for the reporting currency amounts.

## <a name="perform-currency-revaluation-for-the-accounts-from-october-1-2015-through-december-31-2015"></a>Perform currency revaluation for the accounts from October 1, 2015, through December 31, 2015
### <a name="balances-in-the-consolidation-company"></a>Balances in the consolidation company

| Ledger account | Currency | Amount  | Calculation                                          |
|----------------|----------|---------|------------------------------------------------------|
| 110110         | EUR      | 500.00  | Original amount of 500 × 1                           |
| 130100         | EUR      | -500.00 | Original amount of -500 × 1                          |
| 801400         | EUR      | 250     | 500 – 333.33 = 166.67 166.67 + 83.33 = 250           |
| 801600         | EUR      | -250    | -500 – (-333.33) = -166.67 -166.67 + (-83.33) = -250 |




