---
title: 输入和比较询价出价并授予合同
description: 此过程显示您如何输入给询价的回复，以及如何对出价评分和比较出价，然后将出价授予某一供应商。
author: mkirknel
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: PurchRFQCaseTableListPage, PurchRFQCaseTable, PurchRFQReplyTable, PurchRFQCompare, PurchRFQEditLines, PurchRFQEditLinesParameters, PurchTable
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mkirknel
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 333371f7736ae8591d65c6e613057d34b5716c90
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "53322"
---
# <a name="enter-and-compare-rfq-bids-and-award-contracts"></a>输入和比较询价出价并授予合同

[!include [task guide banner](../../includes/task-guide-banner.md)]

此过程显示您如何输入给询价的回复，以及如何对出价评分和比较出价，然后将出价授予某一供应商。 您可以在演示数据公司 USMF 中使用此过程。 在您开始前，您必须有具有至少发送给两个供应商的两个行的询价。 您可以运行“创建询价”过程作为创建此询价的先决条件。 您需要先设置计分条件才能运行此过程。


## <a name="enter-a-reply-from-a-vendor"></a>输入供应商的回复
1. 转到“采购”>“询价”>“所有询价”。
2. 选择具有“已发送”状态的询价，并单击询价案例编号上的链接。
    * 应已发送询价到至少 2 个供应商。  
3. 单击“抬头”转到供应商列表。
4. 选择您要在询价中为其输入响应的供应商。
5. 单击“输入回复”。
6. 在“操作”窗格上，单击“回复”。
7. 单击“将数据复制到回复”。
    * 此操作将复制所选的数据，例如，从询价案例到询价回复的数量。 您也可以跳过此操作，并在编辑回复时手动填写所有响应字段。  
8. 单击“编辑”。
9. 在“单位价格”字段中，输入一个数字。
10. 选择其他报价单行。
11. 在“单位价格”字段中，输入一个数字。

## <a name="score-the-bid"></a>为出价评分
1. 单击“抬头”转到出价评分。
2. 扩展“出价评分”部分。
3. 在“分数”字段中，为一个计分条件输入数字。
    * 如果您悬停在一个计分条件上，工具提示将显示您必须计分的范围。 在此演示中，您可以添加 1 和 5 之间的数字到任何条件。  
4. 选择另一个计分条件。
5. 在“分数”字段中输入数字。
6. 扩展“调查表”部分。
    * 如果询价案例具有发送到供应商的调查表，您可以在调查表部分中输入他们的响应。  
7. 关闭该页面。

## <a name="enter-a-reply-for-another-vendor"></a>输入其他供应商的回复
1. 通过清除您刚才为其输入回复的供应商，然后选择下一个供应商行来选择下一个供应商。
2. 在列表中，找到并选择所需记录。
3. 单击“输入回复”。
4. 单击“将数据复制到回复”。
5. 单击“编辑”。
6. 在“单位价格”字段中，输入一个数字。
7. 选择其他报价单行。
8. 在“单位价格”字段中，输入一个数字。

## <a name="score-the-second-bid"></a>为第二个出价评分
1. 单击“抬头”转到出价评分。
2. 在“分数”字段中输入数字。
3. 在列表中，找到并选择所需记录。
4. 在“分数”字段中输入数字。

## <a name="compare-the-replies"></a>比较回复
1. 在操作窗格上，单击“常规”。
2. 单击“比较回复”。
3. 在“排名”字段中输入数字。
    * 此页显示具有标头和行的出价，以及标头级别的总分。 您可以通过在网格中排序对行进行比较，以便可比较的行相互相邻排列。 信息还包括：数量：供应商报价的数量。 此数量可能不等于在 RFQ 中指定的数量。   净额：供应商的询价，在减去所有折扣后，针对行上的物料。   偏差：投标标题或行的交货日期与询价标题或行所要求的交货日期之间偏差的天数。   您可以为每个出价输入排名。  
4. 选择要排名的其他出价的抬头行。
5. 在“排名”字段中输入数字。
6. 单击“保存”。

## <a name="reject-a-bid"></a>拒绝出价
1. 选择要拒绝的出价的抬头行。
    * 每次每个出价内只能接受、拒绝或返回一个出价或行。  
2. 选择“标记”复选框。
    * 如果您在出价的抬头上选中“标记”复选框，那么所有行也将被标记。 您还可以选择标记出价内行的子集以拒绝或接受它们。 您可以接受询价的有些行的一个供应商出价，然后将其他询价行授予不同的供应商，但是，您需要在 2 个步骤中执行此操作，一次一个出价。 如果存在替换行，则您可以只接受原始投标行或替换行，但不能同时接受两个。  
3. 单击“拒绝”。
4. 单击“参数”以打开下拉对话框。
5. 在“拒绝原因”字段中，输入或选择一个值。
    * 拒绝原因将存储在回复中。  
6. 单击“确定”。
7. 单击“确定”。
8. 关闭该页面。
9. 关闭该页面。
10. 刷新该页面。

## <a name="accept-a-bid"></a>接受出价
1. 选择要接受的出价，然后单击“询价”字段中的链接。
2. 在“操作”窗格上，单击“回复”。
3. 单击“接受”。
    * 如果标记了特定行而不是其他行，那么接受操作将只包括标记的行。 如果要接受出价的所有行，那么您不必标记这些行。  
4. 单击“参数”以打开下拉对话框。
    * 这允许您记录接受出价的原因。 原因将存储在出价中。  
5. 在“接受原因”字段中，输入或选择一个值。
6. 单击“确定”。
7. 单击“确定”。
    * 在单击“确定”后，这将基于在询价接受中包括的行生成采购订单。 如果存在其他尚未处理的出价（已接受、已拒绝或已返回），那么系统将提示您拒绝其余出价。  

## <a name="view-the-purchase-order-thats-been-generated"></a>查看已生成的采购订单
1. 在操作窗格上，单击“常规”。
2. 单击“采购订单”。
    * 在这里您可以查看接受出价时生成的采购订单。  
3. 关闭该页面。
4. 关闭该页面。
5. 关闭该页面。
6. 关闭该页面。

