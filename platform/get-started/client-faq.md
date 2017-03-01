---
title: Dynamics 365 for Operations client FAQ
description: This article provides answers to frequently asked questions about the Microsoft Dynamics 365 for Operations client.
author: jasongre
manager: AnnBe
ms.date: 2015-11-04 19 - 47 - 08
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 12334
ms.assetid: a9a57f0e-a67c-46b1-83c9-5d6350fb3b86
ms.search.region: Global
ms.author: jasongre
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: 4baf60aaa0ee3b61840699e509b2a0f88e6d1b78
ms.lasthandoff: 02/22/2017


---

# <a name="dynamics-365-for-operations-client-faq"></a>Dynamics 365 for Operations client FAQ

This article provides answers to frequently asked questions about the Microsoft Dynamics 365 for Operations client.

<a name="why-arent-symbols-loaded-when-i-use-dynamics-365-for-operations"></a>Why aren't symbols loaded when I use Dynamics 365 for Operations?
-----------------------------------------------------------------

The security settings on your browser might prevent the symbols from being loaded correctly. To resolve this issue, try the following steps:

-   If you're experiencing this issue in Internet Explorer, click **Tools**, and then click **Internet Options**.  In the Internet Options dialog box, on the **Privacy** tab, click **Custom level**, and make sure the **Font download** option is selected.
-   Otherwise, you might have to add the Dynamics 365 for Operations site to the list of trusted sites.

## <a name="i-miss-the-ribbon-from-dynamics-ax-2012-can-i-keep-action-pane-tabs-open-all-the-time"></a>I miss the ribbon from Dynamics AX 2012. Can I keep Action Pane tabs open all the time?
We are planning to implement this feature soon. Users will then be able to choose to keep the tabs on Action Panes open all the time. Otherwise, the tabs will be collapsed when they aren't being used, to gain more screen space for the page.

## <a name="why-do-i-sometimes-see-different-shortcut-menus-when-i-rightclick"></a>Why do I sometimes see different shortcut menus when I rightclick?
If you right-click in an editable field (or if text is selected), the browser's shortcut menu is displayed. This menu gives you access to the **Cut**, **Copy**, and **Paste** commands. We can't embed these commands into the Dynamics 365 for Operations shortcut menus because, for security reasons, browsers don’t allow us to programmatically access the system clipboard.

If you right-click a field label or the value of a read-only control, you'll see the Dynamics 365 for Operations shortcut menu.

To make keyboard access easier, we plan to implement a keyboard shortcut in the future that will open the Dynamics 365 for Operations shortcut menu.

## <a name="where-is-the-view-details-functionality-in-dynamics-365-for-operations"></a>Where is the View details functionality in Dynamics 365 for Operations?
The **View details** option is available in a couple of ways:

-   If a control has **View details **capabilities, and if the control has a value, that value is displayed as a hyperlink. You can click the hyperlink to open a page that contains additional details.
-   **View details** is also an option on Dynamics 365 for Operations shortcut menus. For more information about when Dynamics 365 for Operations shortcut menus are displayed when you right-click, see the previous section.



