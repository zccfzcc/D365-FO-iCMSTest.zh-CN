---
title: 监控主计划运行
description: 生产规划员想要查看主计划运行是否在进行中。
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: DefaultDashboard, ReqCreatePlanWorkspace, ReqTransPlanCard, SysQueryForm, InventItemIdLookupSimple, ReqLog, ReqProcessTaskTrace
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 15b1abfd83ae46cef7d3bd4a6cec2b2ae0b3954d
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55302"
---
# <a name="monitor-a-master-planning-run"></a><span data-ttu-id="5ee28-103">监控主计划运行</span><span class="sxs-lookup"><span data-stu-id="5ee28-103">Monitor a master planning run</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="5ee28-104">生产规划员想要查看主计划运行是否在进行中。</span><span class="sxs-lookup"><span data-stu-id="5ee28-104">The production planner wants to see if a master planning run is in progress.</span></span> <span data-ttu-id="5ee28-105">使用演示数据公司 USMF 来完成此过程。</span><span class="sxs-lookup"><span data-stu-id="5ee28-105">Use the demo data company USMF to complete this procedure.</span></span>


## <a name="run-master-planning"></a><span data-ttu-id="5ee28-106">运行主计划</span><span class="sxs-lookup"><span data-stu-id="5ee28-106">Run master planning</span></span>
1. <span data-ttu-id="5ee28-107">单击“主计划”。</span><span class="sxs-lookup"><span data-stu-id="5ee28-107">Click Master planning.</span></span>
    * <span data-ttu-id="5ee28-108">您将在默认仪表板找到此项。</span><span class="sxs-lookup"><span data-stu-id="5ee28-108">You'll find this on the default dashboard.</span></span>  
2. <span data-ttu-id="5ee28-109">在“计划”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="5ee28-109">In the Plan field, enter or select a value.</span></span>
    * <span data-ttu-id="5ee28-110">示例：StaticPlan</span><span class="sxs-lookup"><span data-stu-id="5ee28-110">Example: StaticPlan</span></span>  
3. <span data-ttu-id="5ee28-111">单击“运行”。</span><span class="sxs-lookup"><span data-stu-id="5ee28-111">Click Run.</span></span>
4. <span data-ttu-id="5ee28-112">在“跟踪处理时间”字段中，选择“是”。</span><span class="sxs-lookup"><span data-stu-id="5ee28-112">Select Yes in the Track processing time field.</span></span>
    * <span data-ttu-id="5ee28-113">如果已选择此字段，则跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="5ee28-113">If the field is already selected, skip this step.</span></span>  
5. <span data-ttu-id="5ee28-114">在“线程数”字段中，输入一个数字。</span><span class="sxs-lookup"><span data-stu-id="5ee28-114">In the Number of threads field, enter a number.</span></span>
6. <span data-ttu-id="5ee28-115">扩展“要包括的记录”部分。</span><span class="sxs-lookup"><span data-stu-id="5ee28-115">Expand the Records to include section.</span></span>
7. <span data-ttu-id="5ee28-116">单击“筛选器”。</span><span class="sxs-lookup"><span data-stu-id="5ee28-116">Click Filter.</span></span>
8. <span data-ttu-id="5ee28-117">在列表中，标记所选的行。</span><span class="sxs-lookup"><span data-stu-id="5ee28-117">In the list, mark the selected row.</span></span>
    * <span data-ttu-id="5ee28-118">标记“字段=物料编号”的行。</span><span class="sxs-lookup"><span data-stu-id="5ee28-118">Mark the row where Field = Item number.</span></span>  
9. <span data-ttu-id="5ee28-119">在“标准”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="5ee28-119">In the Criteria field, enter or select a value.</span></span>
    * <span data-ttu-id="5ee28-120">例子： T0001</span><span class="sxs-lookup"><span data-stu-id="5ee28-120">Example: T0001</span></span>  
10. <span data-ttu-id="5ee28-121">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="5ee28-121">Click OK.</span></span>
11. <span data-ttu-id="5ee28-122">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="5ee28-122">Click OK.</span></span>

## <a name="monitor-the-master-planning-run"></a><span data-ttu-id="5ee28-123">监控主计划运行</span><span class="sxs-lookup"><span data-stu-id="5ee28-123">Monitor the master planning run</span></span>
1. <span data-ttu-id="5ee28-124">单击“历史记录”。</span><span class="sxs-lookup"><span data-stu-id="5ee28-124">Click History.</span></span>
2. <span data-ttu-id="5ee28-125">单击“查询”。</span><span class="sxs-lookup"><span data-stu-id="5ee28-125">Click Inquiries.</span></span>
3. <span data-ttu-id="5ee28-126">单击“流程任务持续时间”。</span><span class="sxs-lookup"><span data-stu-id="5ee28-126">Click Process task duration.</span></span>
4. <span data-ttu-id="5ee28-127">在列表中，找到并选择所需记录。</span><span class="sxs-lookup"><span data-stu-id="5ee28-127">In the list, find and select the desired record.</span></span>
    * <span data-ttu-id="5ee28-128">对于每一物料，您可以获取其花费多长时间完成每个计划步骤的概览。</span><span class="sxs-lookup"><span data-stu-id="5ee28-128">For each item you can get an overview of how long it took to complete each planning step.</span></span>  

