---
title: 将固定资产重新分类
description: 若要重新划分固定资产，您必须将固定资产转移到新的固定资产组，或者将新的固定资产编号分配给同一组内的固定资产。
author: saraschi2
manager: AnnBe
ms.date: 10/30/2017
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: f8f73314c3de0cd8f5a0c34a305b84e872ef5899
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56119"
---
# <a name="reclassify-fixed-assets"></a>将固定资产重新分类

[!include [task guide banner](../../includes/task-guide-banner.md)]

若要重新划分固定资产，您必须将固定资产转移到新的固定资产组，或者将新的固定资产编号分配给同一组内的固定资产。 

为某件固定资产重新分类时：

• 为新的固定资产创建现有固定资产的所有价值模型。 为原始固定资产设置的所有信息都复制到新的固定资产。 原始固定资产的价值模型的状态为“已结算”。 

• 新固定资产的新价值模型将在“购置日期”字段中包含重新分类的日期。 “折旧开始日期”字段中的日期从原始资产信息复制。 如果已开始折旧，则“最近计提折旧日期”字段将显示重新分类的日期。 

• 为新的固定资产，取消和生成原始固定资产的现有固定资产交易记录。

1. 转到“固定资产”>“定期任务”>“重新分类”。
2. 在“固定资产组”字段中，选择要重新分类的组。
3. 在“固定资产编号”字段中，选择要重新分类的固定资产。
4. 在“新的固定资产组字段中，选择要将固定资产转移到的组。
    * 如果新固定资产组附加到编号规则，使用来自新固定资产组的编号规则的编号更新“新增固定资产的编号”字段。 否则，使用来自“固定资产参数”页面中设置的编号规则的编号更新“新增固定资产的编号”字段。 如果未在“固定资产参数”页面中设置编号规则，请在“新增固定资产的编号”字段中输入编号。  
5. 在“重新分类日期”字段中，输入一个日期。
6. 在“凭证系列”字段中，输入或选择一个值。
7. 单击“确定”。

