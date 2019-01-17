---
title: 创建站点计划
description: 此过程显示如何计划没有为站点开始的生产订单。
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProdTableListPage, ProdSchedule, ProdRouteJob
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 6b680929daf6604365cb94d77c19b0843c005cb5
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56439"
---
# <a name="create-a-schedule-for-a-site"></a><span data-ttu-id="4d19b-103">创建站点计划</span><span class="sxs-lookup"><span data-stu-id="4d19b-103">Create a schedule for a site</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="4d19b-104">此过程显示如何计划没有为站点开始的生产订单。</span><span class="sxs-lookup"><span data-stu-id="4d19b-104">This procedure shows how to schedule production orders that are not yet started for a site.</span></span>  <span data-ttu-id="4d19b-105">演示数据公司 USMF 用于完成此过程。</span><span class="sxs-lookup"><span data-stu-id="4d19b-105">The demo data company USMF is used to complete this procedure.</span></span>


## <a name="identify-production-orders-that-are-not-started"></a><span data-ttu-id="4d19b-106">确定未开始的生产订单</span><span class="sxs-lookup"><span data-stu-id="4d19b-106">Identify production orders that are not started</span></span>
1. <span data-ttu-id="4d19b-107">转到“生产控制”>“生产订单”>“全部生产订单”。</span><span class="sxs-lookup"><span data-stu-id="4d19b-107">Go to Production control > Production orders > All production orders.</span></span>
2. <span data-ttu-id="4d19b-108">使用“快速筛选器”以查找记录。</span><span class="sxs-lookup"><span data-stu-id="4d19b-108">Use the Quick Filter to find records.</span></span> <span data-ttu-id="4d19b-109">例如，使用值“1”在“站点”字段中进行筛选。</span><span class="sxs-lookup"><span data-stu-id="4d19b-109">For example, filter on the Site field with a value of '1'.</span></span>
    * <span data-ttu-id="4d19b-110">1 表示 USMF 中的站点。</span><span class="sxs-lookup"><span data-stu-id="4d19b-110">1 represents a site in USMF.</span></span> <span data-ttu-id="4d19b-111">如果您不使用 USMF，请选择您公司的站点。</span><span class="sxs-lookup"><span data-stu-id="4d19b-111">If you are not using USMF, select a site from your own company.</span></span>  
3. <span data-ttu-id="4d19b-112">打开状态列筛选器。</span><span class="sxs-lookup"><span data-stu-id="4d19b-112">Open the Status column filter.</span></span>
4. <span data-ttu-id="4d19b-113">使用“正好是”筛选器运算符将筛选器应用于值为“已计划”的“状态”字段。</span><span class="sxs-lookup"><span data-stu-id="4d19b-113">Apply a filter on the "Status" field, with a value of "Scheduled", using the "is exactly" filter operator.</span></span>

## <a name="create-a-schedule"></a><span data-ttu-id="4d19b-114">创建计划</span><span class="sxs-lookup"><span data-stu-id="4d19b-114">Create a schedule</span></span>
1. <span data-ttu-id="4d19b-115">在列表中，标记或取消标记所有行。</span><span class="sxs-lookup"><span data-stu-id="4d19b-115">In the list, mark or unmark all rows.</span></span>
2. <span data-ttu-id="4d19b-116">在“操作窗格”上，单击“计划” 。</span><span class="sxs-lookup"><span data-stu-id="4d19b-116">On the Action Pane, click Schedule.</span></span>
3. <span data-ttu-id="4d19b-117">单击“计划作业”。</span><span class="sxs-lookup"><span data-stu-id="4d19b-117">Click Schedule jobs.</span></span>
4. <span data-ttu-id="4d19b-118">在“计划的方向”字段中，选择“从交货日期倒推”。</span><span class="sxs-lookup"><span data-stu-id="4d19b-118">In the Scheduling direction field, select 'Backward from delivery date'.</span></span>
5. <span data-ttu-id="4d19b-119">在“有限产能”字段中选择“否”。</span><span class="sxs-lookup"><span data-stu-id="4d19b-119">Select No in the Finite capacity field.</span></span>
6. <span data-ttu-id="4d19b-120">在“有限物料”字段中，选择“否”。</span><span class="sxs-lookup"><span data-stu-id="4d19b-120">Select No in the Finite material field.</span></span>
7. <span data-ttu-id="4d19b-121">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="4d19b-121">Click OK.</span></span>
    * <span data-ttu-id="4d19b-122">这可能需要花费一段时间。</span><span class="sxs-lookup"><span data-stu-id="4d19b-122">This may take a while.</span></span>  

## <a name="view-the-result-of-scheduled-production-orders"></a><span data-ttu-id="4d19b-123">查看已计划生产订单的结果</span><span class="sxs-lookup"><span data-stu-id="4d19b-123">View the result of scheduled production orders</span></span>
1. <span data-ttu-id="4d19b-124">在列表中，标记所选的行。</span><span class="sxs-lookup"><span data-stu-id="4d19b-124">In the list, mark the selected row.</span></span>
    * <span data-ttu-id="4d19b-125">您可以标记任何行。</span><span class="sxs-lookup"><span data-stu-id="4d19b-125">You can mark any row.</span></span>  
2. <span data-ttu-id="4d19b-126">在操作窗格上单击“生产订单”。</span><span class="sxs-lookup"><span data-stu-id="4d19b-126">On the Action Pane, click Production order.</span></span>
3. <span data-ttu-id="4d19b-127">单击“所有作业”。</span><span class="sxs-lookup"><span data-stu-id="4d19b-127">Click All jobs.</span></span>
    * <span data-ttu-id="4d19b-128">在此页，您可以查看工作列表。</span><span class="sxs-lookup"><span data-stu-id="4d19b-128">On this page, you can see the list of jobs.</span></span> <span data-ttu-id="4d19b-129">在”计划“选项卡上，您可以查看作业的开始日期和结束日期。</span><span class="sxs-lookup"><span data-stu-id="4d19b-129">On the Scheduling tab, you can see the Start date and End date for a job.</span></span>  
4. <span data-ttu-id="4d19b-130">单击“物料”。</span><span class="sxs-lookup"><span data-stu-id="4d19b-130">Click Materials.</span></span>
    * <span data-ttu-id="4d19b-131">在此页，您可以查看生产订单中操作的估计物料消耗量和当前可用库存。</span><span class="sxs-lookup"><span data-stu-id="4d19b-131">On this page, you can see the estimated material consumption for the operations on the production order and the current available inventory.</span></span>  
