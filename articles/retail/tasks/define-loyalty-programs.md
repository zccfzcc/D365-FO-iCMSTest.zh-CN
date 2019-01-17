---
title: 定义会员计划
description: 此程序会显示如何设置一个带有两个会员层级的会员计划。
author: jashanno
manager: AnnBe
ms.date: 11/14/2017
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Operations, Retail
ms.search.region: Global
ms.search.industry: Retail
ms.author: jashanno
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 22ae4c220d1a6e23d5a38e5b0e90eda99745f4e3
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55952"
---
# <a name="define-loyalty-programs"></a>定义会员计划

[!include [task guide banner](../includes/task-guide-banner.md)]

此程序会显示如何设置一个带有两个会员层级的会员计划。 此程序使用 USRT 演示数据公司。

1. 转至“零售和商业”> >“会员计划”。
2. 单击“新建”。
3. 在“名称”字段中，键入一个值。
4. 在“描述”字段中，键入一个值。
5. 单击“添加行”。
6. 在“水平”字段，输入一个数值。
7. 在“层”字段中，输入会员层级的名称。
8. 在“描述”字段中，键入一个值。
9. 在“日期区间”字段中，单击下拉按钮以打开查找。
    * 此日期区间应延展到未来。 例如，如果黄金层级选择的日期区间为一年，所有符合该黄金层级的客户可以获得一年分配给该层的奖励。 如果在该层级的客户重新符合黄金层级，则该客户层状态到期日期延伸到另一年，开始日期从客户重新符合黄金层级计算。  
10. 在列表中，单击所选行中的链接。
11. 单击“添加行”。
12. 在“水平”字段，输入一个数字。
13. 在“层”字段中，输入会员层级的名称。
14. 在“描述”字段中，键入一个值。
15. 在“日期区间”字段中，单击下拉按钮以打开查找。
16. 在列表中，单击所选行中的链接。
17. 单击“保存”。
18. 在列表中，找到并选择所需记录。
    * 层级规则定义了在符合该层级的时间内需要获得的最小奖励积分数。  
19. 切换“层规则”部分的扩展项。
20. 单击“新建”。
    * 您可以为每个层级设置多个层级规则。 例如，您可以设置三个不同的条件来获得一个层级：每个月花费 500 美元，一年花费 1000 美元和一年拥有 20 个交易。 为此，您需要创建三个层级规则。  
21. 在“奖励积分”字段中，单击下拉按钮以打开查找。
    * 这应是不可兑换的会员奖励积分。  
22. 在列表中，单击所选行中的链接。
23. 在“发放的最小点数”字段中，输入一个数字。
    * 如果通过参与该计划，所有客户均可轻松符合最低层级，则输入 0。  
24. 在“评估日期区间”字段中，单击下拉按钮以打开查找。
    * 此日期区间应延展到过去。 将仅使用在此日期区间内获得的积分来计算是否达到最小发放积分值。  
25. 在列表中，单击所选行中的链接。
26. 单击“保存”。
27. 在列表中，找到并选择所需记录。
28. 单击“新建”。
29. 在“奖励积分”字段中，单击下拉按钮以打开查找。
30. 在列表中，单击所选行中的链接。
31. 在“发放的最小点数”字段中，输入一个数字。
32. 在“评估日期区间”字段中，单击下拉按钮以打开查找。
    * 此日期区间应延展到过去。  
33. 在列表中，单击所选行中的链接。
34. 单击“保存”。
35. 单击“价格组”。
    * 如果您想要给予会员客户折扣， 您需要将一个或多个价格组分配给会员计划，并将多个价格组分配给折扣。 最佳做法是不要在不同实体类型之间混合价格组。  例如，不要将同一价格组用于会员折扣和渠道折扣。  
36. 在“价格组”字段中，单击下拉按钮以打开查找。
    * 页面顶部价格组链接用于会员计划。 “计划层”快速选项卡中的价格组链接仅供特定会员层级使用。  
37. 在列表中，单击所选行中的链接。
38. 单击“保存”。
39. 关闭该页面。
40. 单击“保存”。
