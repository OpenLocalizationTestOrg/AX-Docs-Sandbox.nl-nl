---
title: Round-off amount for depreciation calculations
description: This article discusses the Round-off depreciation field that is found on the Book setup pages.
author: twheeloc
manager: AnnBe
ms.date: 2015-12-02 23 - 00 - 51
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
ms.search.form: AssetBookTable, AssetDepBookTable
audience: Application User
ms.search.scope: AX 7.0.0, Operations
ms.custom: 13931
ms.assetid: faf7db87-046f-41d1-9baf-0df66e373e97
ms.search.region: Global
ms.author: saraschi
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 8fb9a95dee199cb62695f09e1ffbf0492396fd0a
ms.lasthandoff: 02/22/2017


---

# <a name="round-off-amount-for-depreciation-calculations"></a>Round-off amount for depreciation calculations

This article discusses the Round-off depreciation field that is found on the Book setup pages.

Round-off depreciation amounts are set for each book. Round-off depreciation amounts are used in the fixed asset depreciation profile that shows the future depreciation and value of the fixed asset, and also in depreciation proposals. Enter the lowest depreciation amount that is allowed for the book. Regardless of the rounding that is set up, the depreciation amount in the last depreciation period isn't rounded. At the end of the last depreciation period, the value of the fixed asset must be 0 (zero) or the scrap value, if scrap value is used.

### <a name="example"></a>Example

Depreciation without rounding is calculated as 2,444.44. As the following table shows, the amounts that are suggested vary, depending on how rounding is set up.

| Rounding method | Depreciation amount |
|-----------------|---------------------|
| Rounding 0.1    | 2,444.40            |
| Rounding 1.00   | 2,444.00            |
| Rounding 10.00  | 2,440.00            |
| Rounding 100.00 | 2,400.00            |




