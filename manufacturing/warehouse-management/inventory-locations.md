---
title: Inventory locations | Microsoft Docs
description: Inventory locations are used with basic warehousing (WMS I) to determine where items are stored and where items are picked from in a WMS I warehouse.
author: YuyuScheller
manager: AnnBe
ms.date: 2015-09-10 08:08:37
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
keywords: WMSLocation
audience: Application User
ms.reviewer: 2084
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 2134
ms.assetid: ac338e30-e350-46ba-80b9-7464082f61f9
ms.region: Global
ms.industry: Distribution
ms.author: perlynne
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: aa9ce2980ae8939131fa152658dd59c4e8610816


---

# <a name="inventory-locations"></a>Inventory locations

Inventory locations are used with basic warehousing (WMS I) to determine where items are stored and where items are picked from in a WMS I warehouse.

This topic applies to features in the Inventory management module. It does not apply to features in the Warehouse management module.

The term location refers to the place that items are stored and drawn from.

For each location, the place where the item is inserted can also be specified. By default, they are the same. Items are usually inserted and drawn from the same side of a location, but not always. For example, items that are stored in live storage racks are inserted from one aisle and drawn from another. The main input is given by a location name, which is usually determined by its coordinates: warehouse, aisle, rack, shelf, and bin. This name or ID can be entered manually or generated from the location coordinates—for example, 01-02-03-4 for aisle 1, rack 2, shelf 3, bin 4 in the Inventory locations page.
Location properties
-------------------

A location has the following characteristics:
-   Size (height, width, depth, and thereby volume)
-   Warehouse, aisle, rack, shelf, and bin position
-   Location type (bulk location, picking location, inbound dock, outbound dock, production input location, inspection location, or kanban supermarket)

Check text can be used in online systems to verify that the operator has selected the correct location for a specific item. This check text can be created manually or by default.

## <a name="sort-codes"></a>Sort codes
Use sort codes to optimize the handling of picking lines, which describe the information that is required for picking items from inventory, including the picking order. Sort codes can be specified by the aisle and other coordinates, or assigned manually for the location.

## <a name="blocked-locations"></a>Blocked locations
Occasionally, you might want to indicate that a location is blocked for a period of time, for example, to allow for repairs. At other times, you may want to indicate blocking of only the input or only output.
Tree structure
--------------

In the Inventory locations page, you can view the warehouse layout in a tree structure based on the coordinates of inventory locations, in a defined display format.
Maintain inventory locations via the warehouse form
---------------------------------------------------

It is possible to copy locations from one warehouse to another and to create locations via a wizard. Before you run the wizard you should make sure that you have defined the default location names on the Warehouse page.



<a name="see-also"></a>See also
--------

[Create a new warehouse layout](https://ax.help.dynamics.com/en/wiki/create-a-new-warehouse-layout/)




<!--HONumber=Feb17_HO3-->


