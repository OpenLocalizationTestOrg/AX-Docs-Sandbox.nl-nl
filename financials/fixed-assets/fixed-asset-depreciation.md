---
title: Fixed asset depreciation
description: This article provides an overview of depreciation for fixed assets.
author: twheeloc
manager: AnnBe
ms.date: 2015-09-10 20 - 21 - 29
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: AssetBonus, AssetBookTable
audience: Application User
ms.search.scope: AX 7.0.0, Operations
ms.custom: 3121
ms.assetid: 98ff891f-e0e2-4184-b618-28107a50851f
ms.search.region: Global
ms.author: saraschi
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 3c0a80f9530519e21fb3cef5d6926d38ab2ef277
ms.lasthandoff: 02/22/2017


---

# <a name="fixed-asset-depreciation"></a>Fixed asset depreciation

This article provides an overview of depreciation for fixed assets.

Depreciation is a periodic transaction that typically reduces the value of the fixed asset on the balance sheet, and is charged as an expenditure to a profit and loss account. Therefore, a main account is typically used to credit the periodic depreciation on the balance sheet. An offset account is an account in the profit and loss part of the chart of accounts.

## <a name="depreciation-adjustment"></a>Depreciation adjustment
Usually, only a correction to a posted depreciation transaction is posted as a depreciation adjustment. Therefore, both the main account and the offset account are set up just like the accounts for depreciation. A depreciation adjustment can be either a positive amount or a negative amount, but the functionality of the main account (as a balance sheet account) and the functionality of the offset account (usually as a profit and loss account) remain the same.

## <a name="extraordinary-depreciation"></a>Extraordinary depreciation
Extraordinary depreciation works like basic depreciation. Therefore, a main account is used to credit the depreciation amount to the balance sheet and reduce the value of the fixed asset. An offset account is a profit and loss account, where the depreciation that is calculated for the fiscal period is charged as an expenditure. Extraordinary depreciation works independently of basic depreciation. By having extraordinary depreciation as a separate transaction type, you can post and report the extraordinary depreciation separately from the basic depreciation.

## <a name="special-depreciation-allowance"></a>Special depreciation allowance
You can use special depreciation allowances to take extra depreciation amounts during the first year that an asset is put in service and depreciated. Special depreciation allowances must be taken before any other depreciation calculations. Because special depreciation allowances are often unknown until later in the service life of the fixed asset, it's best to use this type of depreciation with a book that doesn't post to the general ledger. You can use the Delete transactions not posted to general ledger periodic function to delete the transaction history for these books. You can then delete the depreciation history for the fixed asset book, post the special depreciation allowance when it's known, and then post the remaining depreciation transactions for the year. You can create an unlimited number of special depreciation allowance records. After you assign those records to an asset group book, they are applied to the asset book. A special depreciation allowance is entered as either a percentage or a fixed amount. When you post depreciation proposals, special depreciation allowance transactions are posted to the book as transactions that are separate from the depreciation transactions.

## <a name="depreciation-calendars"></a>Depreciation calendars
Each book has a calendar that is used when you depreciate fixed assets. By default, if you don't indicate a calendar on the book, the book uses the ledger fiscal calendar. You must select a fiscal calendar for a book when the depreciation profile that is associated with the book uses a fiscal depreciation year. You can create shared calendars by using the **Fiscal calendars** page in General ledger.

<a name="see-also"></a>See also
--------

[Depreciation methods and conventions](depreciation-methods-conventions.md)


