---
title: Update standard costs in a manufacturing environment | Microsoft Docs
description: This article provides guidance about how to update standard costs in a manufacturing environment.
author: YuyuScheller
manager: AnnBe
ms.date: 2016-04-11 13:25:58
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
keywords: CostingVersion, InventStdCostConv
audience: Application User
ms.reviewer: 2094
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 79663
ms.assetid: 9b93388b-17b8-48de-aee1-1a5a4dafaa1f
ms.region: Global
ms.industry: Manufacturing
ms.author: mguada
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: 49b0fe694469d9405e600d33ee20fa76197512d3


---

# <a name="update-standard-costs-in-a-manufacturing-environment"></a>Update standard costs in a manufacturing environment

This article provides guidance about how to update standard costs in a manufacturing environment. 

Updates can reflect new items, cost categories, or indirect cost calculation formulas. They can also reflect corrections and cost changes. The type of update affects the steps that you must complete to update standard costs, as illustrated in the following cases:

-   Enter expected standard cost changes for purchased items, and then change the status of the item cost records to **Active** on the appropriate date. However, don't recalculate the costs of manufactured items that use the purchased items.
-   Enter standard costs for a new purchased item, but don't recalculate the costs of manufactured items that have a bill of materials (BOM) version that contains the new purchased item as a component.
-   Correct or change the cost of a purchased item, or change the cost group that is assigned to a purchased item, and calculate the cost for all manufactured items that have a BOM version that contains the purchased item as a component.
-   Change the cost for a cost category, and calculate the cost for all manufactured items that have a route version that contains routing operations that use the cost category.
-   Change the cost categories that are assigned to routing operations or the cost group that is assigned to cost categories. Then calculate the cost for all manufactured items that have a route version that contains routing operations that use the cost category.
-   Change an indirect cost calculation formula, and calculate the cost for all manufactured items that are affected by the change.
-   Change or add a manufacturing site for a manufactured item, and calculate the item's manufactured cost for the site.
-   Calculate, or recalculate, the cost for a manufactured item, and recalculate the cost for all manufactured items that have a BOM version that contains the manufactured item as a component.
-   Calculate costs for a new manufactured item, based on its defined, approved, and active BOM and route information.

Each case requires careful consideration about how to update standard costs.




<!--HONumber=Feb17_HO3-->


