---
title: Remove outliers from historical transaction data when calculating a demand forecast
description: This article describes how to exclude outliers from the historical data that is used to calculate a demand forecast. By excluding outliers, you can improve forecast accuracy.
author: YuyuScheller
manager: AnnBe
ms.date: 2016-03-30 12 - 34 - 01
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: ReqDemPlanForecastParameters, ReqDemPlanOutlierQuerySetup
audience: Application User
ms.search.scope: AX 7.0.0, Operations
ms.custom: 72621
ms.assetid: 88a964af-14eb-4c5c-945b-388e5908362c
ms.search.region: global
ms.search.industry: Manufacturing
ms.author: roxanad
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 4aa383f3d6dd3ea0fe23a98abe11516dbddd60b5
ms.lasthandoff: 02/22/2017


---

# <a name="remove-outliers-from-historical-transaction-data-when-calculating-a-demand-forecast"></a>Remove outliers from historical transaction data when calculating a demand forecast

This article describes how to exclude outliers from the historical data that is used to calculate a demand forecast. By excluding outliers, you can improve forecast accuracy.

You can exclude outliers to improve forecast accuracy. This is an optional task. Here is an overview of the process:

1.  Click **Master planning** &gt; **Setup** &gt; **Demand forecasting** &gt; **Outlier removal** to open the **Outlier removal** page, where you can use a query to select the transactions to exclude.
2.  Select the company that the query applies to, and then enter a name and description. The **Query date** field is automatically set to the current date.
3.  Select the **Active** check box to exclude the transactions that the query finds from the historical data. This setting will take effect when you create a baseline forecast.
4.  On the **Outlier removal query** page, you can add, remove, and select the criteria that define which transactions will be excluded when the baseline forecast is calculated. For example, select a specific item or order transaction to exclude.
5.  Click **Display transactions**. The **Outlier transactions** page lists the transactions that meet the criteria that you defined in the query, and that will be excluded from the historical data when the demand forecast is calculated.

**Note:** You can also create a query that is based on an existing query. Select the query to copy, and then click **Duplicate**. The **Query date** field identifies the version. You can use the query as it is, or you can click **Edit query** to modify the criteria. You can optionally modify the name and description of the new query.

<a name="see-also"></a>See also
--------

[Introduction to demand forecasting](introduction-demand-forecasting.md)

[Monitoring forecast accuracy](monitor-forecast-accuracy.md)


