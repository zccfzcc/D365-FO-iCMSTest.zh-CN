---
title: 创建和编辑销售报价单
description: 该过程演示如何创建和更新销售报价单。
author: omulvad
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SalesQuotationListPage, SalesCreateQuotation, SalesQuotationTable, SalesQuotationTotals, SalesQuotationPriceSimulation, SalesQuotationEditLines, SrsReportViewerForm, smmSetNumSeqIfManual, CustTable, SalesTable
audience: Application User
ms.reviewer: kfend
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: omulvad
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 8dfc343f9f6579a38fb0cf3c6ccc012f9707fda9
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56353"
---
# <a name="create-and-edit-sales-quotations"></a>创建和编辑销售报价单

[!include [task guide banner](../../includes/task-guide-banner.md)]

该过程演示如何创建和更新销售报价单。 您可以使用演示数据公司 USMF 或您自己的数据运行该过程。


## <a name="create-a-sales-quotation"></a>创建销售报价单
1. 转到“销售和市场营销”>“销售报价单”>“所有报价单”。
2. 单击“新建”。
3. 在“帐户类型”字段中，选择“目标客户”。
4. 在“目标客户”字段中，输入或选择一个值。
5. 展开“常规”部分。
    * 由于您选择从“销售和市场营销区域”创建报价单，类型自动设置为“销售报价单”。 若要创建项目报价，必须从“项目管理和会计模块”访问。   
6. 单击“确定”。
    * 报价单行上的字段和操作与销售订单行上的非常类似。   报价单与销售订单一样，在不知道物料编号或在报价单创建过程没有物料编号时可针对特定物料创建，还可针对销售类别创建。  
7. 在“物料”字段中，输入或选择一个值。
8. 在“物料”字段中，键入一个值。
9. 关闭该页面。
10. 在“数量”字段中，输入一个数字。
    * 如果在行上选择该物料的有效贸易协议，适用价格和折扣将会自动复制到报价单行上。 确保“单价”字段含有数值，并且您在想要时还可输入折扣值。  
11. 单击“保存”。
12. 在操作窗格上单击“销售报价单”。
13. 单击“总计”。
14. 单击“确定”。
15. 单击“销售报价单行”。
16. 单击“价格”。
    * 在“运行价格模拟”页，您可以进行试验，根据预期单价、折扣金额、折扣百分比、总金额、毛利或贡献率调整报价单的预期收入或收益率。   在对目标值满意时，应用建议到报价单行中，这会相应更新价格相关的字段。  
    * 您可以任意创建多个价格模拟。 在单击“新建”时，当前报价单行的价格条件会复制到该页面。 然后，您可以修改任何价格相关字段中的值到目标字段中。 任一字段的任何更改会触发所有其他字段的重新计算。 为使系统计算销售毛利和贡献率，必须知道产品的单价。 使用“模拟价格”选项卡，查看原价、建议更改价及其对报价单总价的影响的详细视图。   通常，在设为新金额的模拟价应用于报价单行时，系统重新计算并在“单价”字段输入新的数值。 如果模拟基于新毛利或新贡献率，则仅更新净额字段，且单价字段为空。 在这两种情况下，报价单行上的所有折扣将会在模拟前被删除。  
17. 关闭该页面。
18. 在操作窗格上，单击“报价单”。
19. 单击“发送报价单”。
20. 在“打印报价单”字段中选择“是”。
21. 单击“确定”。
    * 报表的生成可能需要一分钟。 生成报表前不要关闭页面。  
22. 关闭该页面。

## <a name="update-a-sales-quotation"></a>更新销售报价单
1. 在操作窗格上，单击“跟进”。
2. 单击“转换为客户”。
3. 在“客户帐户”字段中，输入一个值。
4. 单击“确认”。
    * 确保您看到消息：您输入的帐号可随意使用。  
5. 单击“确定”。
    * 系统现在为目标客户在报价单上创建了新客户帐户。  
6. 关闭该页面。
7. 在操作窗格上，单击“跟进”。
8. 单击“确认”。
9. 在“原因”字段中，输入或选择一个值。
10. 单击“确定”。
11. 在操作窗格上，单击“常规”。
12. 单击“销售订单”。
13. 关闭该页面。

