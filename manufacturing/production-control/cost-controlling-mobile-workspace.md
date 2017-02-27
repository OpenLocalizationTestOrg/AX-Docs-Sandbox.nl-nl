---
title: Cost controlling mobile workspace for Microsoft Dynamics 365 for Operations app
description: With the Cost controlling mobile workspace, cost center managers can see the cost center performance anytime and anywhere.
author: YuyuScheller
manager: AnnBe
ms.date: 2017-01-12 16 - 53 - 04
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: Operations
ms.custom: 267114
ms.assetid: 84740472-494f-444c-9b74-f83b7342fd25
ms.search.region: global
ms.author: yuyus
ms.dyn365.ops.intro: 01-11-2016
ms.dyn365.ops.version: Version 1611
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 3738aab7f5a833f805225a1ed6ce200d092c84dc
ms.lasthandoff: 02/22/2017


---

# <a name="cost-controlling-mobile-workspace-for-microsoft-dynamics-365-for-operations-app"></a>Cost controlling mobile workspace for Microsoft Dynamics 365 for Operations app

With the Cost controlling mobile workspace, cost center managers can see the cost center performance anytime and anywhere. 

<a name="prerequisites"></a>Prerequisites
-------------

| Prerequisite                                                         | Description                                                                                                                                                                   |
|----------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Read about the Microsoft Dynamics 365 for Operations mobile platform | [Dynamics 365 for Operations mobile platform](mobile-platform.md)                                                              |
| Dynamics 365 for Operations                                          | Be sure that you’re using an environment that has Microsoft Dynamics 365 for Operations version 1611 and Microsoft Dynamics for Operations platform update 3 (November 2016). |
| Hotfix KB 3215650                                                    | Install the hotfix to enable the workspaces that are provided in Microsoft Dynamics 365 for Operations.                                                                       |
| Mobile device that has the Dynamics 365 for Operations app installed | Download the Dynamics 365 for Operations app from your mobile app store.                                                                                                      |

## <a name="introduction"></a>Introduction
The Cost controlling mobile workspace provides an instant view of the current performance of cost centers by comparing actual costs against the budgeted costs. You can drill down to statuses of individual cost elements.

### <a name="example"></a>Example

An employee receives an invitation to an international conference. The organization will have to cover all the travel expenses. The employee asks his manger if he can attend the conference. The manager quickly opens the Cost controlling mobile workspace on his mobile phone to see whether he has budget for the employee to attend the conference.

### <a name="data-security"></a>Data security

The data in the Cost controlling workspace is secured by user credentials. A cost center manager is only allowed to see data for his own cost center. The access level security is managed within the Cost accounting module. Cost accountants define the Cost controlling mobile workspace configuration in the Cost accounting module. After the workspace is published to the Microsoft Dynamics 365 for Operations app, it is available in the Dynamics 365 for Operations mobile app. This ensures that all cost center managers in the organization look at data in the same format.

### <a name="actions-views-and-links"></a>Actions, views, and links

The Cost controlling mobile workspace for Dynamics 365 for Operations app provides the following actions, views, and links:

-   Actions 
    -   Select **Configurations** to pick a layout.
    -   Select **Cost objects** to pick the cost centers on which you want filter data. **Note:** The list is displayed according to the access granted in the Cost accounting module.

<!-- -->

-   Based on what is selected under **Actions** and what is configured in the Cost accounting module, you can view the following information in the Cards. Note that the amount is displayed in the same format: Actual, Budget, Variance, and Variance %. 
    -   Actual vs Budget (current period)
    -   Actual vs Revised budget (current period)
    -   Actual vs Budget (previous period)
    -   Actual vs Revised budget (previous period)
    -   Actual vs Budget (year to date)
    -   Actual vs Revised budget (year to date)

<!-- -->

-   Links
    -   Details for current period.
    -   Details for previous period.
    -   Details for year to date.

When you select one of the links, a Card per cost element is displayed. The amount in the Cards is displayed in the following format: Actual, Budget, Budget variance, Budget variance %, Revised budget, Revised budget variance, and Revised budget variance %.  [![cost-controlling](./media/cost-controlling.png)](./media/cost-controlling.png)

## <a name="get-started"></a>Get started
Follow these steps to get started using the cost control mobile app on your mobile device.

1.  On your mobile app store, download and install the Microsoft Dynamics 365 for operations app.
2.  Start the app on your device.
3.  Enter your Dynamics 365 URL.
4.  Enter the company to sign in to. For example, enter **USMF**.
5.  The first time that you sign in, you’re prompted for the user name and password for your Microsoft Dynamics 365 for Operations account. Enter your credentials. After you sign in, you see the available workspaces for your company.

To view workspaces on your mobile app, you must first publish the desired workspaces to the Dynamics 365 for Operations app.

1.  Start Dynamics 365 for Operations.
2.  Go to **System administration** &gt; **Setup** &gt; **system parameters**.
3.  Select **Manage mobile app**.
4.  Select the workspace **Cost controlling **to publish to the mobile platform.
5.  Select **Publish workspace**.
6.  Refresh your device to see the published workspaces.

## <a name="view-the-performance-of-your-cost-center"></a>View the performance of your cost center
1.  On your mobile device, select the **Cost controlling** workspace.
2.  Select **Cost object controlling**.
3.  Click **Actions**.
4.  Click **Select configuration** to select a cost controlling layout.
5.  Click **Done**.
6.  Click **Actions**.
7.  Click **Select cost object** to select the cost centers to which you have been granted access.
8.  Click **Done**.
9.  View the overall performance of your cost center.
10. Click **Details for current period**.
11. View the performance of individual cost elements.
12. You can also search for specific cost elements.



