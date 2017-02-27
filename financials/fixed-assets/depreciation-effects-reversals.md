---
title: Depreciation effects with reversals
description: This article discusses potential implications of reversing a fixed asset transaction.
author: twheeloc
manager: AnnBe
ms.date: 2015-09-10 20 - 17 - 48
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: AssetTrans
audience: Application User
ms.search.scope: AX 7.0.0, Operations
ms.custom: 2961
ms.assetid: 63a3ac92-c321-4379-a86a-b1b14915f340
ms.search.region: Global
ms.author: saraschi
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 53706287c1aefd12cbdda59c9b4d456bb9ec9a26
ms.lasthandoff: 02/22/2017


---

# <a name="depreciation-effects-with-reversals"></a>Depreciation effects with reversals

This article discusses potential implications of reversing a fixed asset transaction. 

You can reverse fixed asset transactions, and the transactions that are associated with a fixed asset. You can also revoke a reversed transaction. You can reverse or revoke a transaction that was not the most recent transaction posted to the book for the asset. You should first determine whether any depreciation transactions were posted after the transaction that you are reversing. This is because depreciation is not recalculated when you reverse a transaction. Therefore, depreciation often is overstated or understated after the reversal, as shown in the examples. To make sure that depreciation is correct when you reverse a transaction, do not continue with the reversal if you receive a message that states that depreciation will not be recalculated. Instead, first reverse the depreciation transaction that was posted after the transaction you tried to reverse, and then continue with the reversal. You will not be warned about depreciation recalculations, and you can continue with the reversal. The following examples show the calculations that occur if you continue beyond the message without first reversing the depreciation transactions.

## <a name="example-1-depreciation-is-overstated"></a>Example 1: Depreciation is overstated
An asset is set up with a 5-year useful life and straight line depreciation (60 depreciation periods). In this example, depreciation is overstated.
#### <a name="asset-transaction-history"></a>Asset transaction history

| Date       | Transaction type                                                          | Amount                                                                                           |
|------------|---------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| January 1  | Acquisition                                                               | 59,000.00                                                                                        |
| January 1  | Acquisition adjustment                                                    | 1,000.00                                                                                         |
| January 31 | Depreciation (created by using a proposal for one period of depreciation) | 1,000.00Calculation: Book value (59,000 + 1,000) / Number of depreciation periods remaining (60) |

#### <a name="reversal-action"></a>Reversal action

| Date      | Transaction type                | Amount    |
|-----------|---------------------------------|-----------|
| January 1 | Acquisition adjustment reversal | –1,000.00 |

#### <a name="depreciation-effect"></a>Depreciation effect

| Date        | Transaction type        | Amount                                                                                                      |
|-------------|-------------------------|-------------------------------------------------------------------------------------------------------------|
| February 28 | Depreciation (proposal) | 983.05Calculation: Book value (59,000 - 1,000 depreciation) / Number of depreciation periods remaining (59) |

Depreciation is overstated by 16.95 (1,000 - 983.05).

## <a name="example-2-depreciation-is-understated"></a>Example 2: Depreciation is understated
An asset is set up with a 5-year useful life and straight line depreciation (60 depreciation periods). In this example, depreciation is understated.
#### <a name="asset-transaction-history"></a>Asset transaction history

| Date       | Transaction type                                                          | Amount                                                                                         |
|------------|---------------------------------------------------------------------------|------------------------------------------------------------------------------------------------|
| January 1  | Acquisition                                                               | 59,000.00                                                                                      |
| January 1  | Write-down adjustment                                                     | 1,000.00                                                                                       |
| January 31 | Depreciation (created by using a proposal for one period of depreciation) | 966.67Calculation: Book value (59,000 - 1,000) / Number of depreciation periods remaining (60) |

#### <a name="reversal-action"></a>Reversal action

| Date      | Transaction type               | Amount    |
|-----------|--------------------------------|-----------|
| January 1 | Write-down adjustment reversal | –1,000.00 |

#### <a name="depreciation-effect"></a>Depreciation effect

| Date        | Transaction type        | Amount                                                                                                       |
|-------------|-------------------------|--------------------------------------------------------------------------------------------------------------|
| February 28 | Depreciation (proposal) | 983.62Calculation: Book value (59,000 - 966.67 depreciation) / Number of depreciation periods remaining (59) |

Depreciation is understated by 16.95 (983.62 - 966.67).

 
-



<a name="see-also"></a>See also
--------

[Fixed asset depreciation](fixed-asset-depreciation.md)


