---
title: Manage store inventory | Microsoft Docs
description: This article describes the types of documents that you can use to manage inventory.
author: josaw1
manager: AnnBe
ms.date: 2015-12-09 18:39:11
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.reviewer: josaw1
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 21391
ms.assetid: 9bdb9854-ff74-4522-869a-3208a79b81e3
ms.region: global
ms.industry: Retail
ms.author: rubendel
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: a1aedcd80e238a86593663b03bf5c0ed7b4b2302


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






<!--HONumber=Feb17_HO3-->


