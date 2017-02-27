---
title: Single voucher and currency revaluation upgrade for Microsoft Dynamics 365 for Operations version 1611
description: Some organizations enter journals that contain a single voucher that has more than one customer or vendor, and they also run the Accounts receivable or Accounts payable foreign currency revaluation process. This topic describes the steps that these organizations should follow when they upgrade to Microsoft Dynamics 365 for Operations version 1611.
author: twheeloc
manager: AnnBe
ms.date: 2016-12-28 16 - 04 - 17
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: Operations, Core
ms.custom: 265364
ms.assetid: c61391e4-c4bf-4f09-bd18-8107a1bf055e
ms.search.region: Global
ms.author: saraschi
ms.dyn365.ops.intro: 01-11-2016
ms.dyn365.ops.version: Version 1611
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 876bc18d9948106cc56ea5f5501f55ae050287cd
ms.lasthandoff: 02/22/2017


---

# <a name="single-voucher-and-currency-revaluation-upgrade-for-microsoft-dynamics-365-for-operations-version-1611"></a>Single voucher and currency revaluation upgrade for Microsoft Dynamics 365 for Operations version 1611

Some organizations enter journals that contain a single voucher that has more than one customer or vendor, and they also run the Accounts receivable or Accounts payable foreign currency revaluation process. This topic describes the steps that these organizations should follow when they upgrade to Microsoft Dynamics 365 for Operations version 1611.

Follow these steps when you upgrade to Microsoft Dynamics 365 for Operations version 1611.

1.  Before you upgrade to Dynamics 365 for Operations, run the foreign currency revaluation processes for Accounts receivable and Accounts payable. Set the **Method** field to **Invoice date**. A revaluation transaction is created that reverses the last foreign currency revaluation. Therefore, the open transactions are valued at their original accounting currency.
2.  Upgrade to Dynamics 365 for Operations version 1611.
3.  Run the Accounts receivable and Accounts payable foreign currency revaluation processes again. This time, set the **Method** field to **Standard**. A new revaluation transaction is created that is based on the current exchange rates. This transaction records the unrealized gain/loss and the correct summary ledger account.



