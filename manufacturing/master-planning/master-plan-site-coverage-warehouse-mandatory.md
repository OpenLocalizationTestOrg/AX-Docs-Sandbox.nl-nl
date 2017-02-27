---
title: Master planning for site coverage, mandatory warehouse
description: This topic describes how an item that has the site as coverage dimension is planned. Warehouse is a mandatory dimension.
author: YuyuScheller
manager: AnnBe
ms.date: 2015-09-10 08 - 45 - 56
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: EcoResStorageDimensionGroup, ReqItemTable
audience: Application User
ms.reviewer: YuyuScheller
ms.search.scope: AX 7.0.0, Operations
ms.custom: 2454
ms.assetid: aa135030-f98c-48bf-902c-e52f680dc247
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: roxanad
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 58e2d8ac1c51a7dbca97a18b6251061c78b0134d
ms.lasthandoff: 02/22/2017


---

# <a name="master-planning-for-site-coverage-mandatory-warehouse"></a>Master planning for site coverage, mandatory warehouse

This topic describes how an item that has the site as coverage dimension is planned. Warehouse is a mandatory dimension.

This master planning scenario involves the following conditions:

-   The site dimension is set to mandatory and must be entered on the demand transaction. This setting can't be modified.
-   The warehouse dimension is set to mandatory and must be entered on the demand transaction.
-   The site dimension is set for coverage planning. Other dimensions may be set for coverage planning also. However, they are not affected by the multisite functionality.
-   The warehouse dimension is not set for coverage planning. Therefore, supply and demand are aggregated by site and, perhaps, other coverage-planned dimensions also.

The following graphic illustrates how master planning proceeds. The parameters that are referred to in the graphic, and their locations, are as follows:
-   Item coverage is defined for the item. Click **Product information management &gt; Products&gt; Released products**. Select the item, and then click **Plan &gt; Item coverage**.
-   Refill relations are defined for the warehouse. Click **Inventory management &gt; Setup &gt; Inventory breakdown &gt; Warehouses**. On the **Master planning** tab, see the **Main warehouse** field group.
-   The default order type is set to Production, Purchase order, or Kanban. Click **Product information management &gt; Products&gt; Released products**. Select the item, and then click **Plan &gt; Default order settings**. In the **Default order settings** form, see the **Default order type**.

![Demand for site coverage warehouse mandatory](./media/multisitedemandexplosionscenarioforsitecoveragewarehousemandatory.jpg)



<a name="see-also"></a>See also
--------

[Master planning and multisite functionality](master-plan-multisite-functionality.md)

[Master planning - site and warehouse coverage, warehouse mandatory](master-plan-site-warehouse-coverage-warehouse-mandatory.md)

[Master planning - site coverage. warehouse mandatory](master-plan-site-coverage-warehouse-mandatory.md)

[Master planning - site and warehouse coverage, warehouse not mandatory](master-plan-site-warehouse-coverage-warehouse-not-mandatory.md)

[Master planning - How the BOM version is determined](master-plan-bom-version-determined.md)


