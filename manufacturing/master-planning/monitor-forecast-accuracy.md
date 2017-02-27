---
title: Monitor forecast accuracy
description: This article describes the types of forecast accuracy that Microsoft Dynamics 365 for Operations calculates, and explains how you can view the accuracy values.
author: YuyuScheller
manager: AnnBe
ms.date: 2016-03-30 12 - 36 - 55
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations
ms.custom: 72863
ms.assetid: 810a0d63-f4c6-4167-b2b3-a178b74ead89
ms.search.region: global
ms.search.industry: Manufacturing
ms.author: roxanad
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 16b6bcc802836620d49f82f284f0256c2d199438
ms.lasthandoff: 02/22/2017


---

# <a name="monitor-forecast-accuracy"></a>Monitor forecast accuracy

This article describes the types of forecast accuracy that Microsoft Dynamics 365 for Operations calculates, and explains how you can view the accuracy values.

Dynamics 365 for Operations calculates the following types of forecast accuracy:

-   Historical forecast accuracy, by comparing the historical forecast that Master Planning uses with the historical demand. To view the values (both absolute values and percentage values) for historical forecast accuracy, click **Show accuracy** on the **Demand forecast details** page.
-   The estimated accuracy of the forecasting model that is used to generate the predictions. You can view the accuracy percentage under **Model details - MAPE** on the **Demand forecast details** page. **Note:** If you use the Dynamics 365 for Operations Demand forecasting Microsoft Azure Machine Learning service, the calculation of internal model accuracy is based on the test data set. To specify the size of the test data set, set the **TEST\_SET\_SIZE\_PERCENT** parameter on the **Demand forecasting parameters** page. For example, if you set the value to **20**, the last 20 percent of the historical data will be used to calculate the internal model accuracy.


<a name="see-also"></a>See also
--------

[Authorizing the adjusted forecast](authorize-adjusted-forecast.md)

[Remove outliers from historical transaction data when calculating a demand forecast](remove-historical-outliers-calculating-demand-forecast.md)


