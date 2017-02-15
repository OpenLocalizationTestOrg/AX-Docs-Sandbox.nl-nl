---
title: Income statement financial report | Microsoft Docs
description: This article describes the default report for income statements. It also describes the building blocks that are associated with this report.
author: twheeloc
manager: AnnBe
ms.date: 2015-11-04 19:35:20
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.reviewer: annbe
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 12294
ms.assetid: d91a6bb8-63ec-4456-93c4-29c8789fb26d
ms.region: Global
ms.author: jcart
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: 7c75cfae15fd975778e6617e270bc3abfe7bb236


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

[Financial reporting](https://docs.microsoft.com/en-us/dynamics365/operations/financials/general-ledger/financial-reporting)

[View financial reports](https://docs.microsoft.com/en-us/dynamics365/operations/financials/general-ledger/view-financial-reports)

[Dynamics Financial Reportign Blog](http://blogs.msdn.com/b/dynamics_financial_reporting/)




<!--HONumber=Feb17_HO3-->


