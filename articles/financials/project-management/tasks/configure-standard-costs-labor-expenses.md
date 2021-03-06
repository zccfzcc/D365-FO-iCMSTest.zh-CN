---
title: 配置人工和支出的标准成本
description: 此过程显示如何为项目的人工和费用设置标准价。
author: KimANelson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProjCostPriceHour, ProjSalesPriceHour, ProjCostPriceExpense, ProjSalesPriceCost
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Service industries
ms.author: knelson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: d6d933b4109ce2d18f06244d136b65d52e2052bb
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "53798"
---
# <a name="configure-standard-costs-for-labor-and-expenses"></a>配置人工和支出的标准成本

[!include [task guide banner](../../includes/task-guide-banner.md)]

此过程显示如何为项目的人工和费用设置标准价。 此任务使用 USSI 数据集。

1. 转至“项目管理与核算 > 设置 > 价格 > 成本价(工时)”。
2. 单击“新建”。
3. 在“有效日期”字段中，输入日期。
4. 在“成本价”字段中，输入一个数字。
    * 可为项目类别设置标准成本价，也可以按照工作人员编号、项目编号、类别、日期以及它们的任何组合来设置成本价。 应用的成本价是最能提供详细信息的成本价。  
5. 单击“保存”。
6. 关闭该页面。
7. 转至“项目管理与核算 > 设置 > 价格 > 销售价(工时)”。
8. 单击“新建”。
9. 在“有效日期”字段中，输入日期。
10. 在“有效”字段中，选择一个选项。
11. 在“定价”字段中输入数字。
    * 可以根据工时交易记录或按项目类别设置标准销售价。 也可以按工作人员编号、项目编号、类别、交易记录日期或其中任一组合设置销售价。 实际销售价是工作人员在“工时”日记帐中输入交易记录时应用的价格，它是具有最高详细级别的销售价。 例如，如果同时设置了一般销售价和工作人员特定的销售价，将使用工作人员特定的销售价。  
12. 单击“保存”。
13. 关闭该页面。
14. 转至“项目管理与核算 > 设置 > 价格 > 销售价(费用)”。
15. 单击“新建”。
16. 在“有效日期”字段中，输入日期。
17. 在“成本价”字段中，输入一个数字。
    * 可以填写多个字段，但是要保存记录，至少必须填写该字段。  
18. 单击“保存”。
19. 关闭该页面。
20. 转至“项目管理与核算 > 设置 > 价格 > 销售价(费用)”。
21. 单击“新建”。
22. 在“有效日期”字段中，输入日期。
23. 在“有效”字段中，选择一个选项。
24. 在“定价”字段中输入数字。
    * 工作人员在费用日记帐凭证中输入交易记录时使用的实际销售价是最详细的销售价。 例如，如果同时设置了日记帐和工作人员特定的销售价，将使用工作人员特定的销售价。  
25. 单击“保存”。

