---
title: 福利资格策略
description: 本文提供有关福利资格策略的信息，可帮助您定义哪些人有资格享受特定福利。
author: rschloma
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-talent
ms.technology: ''
ms.search.form: HcmBenefitEligibilityDetail, SysPolicyListPage, SysPolicySourceDocumentRuleType
audience: Application User
ms.reviewer: rschloma
ms.search.scope: Core, Operations, Talent
ms.custom: 16441
ms.assetid: 4ad0106f-5b07-4fd5-bc1a-5834fa9b198e
ms.search.region: Global
ms.author: kherr
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Talent July 2017 update
ms.openlocfilehash: 5394984ad2135538a693dd8f91f898083b9b8e97
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "60163"
---
# <a name="benefit-eligibility-policies"></a>福利资格策略

[!include [banner](includes/banner.md)]

本主题提供有关福利资格策略的信息，可帮助您定义哪些人有资格享受特定福利。

在您创建福利时，您决定哪些福利可用于哪些员工。 下表显示您可以使其用于特定员工的福利示例。

| 福利          | 福利可用于谁 |
|------------------|---------------------------------|
| 健康保险 | 所有员工                   |
| 移动电话     | 销售员工、主管人员         |
| 停车证   | 主管人员                      |

以下组件用于创建资格策略：

-   政策规则类型
-   福利资格策略

策略规则类型定义开发具体政策规则时所使用的查询参数。 在您创建政策规则类型后，您可以创建福利资格策略。 策略可以创建适用于一个或多个法人的规则集合。 在每个策略中，您可以查看您之前创建的任何福利资格策略规则类型。 

您定义策略中的规则范围。 例如，如果，您创建一个名为**主管人员**的福利资格政策规则类型，您可以指定在该策略中有哪些规则。 在此示例中，规则可能规定包含字词“主管人员”的任何职务都应包括该规则内。 在您定义规则的参数或在策略包括的规则后，可以将一个特定规则分配到福利。

<a name="additional-resources"></a>其他资源
--------

[定义和管理福利计划](manage-benefit-program.md)



