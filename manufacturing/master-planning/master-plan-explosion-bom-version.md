---
title: Explosion of a BOM version
description: This article explains a master planning scenario that involves explosion of a bill of materials (BOM) version.
author: YuyuScheller
manager: AnnBe
ms.date: 2015-12-07 09 - 15 - 33
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: ReqTransExplosion
audience: Application User
ms.reviewer: YuyuScheller
ms.search.scope: AX 7.0.0, Operations
ms.custom: 19211
ms.assetid: fe08c2e6-9cc5-4e34-bbb2-cd07843403b5
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: roxanad
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 2e0d32187163f0ac8ad7c2fc35cd750207a3c3d1
ms.lasthandoff: 02/22/2017


---

# <a name="explosion-of-a-bom-version"></a>Explosion of a BOM version

This article explains a master planning scenario that involves explosion of a bill of materials (BOM) version.

A demand explosion of a bill of materials (BOM) version creates a demand for each BOM line item at a specific site and, possibly, at a specific warehouse. In a site-specific BOM, a specific warehouse can be defined for each BOM line. Additionally, for each BOM line, the item's dimension settings determine whether the warehouse is required. The resulting demand for each BOM line item then becomes the starting point for additional demand explosion. This master planning scenario involves the following conditions:

-   The site dimension is mandatory and must be entered on the demand transaction.
-   The site dimension is consistent. Therefore, the site for lower-level demand is the same as the site on the initial demand transaction.

The following illustration shows how the process for master planning demand explosion. ![Demand explosion using BOM version](./media/multisitedemandexplosionscenariousingbomversion.gif)

<a name="see-also"></a>See also
--------

[Master planning - how the BOM version is determined](master-plan-bom-version-determined.md)

[Master planning and multisite functionality](master-plan-multisite-functionality.md)


