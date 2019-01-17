---
title: 工作流系统
description: 此主题介绍 Microsoft Dynamics 365 for Finance and Operations 中的工作流系统。
author: sericks007
manager: AnnBe
ms.date: 08/17/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User, IT Pro
ms.reviewer: sericks
ms.search.scope: Core, Operations
ms.custom: 56381
ms.assetid: 20b78595-e1d9-439a-ae1c-a776a3438919
ms.search.region: Global
ms.author: tjvass
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 137f2335c5c2ee12931d3f64bd7b731c5bf4c24f
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56189"
---
# <a name="workflow-system"></a><span data-ttu-id="a8b14-103">工作流系统</span><span class="sxs-lookup"><span data-stu-id="a8b14-103">Workflow system</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="a8b14-104">此主题介绍 Microsoft Dynamics 365 for Finance and Operations 中的工作流系统。</span><span class="sxs-lookup"><span data-stu-id="a8b14-104">This topic describes the workflow system in Microsoft Dynamics 365 for Finance and Operations.</span></span>

<a name="what-is-workflow"></a><span data-ttu-id="a8b14-105">什么是工作流？</span><span class="sxs-lookup"><span data-stu-id="a8b14-105">What is workflow?</span></span>
-----------------

<span data-ttu-id="a8b14-106">术语*工作流*可以通过两种方式定义：作为系统和作为业务流程。</span><span class="sxs-lookup"><span data-stu-id="a8b14-106">The term *workflow* can be defined in two ways: as a system and as a business process.</span></span>
### <a name="workflow-is-a-system"></a><span data-ttu-id="a8b14-107">工作流是一个系统</span><span class="sxs-lookup"><span data-stu-id="a8b14-107">Workflow is a system</span></span>

<span data-ttu-id="a8b14-108">工作流是随 Finance and Operations 一起安装，并且在应用程序对象服务器 (AOS) 上运行的系统。</span><span class="sxs-lookup"><span data-stu-id="a8b14-108">Workflow is a system that is installed with Finance and Operations and runs on the Application Object Server (AOS).</span></span> <span data-ttu-id="a8b14-109">使用工作流系统提供的功能，您可以创建单独的工作流或业务流程。</span><span class="sxs-lookup"><span data-stu-id="a8b14-109">The workflow system provides functionality that you can use to create individual workflows, or business processes.</span></span>

### <a name="workflow-is-a-business-process"></a><span data-ttu-id="a8b14-110">工作流是一个业务流程</span><span class="sxs-lookup"><span data-stu-id="a8b14-110">Workflow is a business process</span></span>

<span data-ttu-id="a8b14-111">“工作流”代表业务流程。</span><span class="sxs-lookup"><span data-stu-id="a8b14-111">A workflow represents a business process.</span></span> <span data-ttu-id="a8b14-112">它通过显示谁必须完成任务、制定决策或批准文档定义单据如何在系统中流动或移动。</span><span class="sxs-lookup"><span data-stu-id="a8b14-112">It defines how a document flows, or moves, through the system by showing who must complete a task, make a decision, or approve a document.</span></span> <span data-ttu-id="a8b14-113">例如，下图显示支出报表的工作流。</span><span class="sxs-lookup"><span data-stu-id="a8b14-113">For example, the following illustration shows a workflow for expense reports.</span></span> 

![具有分配给用户的元素的工作流](./media/workflow_user.gif) 

<span data-ttu-id="a8b14-115">为了更好地理解这一工作流，假定 Sam 提交 7,000 美元的支出报表。</span><span class="sxs-lookup"><span data-stu-id="a8b14-115">To better understand this workflow, suppose that Sam submits an expense report for USD 7,000.</span></span> <span data-ttu-id="a8b14-116">在此场景中，Ivan 必须审核 Sam 传送给他的收据。</span><span class="sxs-lookup"><span data-stu-id="a8b14-116">In this scenario, Ivan must review the receipts that Sam routes to him.</span></span> <span data-ttu-id="a8b14-117">然后，晓辉和素心必须对该支出报表进行审核。</span><span class="sxs-lookup"><span data-stu-id="a8b14-117">Then Frank and Sue must approve the expense report.</span></span> <span data-ttu-id="a8b14-118">现在，假定 Sam 提交了一份 11,000 美元的支出报表。</span><span class="sxs-lookup"><span data-stu-id="a8b14-118">Now suppose that Sam submits an expense report for USD 11,000.</span></span> <span data-ttu-id="a8b14-119">在这种情况下，Ivan 必须复核相关收据，并且 Frank、Sue 和 Ann 必须审核该支出报表。</span><span class="sxs-lookup"><span data-stu-id="a8b14-119">In this scenario, Ivan must review the receipts, and Frank, Sue, and Ann must approve the expense report.</span></span>

## <a name="benefits-of-using-the-workflow-system"></a><span data-ttu-id="a8b14-120">使用工作流系统的优点</span><span class="sxs-lookup"><span data-stu-id="a8b14-120">Benefits of using the workflow system</span></span>

<span data-ttu-id="a8b14-121">在组织内使用工作流系统具有若干优点：</span><span class="sxs-lookup"><span data-stu-id="a8b14-121">There are several benefits of using the workflow system in your organization:</span></span>
-   <span data-ttu-id="a8b14-122">**一致的流程** - 您可定义处理特定文档（如采购申请和支出报表）的方法。</span><span class="sxs-lookup"><span data-stu-id="a8b14-122">**Consistent processes** – You can define how specific documents, such as purchase requisitions and expense reports, are processed.</span></span> <span data-ttu-id="a8b14-123">通过使用工作流系统，您可以确保以一致且有效的方式来处理和审核文档。</span><span class="sxs-lookup"><span data-stu-id="a8b14-123">By using the workflow system, you ensure that documents are processed and approved in a consistent and efficient manner.</span></span>
-   <span data-ttu-id="a8b14-124">**流程可见性** - 您可跟踪工作流实例的状态、历史记录和绩效指标。</span><span class="sxs-lookup"><span data-stu-id="a8b14-124">**Process visibility** – You can track the status, history, and performance metrics of workflow instances.</span></span> <span data-ttu-id="a8b14-125">这帮助您确定是否需要对该工作流做出更改，以提高效率。</span><span class="sxs-lookup"><span data-stu-id="a8b14-125">This helps you determine whether changes should be made to the workflow to improve efficiency.</span></span>
-   <span data-ttu-id="a8b14-126">**工作列表集中化** - 用户可以查看集中化的工作列表，该列表显示分配给他们的工作流任务和审核任务。</span><span class="sxs-lookup"><span data-stu-id="a8b14-126">**Centralized work list** – Users can view a centralized work list that displays the workflow tasks and approvals that are assigned to them.</span></span>


## <a name="workflow-content"></a><span data-ttu-id="a8b14-127">工作流内容</span><span class="sxs-lookup"><span data-stu-id="a8b14-127">Workflow content</span></span>

+ [<span data-ttu-id="a8b14-128">工作流架构</span><span class="sxs-lookup"><span data-stu-id="a8b14-128">Workflow architecture</span></span>](workflow-system-architecture.md)
+ [<span data-ttu-id="a8b14-129">工作流元素</span><span class="sxs-lookup"><span data-stu-id="a8b14-129">Workflow elements</span></span>](workflow-elements.md)
+ [<span data-ttu-id="a8b14-130">工作流操作</span><span class="sxs-lookup"><span data-stu-id="a8b14-130">Workflow actions</span></span>](workflow-actions.md)
+ [<span data-ttu-id="a8b14-131">创建工作流</span><span class="sxs-lookup"><span data-stu-id="a8b14-131">Create a workflow</span></span>](create-workflow.md)
+ [<span data-ttu-id="a8b14-132">配置工作流属性</span><span class="sxs-lookup"><span data-stu-id="a8b14-132">Configure workflow properties</span></span>](configure-workflow-properties.md)
+ [<span data-ttu-id="a8b14-133">在工作流中配置手动任务</span><span class="sxs-lookup"><span data-stu-id="a8b14-133">Configure a manual task in a workflow</span></span>](configure-manual-task-workflow.md)
+ [<span data-ttu-id="a8b14-134">在工作流中配置自动化任务</span><span class="sxs-lookup"><span data-stu-id="a8b14-134">Configure an automated task in a workflow</span></span>](configure-automated-task-workflow.md)
+ [<span data-ttu-id="a8b14-135">配置工作流中的审核流程</span><span class="sxs-lookup"><span data-stu-id="a8b14-135">Configure an approval process in a workflow</span></span>](configure-approval-process-workflow.md)
+ [<span data-ttu-id="a8b14-136">配置工作流中的审核步骤</span><span class="sxs-lookup"><span data-stu-id="a8b14-136">Configure an approval step in a workflow</span></span>](configure-approval-step-workflow.md)
+ [<span data-ttu-id="a8b14-137">在工作流中配置手动决策</span><span class="sxs-lookup"><span data-stu-id="a8b14-137">Configure a manual decision in a workflow</span></span>](configure-manual-decision-workflow.md)
+ [<span data-ttu-id="a8b14-138">在工作流中配置有条件决策</span><span class="sxs-lookup"><span data-stu-id="a8b14-138">Configure a conditional decision in a workflow</span></span>](configure-conditional-decision-workflow.md)
+ [<span data-ttu-id="a8b14-139">配置工作流中的并行活动</span><span class="sxs-lookup"><span data-stu-id="a8b14-139">Configure a parallel activity in a workflow</span></span>](configure-parallel-activity-workflow.md)
+ [<span data-ttu-id="a8b14-140">配置工作流中的并行分支</span><span class="sxs-lookup"><span data-stu-id="a8b14-140">Configure a parallel branch in a workflow</span></span>](configure-parallel-branch-workflow.md)
+ [<span data-ttu-id="a8b14-141">配置行项工作流</span><span class="sxs-lookup"><span data-stu-id="a8b14-141">Configure a line-item workflow</span></span>](configure-line-item-workflow.md)