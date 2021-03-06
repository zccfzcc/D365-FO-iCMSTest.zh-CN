---
title: 创建使用询价的申请
description: 此指南演示如何将价格和供应商信息添加到询价流程的采购申请。
author: mkirknel
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: PurchReqTableListPage, PurchReqCreate, PurchReqTable, PurchReqLineRelatedDocuments, EcoResCategorySingleLookup, PurchReqWorkflowDropDialog, WorkflowSubmitDialog, WorkflowStatus, WorkflowWorkItemActionDialog, WorkflowUserListLookup, PurchReqCopyRFQ, SysDataAreaSelectLookup, PurchRFQCaseTable, PurchRFQEditLines, PurchRFQReplyTable, UnitOfMeasureLookup
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mkirknel
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: e30473f77eb469a6a67299a9da220eb24f998a00
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55068"
---
# <a name="create-a-requisition-that-uses-an-rfq"></a>创建使用询价的申请

[!include [task guide banner](../../includes/task-guide-banner.md)]

此指南演示如何将价格和供应商信息添加到询价流程的采购申请。 可以在 USMF 演示数据公司中使用此指南中显示的示例，并且必须以 Admin 身份登录才能完成所有任务。 此指南中的任务通常由采购专业人员完成。


## <a name="create-a-requisition"></a>创建申请
1. 转到“采购”>“采购申请”>“由我起草的采购申请”。
2. 单击“新建”。
3. 在“名称”字段中，键入一个值。
4. 在“请求日期”字段中，输入一个日期。
5. 在“会计结算日期”字段中，输入一个日期。
6. 单击“确定”。
7. 在“原因”字段中，输入或选择一个值。
8. 单击“添加行”。
9. 在“采购类别”字段中，选择树中的类别，然后单击“确定”。
10. 在“产品名称”字段中，键入一个值。
11. 在“数量”字段中，输入一个数字。
12. 在“单位”字段中，输入或选择一个值。
13. 单击“保存”。
14. 单击“工作流程”以打开下拉对话框。
15. 单击“提交”。
16. 关闭该页面。
17. 单击“提交”。

## <a name="reassign-a-workflow-task"></a>为工作流重新分配任务
    * 下一项任务是创建询价以获取供应商对产品的出价。 在 USMF 演示数据中，为申请工作流设置了规则，以便在未选择供应商或某行的单价为 0 时，为特定工作人员分配任务以创建询价。 要继续完成此指南，需要将该任务重新分配给其他用户（您自己）。 仅当您以 Admin 身份登录时，才能执行此操作。  
1. 单击“工作流程”以打开下拉对话框。
2. 单击“查看历史记录”。
3. 刷新该页面。
4. 展开“跟踪详细信息”部分。
5. 在树中，请选择以“行工作流启用于”开始的行。
6. 单击“查看工作流详细信息”。
7. 展开“工作项”部分。
8. 单击“重新分配”。
9. 在“用户”字段中，选择“Admin”。
10. 单击“重新分配”。
11. 关闭该页面。
12. 关闭该页面。

## <a name="create-an-rfq"></a>创建询价
1. 刷新该页面。
2. 单击“询价”。
3. 在“购买法人”字段中，选择 USMF。
    * 必须选择位于申请行中的同一个法人。  
4. 在列表中，标记所选的行。
    * 如果采购申请中有多行，请选择要添加到询价的所有行。  
5. 单击“确定”。
6. 刷新该页面。
7. 打开速见表，然后展开“相关单据”部分。
    * 您可能已经打开了该速见表。 在“行/标题”切换按钮右侧找到带箭头的图标。 如果箭头指向右侧，说明速见表已打开。 如果箭头指向左侧，请单击该箭头打开速见表。  
8. 单击“询价”字段中的链接打开刚才创建的询价。
9. 单击“单头”。
10. 单击“添加”。
11. 在“供应商帐户”字段中，输入或选择一个值。
12. 单击“添加”。
13. 在“供应商帐户”字段中，输入或选择一个值。
14. 单击“发送”。
15. 单击“确定”。
16. 单击“输入回复”。
17. 在“操作”窗格上，单击“回复”。
18. 单击“将数据复制到回复”。
    * 这将把数量和日期之类数据从询价复制到回复。  
19. 在“单位价格”字段中，输入一个数字。
    * 这是您从供应商处收到的价格。 您可能还希望输入供应商提供的其他信息。  
20. 单击“接受”。
21. 单击“确定”。

## <a name="verify-that-vendor-and-price-have-been-transferred-to-the-requisition"></a>验证是否已将供应商和价格转移到申请
1. 关闭该页面。
2. 单击“行”。
3. 单击“相关信息”。
4. 单击“采购申请”。
5. 选择已转移到询价的行。
    * 验证是否已将价格和供应商复制到申请。  
6. 单击“工作流程”以打开下拉对话框。
7. 单击“完成”。
8. 关闭该页面。
9. 单击“完成”。

