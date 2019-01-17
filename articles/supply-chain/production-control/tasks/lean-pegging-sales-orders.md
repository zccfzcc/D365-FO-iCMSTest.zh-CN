---
title: 销售订单的精益限定标准
description: 该过程主要为验证看板生产物料的销售行限定标准树形图而设计的。
author: ChristianRytt
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SalesTableListPage, SalesCreateOrder, SalesTable, LeanPeggingTree
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: crytt
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: ec7c1263c23ae8fca1d4c624622fb0f1803733f6
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54502"
---
# <a name="lean-pegging-from-sales-orders"></a><span data-ttu-id="2d985-103">销售订单的精益限定标准</span><span class="sxs-lookup"><span data-stu-id="2d985-103">Lean pegging from sales orders</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="2d985-104">该过程主要为验证看板生产物料的销售行限定标准树形图而设计的。</span><span class="sxs-lookup"><span data-stu-id="2d985-104">This procedure focuses on validating the pegging tree from a sales line where the item is produced with kanbans.</span></span> <span data-ttu-id="2d985-105">在验证限定标准树形图后，所有的看板作业为计划作业。</span><span class="sxs-lookup"><span data-stu-id="2d985-105">After validating the pegging tree, all the kanban jobs are planned.</span></span> <span data-ttu-id="2d985-106">这对订单员需要保证立刻生产的订单方案有用。</span><span class="sxs-lookup"><span data-stu-id="2d985-106">This is useful for order scenarios where the order taker needs to ensure that production can start right away.</span></span> <span data-ttu-id="2d985-107">创建此程序的演示数据公司是 USMF。</span><span class="sxs-lookup"><span data-stu-id="2d985-107">The demo data company used to create this procedure is USMF.</span></span> <span data-ttu-id="2d985-108">该过程目的在于设计精益公司的高级订单员的工作。</span><span class="sxs-lookup"><span data-stu-id="2d985-108">This procedure is intended for the advanced order taker working in a lean company.</span></span>


## <a name="create-a-sales-order-for-a-kanban-controlled-item"></a><span data-ttu-id="2d985-109">创建一个看板管理物料销售订单</span><span class="sxs-lookup"><span data-stu-id="2d985-109">Create a sales order for a kanban controlled item</span></span>
1. <span data-ttu-id="2d985-110">转到“所有销售订单”。</span><span class="sxs-lookup"><span data-stu-id="2d985-110">Go to All sales orders.</span></span>
2. <span data-ttu-id="2d985-111">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="2d985-111">Click New.</span></span>
3. <span data-ttu-id="2d985-112">在“客户帐户”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="2d985-112">In the Customer account field, enter or select a value.</span></span>
    * <span data-ttu-id="2d985-113">使用 US-001。</span><span class="sxs-lookup"><span data-stu-id="2d985-113">Use US-001.</span></span>  
4. <span data-ttu-id="2d985-114">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="2d985-114">Click OK.</span></span>
5. <span data-ttu-id="2d985-115">在“物料编号”字段中，键入“L0001”。</span><span class="sxs-lookup"><span data-stu-id="2d985-115">In the Item number field, type 'L0001'.</span></span>
6. <span data-ttu-id="2d985-116">将“数量”设置为“30”。</span><span class="sxs-lookup"><span data-stu-id="2d985-116">Set Quantity to '30'.</span></span>
    * <span data-ttu-id="2d985-117">数量高于 24 以触发事项看板规则很重要。</span><span class="sxs-lookup"><span data-stu-id="2d985-117">It is important that the quantity is higher than 24 in order to trigger the event kanban rule.</span></span>  

## <a name="open-a-pegging-tree"></a><span data-ttu-id="2d985-118">打开一个限定标准树形图</span><span class="sxs-lookup"><span data-stu-id="2d985-118">Open a pegging tree</span></span> 
1. <span data-ttu-id="2d985-119">单击“产品和供应”。</span><span class="sxs-lookup"><span data-stu-id="2d985-119">Click Product and supply.</span></span>
2. <span data-ttu-id="2d985-120">单击“查看限定标准树”。</span><span class="sxs-lookup"><span data-stu-id="2d985-120">Click View pegging tree.</span></span>
    * <span data-ttu-id="2d985-121">请注意，该限定标准树形图显示的销售订单行限定标准所需的所有级别。</span><span class="sxs-lookup"><span data-stu-id="2d985-121">Notice that the pegging tree shows all levels of the pegging needed for the sales order line.</span></span> <span data-ttu-id="2d985-122">在此案例中，有两个级别的看板和所有必需的组件。</span><span class="sxs-lookup"><span data-stu-id="2d985-122">In this case, there are two levels of kanbans and all the required components.</span></span>  

## <a name="plan-the-pegging-tree"></a><span data-ttu-id="2d985-123">计划该限定标准树形图。</span><span class="sxs-lookup"><span data-stu-id="2d985-123">Plan the pegging tree</span></span>
1. <span data-ttu-id="2d985-124">在该树形图中，选择“销售管线 000832\看板 000558”</span><span class="sxs-lookup"><span data-stu-id="2d985-124">In the tree, select 'Sales line 000832\Kanban 000558'.</span></span>
2. <span data-ttu-id="2d985-125">展开“看板”部分。</span><span class="sxs-lookup"><span data-stu-id="2d985-125">Expand the Kanban jobs section.</span></span>
    * <span data-ttu-id="2d985-126">请注意，该看板作业的作业状态为“未计划”。</span><span class="sxs-lookup"><span data-stu-id="2d985-126">Notice that the job status for the kanban job is Not planned.</span></span>  
3. <span data-ttu-id="2d985-127">单击“计划整个限定标准树形图”。</span><span class="sxs-lookup"><span data-stu-id="2d985-127">Click Plan entire pegging tree.</span></span>
    * <span data-ttu-id="2d985-128">“作业状态”由“未计划”更改为“已计划”，可以在限定标准树形图中计划所有的看板作业。</span><span class="sxs-lookup"><span data-stu-id="2d985-128">This will plan all kanban jobs in the pegging tree, changing the Job status from Not planned to Planned.</span></span>  
4. <span data-ttu-id="2d985-129">刷新该页面。</span><span class="sxs-lookup"><span data-stu-id="2d985-129">Refresh the page.</span></span>
    * <span data-ttu-id="2d985-130">请注意，该看板作业的“作业状态”由“未计划”更改为“已计划”。</span><span class="sxs-lookup"><span data-stu-id="2d985-130">Notice that the kanban Job status changed from Not planned to Planned.</span></span>  
5. <span data-ttu-id="2d985-131">在该树形图中，选择“销售管线 000832\看板 000558\装运 L0001\看板 000559”。</span><span class="sxs-lookup"><span data-stu-id="2d985-131">In the tree, select 'Sales line 000832\Kanban 000558\Issue for L0001\Kanban 000559'.</span></span>
    * <span data-ttu-id="2d985-132">第二个看板作业也为计划作业，因为整个限定标准树形图为计划作业。</span><span class="sxs-lookup"><span data-stu-id="2d985-132">The job for the second kanban is also planned, because the entire pegging tree is planned.</span></span> <span data-ttu-id="2d985-133">请注意，该看板作业状态由“未计划”更改为“已计划”。</span><span class="sxs-lookup"><span data-stu-id="2d985-133">Notice that the kanban job status is changed from Not planned to Planned.</span></span>  

