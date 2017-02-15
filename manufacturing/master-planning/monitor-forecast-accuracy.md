---
title: Monitor forecast accuracy | Microsoft Docs
description: This article describes the types of forecast accuracy that Microsoft Dynamics 365 for Operations calculates, and explains how you can view the accuracy values.
author: YuyuScheller
manager: AnnBe
ms.date: 2016-03-30 12:36:55
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.reviewer: 2094
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 72863
ms.assetid: f6ab5e66-020e-4286-9a5a-59dd47476b30
ms.region: global
ms.industry: Manufacturing
ms.author: roxanad
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: cee8ac74699f7005f24105b80694be36c7085bff


---

# <a name="monitor-forecast-accuracy"></a>Monitor forecast accuracy

This article describes the types of forecast accuracy that Microsoft Dynamics 365 for Operations calculates, and explains how you can view the accuracy values.

Dynamics 365 for Operations calculates the following types of forecast accuracy:

-   Historical forecast accuracy, by comparing the historical forecast that Master Planning uses with the historical demand. To view the values (both absolute values and percentage values) for historical forecast accuracy, click **Show accuracy** on the **Demand forecast details** page.
-   The estimated accuracy of the forecasting model that is used to generate the predictions. You can view the accuracy percentage under **Model details - MAPE** on the **Demand forecast details** page. **Note:** If you use the Dynamics 365 for Operations Demand forecasting Microsoft Azure Machine Learning service, the calculation of internal model accuracy is based on the test data set. To specify the size of the test data set, set the **TEST\_SET\_SIZE\_PERCENT** parameter on the **Demand forecasting parameters** page. For example, if you set the value to **20**, the last 20 percent of the historical data will be used to calculate the internal model accuracy.


<a name="see-also"></a>See also
--------

[Authorizing the adjusted forecast](https://docs.microsoft.com/en-us/dynamics365/operations/manufacturing/master-planning/authorizing-the-adjusted-forecast)

[Remove outliers from historical transaction data when calculating a demand forecast](https://docs.microsoft.com/en-us/dynamics365/operations/manufacturing/master-planning/remove-outliers-from-historical-transaction-data-when-calculating-a-demand-forecast)




<!--HONumber=Feb17_HO3-->


