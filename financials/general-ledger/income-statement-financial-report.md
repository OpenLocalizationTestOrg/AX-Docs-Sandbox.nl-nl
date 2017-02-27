---
title: Income statement financial report
description: This article describes the default report for income statements. It also describes the building blocks that are associated with this report.
author: twheeloc
manager: AnnBe
ms.date: 2015-11-04 19 - 35 - 20
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.reviewer: annbe
ms.search.scope: AX 7.0.0, Operations
ms.custom: 12294
ms.assetid: 30820be0-d943-4f8b-8c25-6414ec393b3d
ms.search.region: Global
ms.author: jcart
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: aaaa3afd03173a550f6157cea51f443dd9f0dd53
ms.lasthandoff: 02/22/2017


---

# <a name="income-statement-financial-report"></a>Income statement financial report

This article describes the default report for income statements. It also describes the building blocks that are associated with this report. 

<a name="default-income-statement-report"></a>Default income statement report
-------------------------------

| Default report             | What it does                                                                                              |
|----------------------------|-----------------------------------------------------------------------------------------------------------|
| Income Statement – Default | Provides a view of the organization’s profitability for the current period and also for the year to date. |

## <a name="building-blocks"></a>Building blocks
The income statement financial report uses the following building blocks.

| Default report             | Row definition                     | Column definition          |
|----------------------------|------------------------------------|----------------------------|
| Income Statement - Default | Summary Income Statement - Default | Periodic and YTD - Default |

### <a name="row-definition"></a>Row definition

The row definition, Summary Income Statement – Default, contains a section for each part of a traditional income statement. The Main Account Category dimension is used to build this row definition. Therefore, anyone can generate the report without having to make any modifications.

### <a name="column-definition"></a>Column Definition

The column definitions contain different types of columns to provide different levels of detail and financial data.

-   **Periodic and YTD – Default column types:**
    -   **DESC** – The description from the row definition
    -   **FD** – Financial data for the current period
    -   **FD** – Financial data for the year to date

 

<a name="see-also"></a>See also
--------

[Financial reporting](financial-reporting-getting-started.md)

[View financial reports](view-financial-reports.md)

[Dynamics Financial Reportign Blog](http://blogs.msdn.com/b/dynamics_financial_reporting/)


