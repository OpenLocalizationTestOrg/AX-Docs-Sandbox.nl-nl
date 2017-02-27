---
title: Manage store inventory
description: This article describes the types of documents that you can use to manage inventory.
author: josaw1
manager: AnnBe
ms.date: 2015-12-09 18 - 39 - 11
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations
ms.custom: 21391
ms.assetid: bfef3717-d0e0-491d-8466-d8a9c995177d
ms.search.region: global
ms.search.industry: Retail
ms.author: rubendel
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 435ca4aa9acea9187209a52b609389f017f34a87
ms.lasthandoff: 02/22/2017


---

# <a name="manage-store-inventory"></a>Manage store inventory

This article describes the types of documents that you can use to manage inventory.

You can use the following types of documents to manage your organization's inventory.

## <a name="purchase-orders"></a>Purchase orders
Purchase orders are created at the head office. If a retail warehouse is included in the purchase order header, the order can be received at the store by using Modern POS (MPOS) or Cloud POS in Microsoft Dynamics 365 for Operations - Retail. After the quantities that are received at the store are entered, they can be saved locally for additional modification. Alternatively, the quantities can be committed and sent to the head office. At the head office, the quantities that were received at the store are displayed in Dynamics 365 for Operations, in the **Receive now** field on the purchase order.
Transfer orders
---------------

A transfer order can specify that a particular store is a location that items can be shipped from. In this case, the transfer order appears at the store as a picking request in MPOS or Cloud POS. After the quantities that are requested are picked, they are committed and sent to the head office. At the head office, the quantities that were picked at the store are displayed in Dynamics 365 for Operations, in the **Ship now** field on the transfer order. A transfer order may specify that a particular store is a location that items can be shipped to. In this case, the transfer order appears at the store as a receiving request in MPOS or Cloud POS. After the quantities that are received at the store are entered, they can be saved locally for additional modification. Alternatively, the quantities can be committed and sent to the head office. At the head office, the quantities that were received at the store are displayed in Dynamics 365 for Operations, in the **Receive now** field on the transfer order.

## <a name="stock-counts"></a>Stock counts
Stock counts can be either scheduled or unscheduled. Scheduled stock counts are initiated at the head office, which specifies the items that must be counted. The head office creates a counting document that can be received at the store, where the quantities of actual on-hand stock are entered in MPOS or Cloud POS. Unscheduled stock counts are initiated at a store, and the quantities of actual on-hand stock are updated in either MPOS or Cloud POS. Unlike scheduled stock counts, unscheduled stock counts do not have a predefined list of items. When a stock count of either type is completed, it is committed and sent to the head office. At the head office, the count is validated and posted.




