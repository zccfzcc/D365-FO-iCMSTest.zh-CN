---
title: 创建多个活动的看板规则
description: 此过程演示如何创建包含来自生产流的多个活动的看板规则。
author: ChristianRytt
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: KanbanRules, LeanProductionFlowActivityLookup, KanbanFlowSelection, InventItemIdLookupSimple, KanbanCreateScheduled, Kanban
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: crytt
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 0df1c44897a18fc6ae6da4569af2f4780a1a4ea3
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54951"
---
# <a name="create-a-kanban-rule-for-multiple-activities"></a><span data-ttu-id="d6ce1-103">创建多个活动的看板规则</span><span class="sxs-lookup"><span data-stu-id="d6ce1-103">Create a kanban rule for multiple activities</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="d6ce1-104">此过程演示如何创建包含来自生产流的多个活动的看板规则。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-104">This procedure shows how to create a kanban rule that includes multiple activities from a production flow.</span></span> <span data-ttu-id="d6ce1-105">创建此任务的演示数据公司是 USMF。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-105">The demo data company used to create this task is USMF.</span></span> <span data-ttu-id="d6ce1-106">该任务面向工艺工程师或价值流经理，因为他们负责新型或改良产品的生产准备。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-106">This task is intended for the process engineer or the value stream manager, as they prepare production of a new or modified product in a lean environment.</span></span>


## <a name="create-a-new-kanban-rule"></a><span data-ttu-id="d6ce1-107">创建新看板规则</span><span class="sxs-lookup"><span data-stu-id="d6ce1-107">Create a new kanban rule</span></span>
1. <span data-ttu-id="d6ce1-108">转到“产品信息管理”>“Lean manufacturing”>“看板规则”。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-108">Go to Product information management > Lean manufacturing > Kanban rules.</span></span>
2. <span data-ttu-id="d6ce1-109">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-109">Click New.</span></span>
3. <span data-ttu-id="d6ce1-110">在“补货策略”字段中，选择“已计划”。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-110">In the Replenishment strategy field, select 'Scheduled'.</span></span>
4. <span data-ttu-id="d6ce1-111">在“第一个计划活动”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-111">In the First plan activity field, enter or select a value.</span></span>
    * <span data-ttu-id="d6ce1-112">选择 SpeakerAssemblyAndPolish。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-112">Select SpeakerAssemblyAndPolish.</span></span>  
5. <span data-ttu-id="d6ce1-113">选中“多个活动”复选框。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-113">Select the Multiple activities check box.</span></span>
    * <span data-ttu-id="d6ce1-114">目的是在看板规则中包含多个活动。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-114">The purpose is to include more than one activity in the kanban rule.</span></span> <span data-ttu-id="d6ce1-115">当您选择最后一个计划活动时，您就选择了生产流中的一个路径。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-115">You choose a path in the production flow when you select the last plan activity.</span></span>  
6. <span data-ttu-id="d6ce1-116">在“最后一个计划活动”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-116">In the Last plan activity field, enter or select a value.</span></span>
    * <span data-ttu-id="d6ce1-117">选择 SpeakerTestAndPackaging。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-117">Select SpeakerTestAndPackaging.</span></span> <span data-ttu-id="d6ce1-118">选择值之后，将自动打开一个页面。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-118">After you select the value, a page automatically opens.</span></span> <span data-ttu-id="d6ce1-119">选择看板流 SpeakerAssemblyAndPolish > SpeakerTestAndPackaging。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-119">Select the kanban flow SpeakerAssemblyAndPolish > SpeakerTestAndPackaging.</span></span> <span data-ttu-id="d6ce1-120">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-120">Click OK.</span></span>  
7. <span data-ttu-id="d6ce1-121">展开“详细信息”部分。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-121">Expand the Details section.</span></span>
8. <span data-ttu-id="d6ce1-122">在“产品”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-122">In the Product field, enter or select a value.</span></span>
    * <span data-ttu-id="d6ce1-123">选择物料 L0006。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-123">Select Item L0006.</span></span>  

## <a name="create-kanban-and-view-jobs"></a><span data-ttu-id="d6ce1-124">创建看板和查看作业</span><span class="sxs-lookup"><span data-stu-id="d6ce1-124">Create kanban and view jobs</span></span>
1. <span data-ttu-id="d6ce1-125">展开“看板”部分。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-125">Expand the Kanbans section.</span></span>
2. <span data-ttu-id="d6ce1-126">单击“添加”。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-126">Click Add.</span></span>
3. <span data-ttu-id="d6ce1-127">在“新看板数”字段中输入“1”。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-127">In the Number of new kanbans field, enter '1'.</span></span>
    * <span data-ttu-id="d6ce1-128">这将创建一个看板。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-128">This will create one kanban.</span></span>  
4. <span data-ttu-id="d6ce1-129">将产品数量设置为“3”。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-129">Set Product quantity to '3'.</span></span>
    * <span data-ttu-id="d6ce1-130">看板将处理 3 个产品。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-130">Kanban will process 3 products.</span></span>  
5. <span data-ttu-id="d6ce1-131">在“到期日期/时间”字段中输入日期和时间。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-131">In the Due date/time field, enter a date and time.</span></span>
    * <span data-ttu-id="d6ce1-132">可以输入“今天”。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-132">You can enter Today.</span></span>  
6. <span data-ttu-id="d6ce1-133">单击“创建”。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-133">Click Create.</span></span>
7. <span data-ttu-id="d6ce1-134">单击“详细信息”。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-134">Click Details.</span></span>
    * <span data-ttu-id="d6ce1-135">请注意，此看板有两个来自生产流的处理作业。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-135">Notice that the kanban has two process jobs from the production flow.</span></span> <span data-ttu-id="d6ce1-136">第一个是 SpeakerAssemblyAndPolish，第二个是 SpeakerTestAndPackaging。</span><span class="sxs-lookup"><span data-stu-id="d6ce1-136">The first one is SpeakerAssemblyAndPolish, and the second one is SpeakerTestAndPackaging.</span></span>  
    * <span data-ttu-id="d6ce1-137">这是最后一个步骤！</span><span class="sxs-lookup"><span data-stu-id="d6ce1-137">This is the last step!</span></span>  

