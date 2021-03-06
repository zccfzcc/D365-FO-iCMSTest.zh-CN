---
title: 支出报表和多个审核人
description: 此主题介绍需要多人审核的支出报表。
author: saraschi2
manager: AnnBe
ms.date: 02/23/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TrvExpensesReportList
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 0c320a9c9bc41f74d867fa6d0719c95debd2664d
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55902"
---
# <a name="expense-reports-and-multiple-approvers"></a>支出报表和多个审核人

[!include [banner](../includes/banner.md)]

根据您组织的支出审核策略，可能需要多人审核由员工提交的支出报表。 在您设置支出报表审核的工作流程时，可以添加包括一个或多个支出报表审核人的任务或步骤的工作流元素。 例如，您可能需要所有支出报表首先由提交报表的员工经理审核，然后由应付帐款协调员进行审核。

如果您决定需要多个支出报表审核人，您可以添加在以下任何方法中的工作流元素：

- 添加包含一个步骤的一个审核元素。 例如，该步骤可能要求将支出报表分配给用户组，并且由 50% 的用户组成员进行审核。
- 添加包含多个步骤的一个审核元素。 例如，审核元素可能包含以下步骤：

    1. 由提交支出报表的员工经理审核。
    2. 应付帐款职员验证收据和支出报表物料。
    3. 由预算所有者审核支出报表。

- 添加多个审核元素，每个审核元素中包含一个步骤。 例如，您可以为下面的每个步骤添加一个单独的审核元素：

    1. 员工经理审核支出报表。
    2. 由预算所有者审核支出报表。
