---
title: Configure a parallel activity in a workflow
description: To configure a parallel activity, complete the following procedures in the workflow editor.
author: sericks007
manager: AnnBe
ms.date: 2016-09-30 15 - 56 - 21
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User, IT Pro
ms.search.scope: AX 7.0.0, Operations, Core
ms.custom: 195753
ms.assetid: 6d0656df-b5af-4001-96e6-6f0fcc44d022
ms.search.region: Global
ms.author: donaldc
ms.dyn365.ops.intro: 01-02-2016
ms.dyn365.ops.version: AX 7.0.0
translationtype: Human Translation
ms.sourcegitcommit: b97d17ceabfd25c52c5f0c1e96a123bae6941c5a
ms.openlocfilehash: b12d9bdaf8761f271755958c6f7d925641da029d
ms.lasthandoff: 02/22/2017


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




