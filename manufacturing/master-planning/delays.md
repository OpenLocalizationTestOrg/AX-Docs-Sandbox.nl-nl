---
title: Delays
description: This article provides information about delayed dates in master planning. A delayed date is a realistic due date that a transaction receives if the earliest fulfillment date that master planning calculates is later than the requested date.
author: YuyuScheller
manager: AnnBe
ms.date: 2015-12-07 09 - 17 - 45
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: ReqTransFuturesListPage
audience: Application User
ms.reviewer: YuyuScheller
ms.search.scope: AX 7.0.0, Operations
ms.custom: 19311
ms.assetid: 5ffb1486-2e08-4cdc-bd34-b47ae795ef0f
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: roxanad
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 2a14c1587d0f631e8e101dffc797d3139fc79b20
ms.lasthandoff: 02/22/2017


---

# <a name="delays"></a>Delays

This article provides information about delayed dates in master planning. A delayed date is a realistic due date that a transaction receives if the earliest fulfillment date that master planning calculates is later than the requested date.

Master planning can calculate the earliest fulfillment date for a transaction, based on lead times, material availability, capacity availability, and various planning parameters. If master planning calculates an order date that precedes the current date, the order can't be fulfilled on time. Therefore, the order is delayed. In this case, master planning forward-plans the order from the current date and includes lead times. These lead times start with any lower-level component items. The order then receives a delayed date. A delayed date is a realistic due date, based on the current data. Master planning also calculates the number of delay days. In some situations, you might choose not to calculate delays, such as when users know that they can expedite lead times by selecting alternative modes of delivery. You can configure how delays are calculated for a coverage group. You can then attach the coverage group to an item later. On the **Master planning parameters** page, you can set the start time for the calculation of delays. If an order is fulfilled after this time, a delay of one day is added to the delay date of the order. **Note:** In earlier versions, calculated delays were known as *futures messages*, the delayed date was known as the *futures date*, and a delayed transaction was referred to as *a transaction that was future set*.

<a name="see-also"></a>See also
--------

[Coverage settings](coverage-settings.md)


