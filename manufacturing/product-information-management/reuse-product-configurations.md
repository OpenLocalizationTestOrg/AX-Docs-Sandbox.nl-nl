---
title: Reuse product configurations | Microsoft Docs
description: "You can specify that you want to automatically reuse an existing configuration for a product. Then, when a user has completed a configuration session, the system verifies whether a configuration that matches the user’s selections already exists. If a matching configuration is found, the configuration ID, corresponding bill of materials (BOM), and route are reused."
author: YuyuScheller
manager: AnnBe
ms.date: 2016-10-07 08:36:48
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
keywords: PCProductConfigurationModelDetails
audience: Application User
ms.reviewer: YuyuScheller
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 201813
ms.assetid: 25105f3b-5b18-44db-865c-e141cfdd3f10
ms.region: Global
ms.industry: Manufacturing
ms.author: yuyus
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: 9c575d78d28b637750f2a3f45d855a6c38bbd75b


---

# <a name="reuse-product-configurations"></a>Reuse product configurations

You can specify that you want to automatically reuse an existing configuration for a product. Then, when a user has completed a configuration session, the system verifies whether a configuration that matches the user’s selections already exists. If a matching configuration is found, the configuration ID, corresponding bill of materials (BOM), and route are reused.

<a name="requirements-for-reusing-configurations"></a>Requirements for reusing configurations
---------------------------------------

To enable configurations to be reused, you must specify the following information for the components and attributes on the **Product configuration model details** page:

-   **Components and subcomponents** – On the **General** FastTab, in the **Reuse configurations** field, select **Yes**.
-   **Attributes** – On the **Attributes** FastTab, select the **Include in reuse** option. This option appears only when the related component is enabled for reuse. If you don't select any attributes for reuse, the configuration is always reused, regardless of the user’s selections during a configuration session. The attribute values in the existing configuration must match the user’s selections. For example, if the user selects **Blue** as the color during a configuration session, the system verifies whether an existing configuration of the component has the color blue.

## <a name="resetting-configuration-reuse"></a>Resetting configuration reuse
When you reset configuration reuse, previously created configurations are no longer considered. You might want to reset configuration reuse if the BOM or route was changed, but no related attributes were changed. You reset configuration reuse on the **General** FastTab for the component.




<!--HONumber=Feb17_HO3-->


