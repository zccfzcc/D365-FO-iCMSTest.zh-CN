---
title: 设置采购类别层次结构
description: 该过程会显示如何在采购类别层次结构中创建新节点，以及如何配置采购类别以用于采购流程。
author: mkirknel
manager: AnnBe
ms.date: 11/06/2017
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Operations
ms.search.region: Global
ms.author: mkirknel
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 24fe482b089cbb0c526cc433e5ab0511671114a5
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "53844"
---
# <a name="set-up-a-procurement-category-hierarchy"></a>设置采购类别层次结构

[!include [task guide banner](../../includes/task-guide-banner.md)]

该过程会显示如何在采购类别层次结构中创建新节点，以及如何配置采购类别以用于采购流程。 这些任务通常由采购经理完成。 在您开始该过程之前，采购类型层次结构必须存在。 如果您正在使用公司演示数据，则您可以在 USMF 公司中执行该过程。


## <a name="add-a-new-procurement-category"></a>添加新采购类别
1. 转到采购>采购目录。 
2. 单击“编辑类别层次结构”。
    * 当前采购类别层次结构会显示在页左侧。 您即将修改该层次结构。  
3. 单击“新类别节点”。
    * 系统会默认选择顶端节点。 如果您正在运行该过程以作为任务指南，您可以单击“解除锁定”按钮，并选择另一个父节点，以插入您的新节点。 一旦完成此项操作，再次锁定任务指南，然后单击“新类别节点”。  
4. 在“名称”字段中，键入一个值。
5. 在“描述”字段中，键入一个值。
6. 在“易记名称”字段中，键入一个值。
    * 易记名称是可选的。 它将连同类别名称一起显示在类别查找中。  
7. 单击“保存”。

## <a name="add-products-to-your-new-procurement-category"></a>添加产品到您的新采购类别
1. 转到采购>采购目录。 
    * 选择您刚添加的节点。 如果您正在运行该过程以作为任务指南，您可能需要解除任务指南锁定，以选择节点。  
2. 切换“产品”部分的展开项。
3. 单击“添加”以关联产品和采购类别。
4. 选择您想要添加到采购类别的产品。
5. 单击箭头以选择产品。
6. 选择要添加到采购类别的另一个产品。
7. 单击箭头以选择产品。
8. 单击“确定”。

## <a name="add-approved-and-preferred-vendors"></a>添加核准供应商和首选供应商
1. 切换供应商部分的扩展。
2. 单击“添加”。
    * 您可以添加一个供应商到采购类别，并指定供应商是否为该类别的首选供应商或只是核准供应商。 在您从某一类别中删除某一供应商时，类别中该供应商的历史交易记录不会被删除。   
3. 查找您想要添加到该采购类别的供应商。
4. 单击箭头以选择供应商。
5. 单击“确定”。
6. 选择您想要修改的供应商行。
7. 在“供应商状态”字段中，选择一个选项。
    * 类别策略规则中的供应商选择设置会管制采购申请上的所有供应商是否为首选、核准或可用供应商。   

## <a name="add-additional-information-to-the-category"></a>添加附加信息到该类别
1. 切换“供应商评估条件组”部分的展开项。
    * 此选项卡可使您定义该采购类别中的供应商应根据什么标准进行评级。 为此，您可以单击“添加”，然后选择一个包含您想要条件的供应商评估组。  
2. 切换“调查问卷”部分的展开项。
    * 此选项卡可使您添加将在申请中显示的调查问卷，只要您将“活动类型”设置为“申请”。 然后，申请者必须填写调查问卷，从而才能提交关于该采购类别中特定产品的申请。  
3. 切换物料销售税组部分的展开项。
4. 在“物料销售税组”字段中，单击下拉按钮以打开查找。
5. 选择增值税组。
6. 切换“类别页”部分的展开项。
    * 可在类别层次结构页中创建类别页。 它们包含关于采购类别的信息（例如关于类别中的产品类型信息）、类别中的产品图形或通告（例如类别中可用的折扣）。 某个类别页中的信息会显示在采购申请上。  
7. 关闭该页面。

