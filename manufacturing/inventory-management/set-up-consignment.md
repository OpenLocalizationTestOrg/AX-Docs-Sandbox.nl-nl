---
title: Set up consignment | Microsoft Docs
description: This topic explains how to configure inbound consignment inventory operations.
author: YuyuScheller
manager: AnnBe
ms.date: 2016-10-31 13:59:51
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
keywords: DirPartyTable, EcoResTrackingDimensionGroup, InventJournalName, InventJournalOwnershipChange, InventOwner, InventTableInventoryDimensionGroups, VendTable
audience: Application User
ms.reviewer: 2084
ms.suite: Released- Dynamics 365 for Operations version 1611
ms.custom: 220804
ms.assetid: 9dbee4cc-5b34-458f-bdb4-6a48252b9cb3
ms.region: Global
ms.author: perlynne
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: f7b3b49a2c600f9a7d4a3c2ec407a627a459e7b5


---

# <a name="set-up-consignment"></a>Set up consignment

This topic explains how to configure inbound consignment inventory operations. 

Consignment inventory is inventory that’s owned by a vendor, but stored at your site. When you’re ready to consume or use the inventory, you take over the ownership of the inventory. This topic describes the setup needed to enable consignment processes. For more information about consignment processes, see [Consignment](https://docs.microsoft.com/en-us/dynamics365/operations/manufacturing/inventory-management/consignment).

## <a name="inventory-owners"></a>Inventory owners
In order to record physical inbound consignment inventory, you need to define a vendor owner. This is done on the **Inventory owner** page. When you select a **Vendor account** this generates default values for the **Name** and **Owner** fields. The value in the **Owner** field will be visible to the vendor, so you might want to change it if your vendor account names aren’t easy for external people to recognize. It’s possible to edit the **Owner** field, but only up to the point when you save the **Inventory owner** record. The **Name** field is populated with the name of the party that the vendor account is associated with, and this cannot be changed. [![inventory-owners](./media/inventory-owners.png)](./media/inventory-owners.png)

## <a name="tracking-dimension-group"></a>Tracking dimension group
Items that are going to be used in consignment processes must be associated with a **Tracking dimension group** where the **Owner** dimension is set to **Active**. The Owner dimension always has the **Physical inventory** and **Financial inventory** options selected. The **Coverage plan by dimension** is never selected. [![tracking-dimension-group](./media/tracking-dimension-group.png)](./media/tracking-dimension-group.png)

## <a name="inventory-ownership-change-journal"></a>Inventory ownership change journal
The **Inventory ownership change** journal is used to record the transfer of ownership of consignment inventory from the vendor to the legal entity that’s consuming it. Like any inventory journal, it must be identified with an Inventory journal name. These names are created on the **Inventory journal names** page, and the **Journal type** must be set to **Ownership change**. [![inventory-ownership-change-journal](./media/inventory-ownership-change-journal.png)](./media/inventory-ownership-change-journal.png)

## <a name="vendor-collaboration-in-consignment-processes"></a>Vendor collaboration in consignment processes
If your vendors are using the vendor collaboration interface, they can use this to monitor the consumption of inventory at your site. For more information about setting up vendors to use vendor collaboration, see [Configuration of security for vendor collaboration users](https://docs.microsoft.com/en-us/dynamics365/operations/manufacturing/procurement-sourcing/configuring-security-for-vendor-portal-users).




<!--HONumber=Feb17_HO3-->


