---
title: Benefit eligibility policies | Microsoft Docs
description: This article provides information about benefit eligibility policies, which help you define who is eligible for specific benefits.
author: rschloma
manager: AnnBe
ms.date: 2015-12-04 02:16:06
ms.topic: article
ms.prod: 
ms.service: Dynamics365Operations
ms.technology: 
keywords: HcmBenefitEligibilityDetail, SysPolicyListPage, SysPolicySourceDocumentRuleType
audience: Application User
ms.reviewer: rschloma
ms.suite: Released- Dynamics AX 7.0.0
ms.custom: 16441
ms.assetid: 9341c8e9-c37c-473f-b090-6c56d43b0a24
ms.region: Global
ms.author: kherr
translationtype: Human Translation
ms.sourcegitcommit: 744ac447b01dee241043ba27e3b1ffdcb0022a1b
ms.openlocfilehash: a65c82f8877ae458df15d32ce4a44f5a5533524e


---

# <a name="benefit-eligibility-policies"></a>Benefit eligibility policies

This article provides information about benefit eligibility policies, which help you define who is eligible for specific benefits.

When you create benefits, you decide which benefits will be available to which employees. The following table shows examples of benefits that you might make available to specific employees.

| Benefit          | Who the benefit is available to |
|------------------|---------------------------------|
| Health insurance | All employees                   |
| Mobile phone     | Sales staff, executives         |
| Parking passes   | Executives                      |

The following components in are used to create eligibility policies:

-   Policy rule types
-   Benefit eligibility policies

Policy rule types define the query parameters that are used when you develop specific policy rules. After you create policy rule types, you can create benefit eligibility policies. The policies let you create a collection of rules that apply to one or more legal entities. Within each policy, you can view any of the benefit eligibility policy rule types that you created earlier. You define the scope of the rule within the policy. For example, if you create a benefit eligibility policy rule type that is named **Executive**, you can specify what the rule is within that policy. In this example, the rule might state that any job title that contains the word “executive” should be included in the rule. After you've defined the parameters of the rule or rules that are included in the policy, you can assign a specific rule to the benefit.

<a name="see-also"></a>See also
--------

[Defining and managing a benefit program](https://docs.microsoft.com/en-us/dynamics365/operations/human-resources/managing-benefit-program)




<!--HONumber=Feb17_HO3-->


