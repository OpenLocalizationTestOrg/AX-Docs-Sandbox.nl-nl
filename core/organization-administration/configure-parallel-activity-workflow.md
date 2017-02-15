---
title: Configure a parallel activity in a workflow | Microsoft Docs
description: To configure a parallel activity, complete the following procedures in the workflow editor.
author: sericks007
manager: AnnBe
ms.date: 2016-09-30 15:56:21
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User, IT Pro
ms.reviewer: 71
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 195753
ms.assetid: 7aa762ce-dd7c-436c-ab66-348334938f2a
ms.region: Global
ms.author: donaldc
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: 1fc8e3baa8c94edbd91952484259430331bd628d


---

# <a name="configure-a-parallel-activity-in-a-workflow"></a>Configure a parallel activity in a workflow

To configure a parallel activity, complete the following procedures in the workflow editor.

A parallel activity consists of workflow branches that run at the same time.

## <a name="name-a-parallel-activity"></a>Name a parallel activity
Follow these steps to enter a name for a parallel activity.
1.  Right-click the parallel activity, and then click **Properties** to open the **Properties** form.
2.  In the left pane, click **Basic Settings**.
3.  In the **Name** field, enter a unique name for the parallel activity.
4.  Click **Close**.

## <a name="configure-the-branches-of-a-parallel-activity"></a>Configure the branches of a parallel activity
Follow these steps to add and configure the branches of this parallel activity.
1.  Double-click the parallel activity to display the branches of the parallel activity.
2.  To add a branch, drag the **Branch** element from the **Workflow elements** area to an insertion point on the canvas. The following figure shows an insertion point.![Insertion point](./media/workflow_insertionpoint.gif)
    | **Note**                                                                                                         |
    |------------------------------------------------------------------------------------------------------------------|
    | The order of the branches is not important because all the branches of a parallel activity run at the same time. |

3.  To configure each branch, see [Configure a parallel branch](http://axhelp.dynamics.com/en/wiki/configure-a-parallel-branch/).






<!--HONumber=Feb17_HO3-->


