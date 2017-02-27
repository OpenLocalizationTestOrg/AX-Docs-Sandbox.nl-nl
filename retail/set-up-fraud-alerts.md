---
title: Set up fraud alerts
description: This topic explains how to set up rules to alert customer service representatives of potentially fraudulent information when orders are processed. You can define specific codes to use to automatically or manually put suspicious orders on hold.
author: josaw1
manager: AnnBe
ms.date: 2016-04-07 19 - 45 - 58
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations
ms.custom: 79103
ms.assetid: e342af8d-7498-4d20-8483-ab368429c578
ms.search.region: global
ms.search.industry: Retail
ms.author: josaw
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 120c37d479d37aed55ed463c71440a10f213c1c7
ms.lasthandoff: 02/22/2017


---

# <a name="set-up-fraud-alerts"></a>Set up fraud alerts

This topic explains how to set up rules to alert customer service representatives of potentially fraudulent information when orders are processed. You can define specific codes to use to automatically or manually put suspicious orders on hold. 

Before you set up and use fraud checking rules, you must enable fraud checking and define the basic fraud checking values in the call center parameters. There are two types of fraud rules:

-   **Static rules** use a specific value, such as a phone number that has been blacklisted.
-   **Dynamic rules** can be composed from variables and conditions.

Before you create a dynamic rule, you must create the variables and conditions that define who the rule applies to and when the rule should be applied. For example, you want to create a rule to require that any sales order that customer 1202 places that is worth 1,000.00 or more be put on hold until the customer payment can be verified. In this case, the variables are customer 1202 and an order total of 1,000.00. The condition specifies that if customer 1202 places an order, and the total amount of the order is equal to or more than 1,000.00, the sales order must be put on hold until the customer payment can be verified.


