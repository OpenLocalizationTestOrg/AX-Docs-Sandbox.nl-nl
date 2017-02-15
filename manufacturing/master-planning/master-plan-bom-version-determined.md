---
title: Determine the BOM version | Microsoft Docs
description: During a demand explosion, if an item has a default order type of Production, the planning engine finds a valid BOM version based on the site.
author: YuyuScheller
manager: AnnBe
ms.date: 2015-09-10 08:51:05
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
keywords: BOMConsistOf, BOMDesigner, BOMTable, InventItemOrderSetup
audience: Application User
ms.reviewer: YuyuScheller
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 2534
ms.assetid: b78c3887-a37c-4766-a6be-200c59f071ec
ms.region: Global
ms.industry: Manufacturing
ms.author: roxanad
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: 69ee3b6d43a41ea84e97253faf980e16abe9014a


---

# <a name="determine-the-bom-version"></a>Determine the BOM version

During a demand explosion, if an item has a default order type of Production, the planning engine finds a valid BOM version based on the site. 

The site dimension is always known and is stated on the demand transaction. The following process is used to determine the BOM version to use:

-   If there is a BOM version defined for the item at the demand site, the site-specific BOM is used.
-   If there is no site-specific BOM version defined for an item at the demand site, a general BOM is used. A general BOM does not state a site, and it is valid for multiple sites. If there is a general BOM, it is used.
-   If there is no general BOM version to use, the demand explosion stops at this point.

A valid BOM version, whether site-specific or general, must meet the required criteria for date and quantity.






<!--HONumber=Feb17_HO3-->


