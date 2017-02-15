---
title: Set up extended logon functionality for Cloud POS and MPOS | Microsoft Docs
description: This wiki covers your options for setting up extended logon for Cloud POS and Retail Modern POS (MPOS).
author: josaw1
manager: AnnBe
ms.date: 2016-06-15 20:44:32
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
audience: Application User
ms.reviewer: 41
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 92353
ms.assetid: 52786e1e-2ba3-4c3c-bff4-11ab300b6a03
ms.region: global
ms.industry: Retail
ms.author: rubendel
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: b921d3beaa6bd948b2e828c8927e5d0cb374ac8f


---

# <a name="set-up-extended-logon-functionality-for-cloud-pos-and-mpos"></a>Set up extended logon functionality for Cloud POS and MPOS

This wiki covers your options for setting up extended logon for Cloud POS and Retail Modern POS (MPOS).

<a name="setting-up-extended-logon"></a>Setting up extended logon
=========================

You can find the setup for bar code masks at **Retail and commerce** &gt; **Channel setup** &gt; **POS setup** &gt; **POS profiles** &gt; **Functionality profiles**. The **Functions** FastTab includes the following options that are related to extended logon.

### <a name="staff-bar-code-logon"></a>Staff bar code logon

When the **Staff bar code logon** option is enabled, workers who have an extended logon assigned to their point of sale (POS) credentials can log on by using a bar code.

### <a name="staff-bar-code-logon-requires-password"></a>Staff bar code logon requires password

When the **Staff bar code logon requires password** option is enabled, the staff bar code logon selects only the worker who is assigned to the extended logon that is presented. Workers must still enter their password when this option is enabled.

### <a name="staff-card-logon"></a>Staff card logon

When the **Staff card logon** option is enabled, workers who have an extended logon assigned to their POS credentials can log on by using a magnetic stripe.

### <a name="staff-card-logon-requires-password"></a>Staff card logon requires password

When the **Staff card logon requires password** option is enabled, the staff card logon selects only the worker who is assigned to the extended logon that is presented. Workers must still enter their password when this option is enabled.

<a name="assigning-an-extended-logon"></a>Assigning an extended logon
===========================

By default, only managers can assign extended logon to workers. To assign extended logon, go to **Extended log on** in POS. Then search for a worker by entering his or her operator ID in the search field. Select the worker, and then click **Assign**. On the next page, swipe or scan the extended logon to assign to the worker. If the swipe or scan is successfully read, the **OK** button becomes available. Click **OK** to save the extended logon for that worker.

<a name="deleting-an-extended-logon"></a>Deleting an extended logon
==========================

To delete the extended logon that is assigned to a worker, search for the worker by using the **Extended log on** operation. Select the worker, and then click **Unassign**. All extended logon credentials that are associated with that worker are removed.

<a name="extending-extended-logon"></a>Extending extended logon
========================

The logon service can be extended to support additional extended logon devices, such as palm scanners. For more information, see the POS extensibility documentation.

<a name="using-extended-logon"></a>Using extended logon
====================

When extended logon is configured, and a worker has been assigned a bar code or magnetic stripe, the worker just has to swipe or scan his or her card while the POS logon page is displayed. If a password is also required before logon can proceed, the worker is prompted to enter his or her password.




<!--HONumber=Feb17_HO3-->


