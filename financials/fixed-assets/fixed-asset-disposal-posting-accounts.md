---
title: Fixed asset disposal posting accounts
description: This article explains how to set up general ledger posting accounts for disposing of assets.
author: twheeloc
manager: AnnBe
ms.date: 2015-09-10 21 - 04 - 08
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: AssetPosting
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: AX 7.0.0, Operations
ms.custom: 3461
ms.assetid: dfdc0730-e030-48cc-8d93-15bdc7b23776
ms.search.region: Global
ms.author: saraschi
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: d0fbe400b900e22245a4265ecd1177c0c930f707
ms.lasthandoff: 02/22/2017


---

# <a name="fixed-asset-disposal-posting-accounts"></a>Fixed asset disposal posting accounts

This article explains how to set up general ledger posting accounts for disposing of assets.

In the Fixed asset posting profiles page, on the Ledger accounts FastTab, select Disposal - sale and Disposal - scrap to set up postings to the ledger.
For both transaction types, the ledger account is credited for the disposal value of the fixed asset. The debit is posted to an offset account, which might be, for example, a bank account. If a fixed asset is sold to a customer, the customer account is used instead of the offset account. Click Disposal and then click Sale or Scrap, and then set up detailed accounts to reverse the net book value of the fixed asset. You can also enter information in the Post value and Sales value type fields in the Disposal parameters page. The disposal transaction for an asset in a low-value pool reduces the net book value of the low-value pool by the disposed amount only. However, when the sale of an asset is exceeds the net book value of the low-value pool, the net book value is reduced to zero.




