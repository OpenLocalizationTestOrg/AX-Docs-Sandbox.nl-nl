---
title: Create production orders
description: When a production order is created, a request is initiated to start producing an item. The production order contains information about what will be produced, the quantity to produce, and the planned finish date. It also contains information about which materials to consume and which process to follow to produce the item.
author: YuyuScheller
manager: AnnBe
ms.date: 2015-12-07 17 - 51 - 31
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: ProdTable, ProdTableCreate
audience: Application User
ms.reviewer: annbe
ms.search.scope: AX 7.0.0, Operations
ms.custom: 19741
ms.assetid: bbb6e69d-479c-45fc-a0a8-66da5df16c7f
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: johanho
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 330897407e53bf56f71afecece032fb99fa66bb7
ms.lasthandoff: 02/22/2017


---

# <a name="create-production-orders"></a>Create production orders

When a production order is created, a request is initiated to start producing an item. The production order contains information about what will be produced, the quantity to produce, and the planned finish date. It also contains information about which materials to consume and which process to follow to produce the item.

A production order passes through stages of the production life cycle. When an order is created, it is assigned the status **Created**. When an order is finished, it is assigned the status **Ended**. A parameter setting in each stage allows a user to configure each step. The setting can be set up for a single user or for all users.

The production bill of material and the production route are the main entities of the production order. They are copied to the production order based on the selected item and quantity that are going to be produced. Before the production order is started, the production bill of material and route can be edited.

A production order can be created in the following scenarios:

-   Created by master planning execution based on material demand.
-   Created directly from a sales order line or when a higher-level production order is created and estimated (pegged supply).
-   Created manually.



