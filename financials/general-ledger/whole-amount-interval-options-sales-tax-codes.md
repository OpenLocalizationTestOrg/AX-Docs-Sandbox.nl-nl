---
title: Whole amount and Interval calculation options for sales tax codes
description: This article explains the options for the Calculation method field on sales tax codes and how sales tax is calculated for intervals and whole amounts.
author: ShylaThompson
manager: AnnBe
ms.date: 2015-09-14 09 - 43 - 08
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: TaxData, TaxTable
audience: Application User
ms.reviewer: ShylaThompson
ms.search.scope: AX 7.0.0, Operations
ms.custom: 5624
ms.assetid: 96166db4-b7ca-470b-aeb7-0a66fe0554c4
ms.search.region: Global
ms.author: vstehman
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 76615fb7407a1bf2729c319d23c29962a8d1f2da
ms.lasthandoff: 02/22/2017


---

# <a name="whole-amount-and-interval-calculation-options-for-sales-tax-codes"></a>Whole amount and Interval calculation options for sales tax codes

This article explains the options for the Calculation method field on sales tax codes and how sales tax is calculated for intervals and whole amounts.

You can set up a sales tax code to be calculated based on a whole amount or an interval amount. In the Sales tax codes page, use the Calculation method field on the Calculation FastTab to select how to calculate a sales tax code.
-   Whole amount – The tax rate is applied to the whole taxable amount.
-   Interval – The taxable amount is divided into parts, each of which falls in a range that has a specific sales tax rate. The part of the amount that falls in a given interval is taxed according to the tax rate for that interval. The sales tax is the sum of the tax amounts that are calculated for each amount interval.
    | **Note**                                                                                                                                                |
    |---------------------------------------------------------------------------------------------------------------------------------------------------------|
    | The Interval option is available only when you select Line in the Calculation method field in the Sales tax area of the General ledger parameters page. |

Intervals are set up in the Sales tax code values page by entering Minimum and Maximum limit amounts per tax rate. For taxes to be calculated on all taxable amounts, regardless of which calculation method is selected, intervals must follow these rules:
-   The first interval must have a Minimum limit of zero.
-   The last interval must have a Maximum limit of zero, which indicates infinity.
-   The Maximum limit of an interval must be the Minimum limit of the next interval.

If an amount is the Maximum limit of the previous interval and the Minimum limit of the next interval, the sales tax rate of the first interval will be applied to the amount. If an amount falls outside the intervals that are defined by upper and lower limits, a sales tax rate of zero will be applied.

## <a name="example-whole-amount-method-of-calculation"></a>Example: Whole amount method of calculation
In the Sales tax code values page, sales tax rates are set up in the following intervals:
|                   |                   |              |
|-------------------|-------------------|--------------|
| **Minimum limit** | **Maximum limit** | **Tax rate** |
| 0.00              | 50.00             | 30%          |
| 50.00             | 100.00            | 20%          |
| 100.00            | 0.00              | 10%          |

The sales tax is calculated on the whole taxable amount.

| Taxable amount (price) | Calculation    | Sales tax |
|------------------------|----------------|-----------|
| 35.00                  | 35.00 \* 0.30  | 10.50     |
| 50.00                  | 50.00 \* 0.30  | 15.00     |
| 85.00                  | 85.00 \* 0.20  | 17.00     |
| 305.00                 | 305.00 \* 0.10 | 30.50     |

## <a name="example-interval-method-of-calculation"></a>Example: Interval method of calculation
In the Values page, sales tax rates are set up in the following intervals:

|                   |                   |              |
|-------------------|-------------------|--------------|
| **Minimum limit** | **Maximum limit** | **Tax rate** |
| 0.00              | 50.00             | 30%          |
| 50.00             | 100.00            | 20%          |
| 100.00            | 0.00              | 10%          |

The sales tax is the sum of the tax amounts that are calculated for each amount interval.

| Taxable amount (price) | Calculation                                                               | Sales tax |
|------------------------|---------------------------------------------------------------------------|-----------|
| 35.00                  | 35.00 \* 0.30                                                             | 10.50     |
| 50.00                  | 50.00 \* 0.30                                                             | 15.00     |
| 85.00                  | (50.00 \* 0.30 = 15.00) + (35.00 \* 0.20 = 7.00)                          | 22.00     |
| 305.00                 | (50.00 \* 0.30 = 15.00) + (50.00 \* 0.20 = 10.00) + (205 \* 0.10 = 20.50) | 45.50     |

 
-



<a name="see-also"></a>See also
--------

[Determining sale tax rates based on the Marginal base and Calculation method fields](marginal-base-field.md)

[Sales tax calculation methods in the Origin field](https://ax.help.dynamics.com/en/wp-admin/post.php?post=79751&action=edit)


