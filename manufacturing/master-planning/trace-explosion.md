---
title: Use tracing for explosion
description: This article explains how you can use tracing to explore the causes behind the outcome of an order explosion.
author: YuyuScheller
manager: AnnBe
ms.date: 2015-12-07 09 - 15 - 50
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: ReqTransExplosion
audience: Application User
ms.reviewer: YuyuScheller
ms.search.scope: AX 7.0.0, Operations
ms.custom: 19231
ms.assetid: 9bc9bfbe-a7a9-437b-a947-826229b0585a
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: roxanad
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 8bfa9a19f4fba81e804d490cee08b7cd810f7394
ms.lasthandoff: 02/22/2017


---

# <a name="use-tracing-for-explosion"></a>Use tracing for explosion

This article explains how you can use tracing to explore the causes behind the outcome of an order explosion.

By enabling tracing, you can view information about the factors that contributed to the outcome of the explosion of a particular order. The following examples show how you can use the tracing information:

-   View relations between the actions on planned orders to optimize the supply chain and inventory reservations.
-   View relations to orders that are already approved. You can focus on automatically firming derived requirements and then prioritize orders more accurately.
-   Simulate planning results to determine whether the planning parameters are optimal.
-   Identify how information such as production dates, quantities, and priorities for an order were determined.

You can view details about futures and actions for a selected order. On the **Explosion** page, tracing information is available on the **Explanation** tab in the upper pane. Tracing occurs when you explode an order. To start tracing for the order, click **Update**, and then select the **Enable trace** check box. You can use the **Find text** field to search the log for specific information. Search results are highlighted in the tree.

<a name="see-also"></a>See also
--------

[Master plans](https://ax.help.dynamics.com/en/wiki//master-plans)


