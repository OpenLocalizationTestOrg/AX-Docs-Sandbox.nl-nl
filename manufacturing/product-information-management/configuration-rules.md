---
title: Configuration rules
description: This article provides general information about configuration rules. Configuration rules define relationships between items in a bill of materials (BOM) for products that use the dimension-based configuration technology.
author: YuyuScheller
manager: AnnBe
ms.date: 2015-12-07 17 - 51 - 44
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: BOMConfigRule
audience: Application User
ms.reviewer: YuyuScheller
ms.search.scope: AX 7.0.0, Operations
ms.custom: 19761
ms.assetid: e4c6622d-1e2d-4a4d-8047-c553a25d4f87
ms.search.region: Global
ms.author: yuyus
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 6482ee7305642abf1e4c95b22739b1ff60b2e3a4
ms.lasthandoff: 02/22/2017


---

# <a name="configuration-rules"></a>Configuration rules

This article provides general information about configuration rules. Configuration rules define relationships between items in a bill of materials (BOM) for products that use the dimension-based configuration technology.

Configuration rules are available when you define dimension-based configuration models. Configuration rules are used to either enforce or prohibit specific item combinations in a bill of materials (BOM). After a BOM has been created and the relevant items have been assigned to their respective configuration groups, one or more configuration rules can be defined. If two items belong together, the **Select** operator is used to ensure inclusion. If two items are mutually exclusive, the **Deselect** operator is used to ensure exclusion. **Note:** This information applies only to product masters that use the dimension-based configuration technology. Existing configurations aren't affected by subsequent changes to the configuration rules. However, it's important that you set the rules before you define a new configuration, and that you check the rules if you think they have been changed. **Note:** For the **Select** method, the derived configuration group, item number, and configuration are automatically selected. For the **Deselect** method, the derived configuration group, item number, and configuration can't be selected.

<a name="see-also"></a>See also
--------

[Dimension-based product configuration](https://ax.help.dynamics.com/en/?post_type=incsub_wiki&p=231054)


