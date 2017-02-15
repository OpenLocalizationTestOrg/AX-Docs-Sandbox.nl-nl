---
title: Create a bill of lading | Microsoft Docs
description: This topic describes how to create a bill of lading when using warehouse management processes.
author: YuyuScheller
manager: AnnBe
ms.date: 2016-09-22 12:00:26
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
keywords: WHSBillOfLading, WHSLoadPlanningWorkbench
audience: Application User
ms.reviewer: 2084
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 193583
ms.assetid: 0f30de98-97d1-49af-b734-95d8f6e9373d
ms.region: Global
ms.author: yuyus
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: 4c04c337a54ea6005c02b61e96d69c3482436d30


---

# <a name="create-a-bill-of-lading"></a>Create a bill of lading

This topic describes how to create a bill of lading when using warehouse management processes. 


A bill of lading is a legal document between the company that ships the items and the carrier. The document accompanies the shipped items, and it serves as a receipt of shipment when the items are delivered at the destination. If you're using warehouse management, there are two ways to generate a bill of lading:

-   Create the report manually, using the **Bill of lading** page.
-   Generate the report from the **Load planning workbench**.

If you generate the bill of lading from the **Load planning workbench**, the load status must be **Shipped.** If there's more than one shipment in the load, a bill of lading is created for each shipment. After a bill of lading has been created you can make changes to it on the **Bill of lading** page.

## <a name="master-bill-of-lading"></a>Master bill of lading
If there's more than one shipment in the load, you can generate a master bill of lading. This has the same layout and information as a bill of lading, but contains the summarized content for all the shipments. If the **Create a master bill of lading when there's more than one shipment on a load** option is set to **Yes** on the **Transportation management parameters** page, a master bill of lading is automatically generated if you create a bill of lading from the **Load planning workbench**, and there's more than one shipment. You can also get a list of the bills of lading by clicking **Related information** &gt; **Bill of lading**. If you're creating bills of lading manually, you can create a master bill of lading on the **Bill of lading** page.




<!--HONumber=Feb17_HO3-->


