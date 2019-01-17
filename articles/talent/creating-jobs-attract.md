---
title: 在 Attract 中创建、审核和发布工作
description: 此主题描述 Attract 中的工作元素。 它还介绍了如何创建工作。
author: josaw
manager: AnnBe
ms.date: 10/24/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-talent
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Talent, Core
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.search.industry: ''
ms.author: josaw
ms.search.validFrom: 2018-10-24
ms.dyn365.ops.version: Talent October 2018 update
ms.openlocfilehash: af945042c150fff1a95cdb046f2a712cb2c2c061
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "60272"
---
# <a name="create-approve-and-post-jobs-in-attract"></a><span data-ttu-id="13c8b-104">在 Attract 中创建、审核和发布工作</span><span class="sxs-lookup"><span data-stu-id="13c8b-104">Create, approve, and post jobs in Attract</span></span>

[!include [banner](includes/banner.md)]

<span data-ttu-id="13c8b-105">此主题描述 Microsoft Dynamics 365 for Talent: Attract 中的工作元素。</span><span class="sxs-lookup"><span data-stu-id="13c8b-105">This topic describes the elements of a job in Microsoft Dynamics 365 for Talent: Attract.</span></span> <span data-ttu-id="13c8b-106">它还介绍了如何创建工作。</span><span class="sxs-lookup"><span data-stu-id="13c8b-106">It also explains how to create a job.</span></span>

## <a name="job-creation"></a><span data-ttu-id="13c8b-107">工作创建</span><span class="sxs-lookup"><span data-stu-id="13c8b-107">Job creation</span></span>

<span data-ttu-id="13c8b-108">管理员、招聘人员和招聘经理可以创建工作。</span><span class="sxs-lookup"><span data-stu-id="13c8b-108">Admins, recruiters, and hiring managers can create jobs.</span></span> <span data-ttu-id="13c8b-109">当创建工作时，系统将提示您选择您在流程中的角色：招聘经理或招聘人员。</span><span class="sxs-lookup"><span data-stu-id="13c8b-109">When you create a job, you're prompted to select your role in the process: hiring manager or recruiter.</span></span> <span data-ttu-id="13c8b-110">在选择角色之后，将提示您选择流程模板。</span><span class="sxs-lookup"><span data-stu-id="13c8b-110">After you select a role, you're prompted to select a process template.</span></span> <span data-ttu-id="13c8b-111">如果您选择**跳过**，将使用默认模板。</span><span class="sxs-lookup"><span data-stu-id="13c8b-111">If you select **Skip**, the default template is used.</span></span> <span data-ttu-id="13c8b-112">有关流程模板的详细信息，请参阅[在 Attract 中创建流程模板](./process-templates-attract.md)。</span><span class="sxs-lookup"><span data-stu-id="13c8b-112">For more information about process templates, see [Create a process template in Attract](./process-templates-attract.md).</span></span>

<span data-ttu-id="13c8b-113">Attract 中的工作包含工作详细信息、招聘团队、招聘流程、工作发布和分析。</span><span class="sxs-lookup"><span data-stu-id="13c8b-113">A job in Attract has job details, a hiring team, a hiring process, job postings, and analytics.</span></span>

## <a name="job-details"></a><span data-ttu-id="13c8b-114">工作详细信息</span><span class="sxs-lookup"><span data-stu-id="13c8b-114">Job details</span></span>

<span data-ttu-id="13c8b-115">**工作详细信息**选项卡包含有关工作职责和属性的详细信息。</span><span class="sxs-lookup"><span data-stu-id="13c8b-115">The **Job details** tab contains details about the job's responsibilities and attributes.</span></span> <span data-ttu-id="13c8b-116">职务、工作描述和工作位置字段是必填字段。</span><span class="sxs-lookup"><span data-stu-id="13c8b-116">The fields for the job title, job description, and job location are required.</span></span> <span data-ttu-id="13c8b-117">其他字段是可选的。</span><span class="sxs-lookup"><span data-stu-id="13c8b-117">The other fields are optional.</span></span>

<span data-ttu-id="13c8b-118">默认情况下，**空缺数量**字段设置为 **1**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-118">By default, the **Number of openings** field is set to **1**.</span></span> <span data-ttu-id="13c8b-119">然而，您可以更改值。</span><span class="sxs-lookup"><span data-stu-id="13c8b-119">However, you can change the value.</span></span> <span data-ttu-id="13c8b-120">当为工作准备好了聘约时，**可用空缺数量**字段的值将减少。</span><span class="sxs-lookup"><span data-stu-id="13c8b-120">When an offer has been prepared for a job, the value of the **Number of openings available** field is decremented.</span></span>

<span data-ttu-id="13c8b-121">如果职位管理在管理员中心已打开，**更新职位**查找将可用。</span><span class="sxs-lookup"><span data-stu-id="13c8b-121">If position management has been turned on in the Admin Center, the **Update positions** lookup is available.</span></span> <span data-ttu-id="13c8b-122">此查找读取 Common Data Service for Apps 中的 JobPosition 实体并返回可为工作选择的职位列表。</span><span class="sxs-lookup"><span data-stu-id="13c8b-122">This lookup reads the JobPosition entity in Common Data Service for Apps and returns a list of positions that can be selected for the job.</span></span> <span data-ttu-id="13c8b-123">如果选择的职位数量超出空缺职位数量，将收到警告。</span><span class="sxs-lookup"><span data-stu-id="13c8b-123">If the number of positions that you select exceeds the number of open positions, you receive a warning.</span></span> <span data-ttu-id="13c8b-124">如果一个职位用于多个工作，您也会收到警告。</span><span class="sxs-lookup"><span data-stu-id="13c8b-124">You also receive a warning if a position is used on multiple jobs.</span></span>

> [!NOTE]
> <span data-ttu-id="13c8b-125">职位管理随综合招聘附件提供。</span><span class="sxs-lookup"><span data-stu-id="13c8b-125">Position management is available with the Comprehensive Hiring Add-on.</span></span>

<span data-ttu-id="13c8b-126">根据招聘流程的聘约活动的设置，职位编号可以在聘约中使用两次。</span><span class="sxs-lookup"><span data-stu-id="13c8b-126">Depending on the settings in the Offer activity of the hiring process, a position number can be used twice in an offer.</span></span> <span data-ttu-id="13c8b-127">有关详细信息，请参阅[招聘流程](./activities-attract.md)。</span><span class="sxs-lookup"><span data-stu-id="13c8b-127">For more information, see [Hiring process](./activities-attract.md).</span></span>

<span data-ttu-id="13c8b-128">Attract 包含一组默认**技能**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-128">Attract includes a default set of **Skills**.</span></span> <span data-ttu-id="13c8b-129">在键入时，这些技能作为建议出现。</span><span class="sxs-lookup"><span data-stu-id="13c8b-129">These skills appear as suggestions as you type.</span></span> <span data-ttu-id="13c8b-130">您可以通过在字段中输入新技能文本然后按 Enter 来添加更多技能。</span><span class="sxs-lookup"><span data-stu-id="13c8b-130">You can add more skills by entering the new skill text in the field and then pressing Enter.</span></span>

<span data-ttu-id="13c8b-131">Attract 包含一组默认的**工作职能**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-131">Attract includes a default set of **Job functions**.</span></span> <span data-ttu-id="13c8b-132">您可以通过在字段中输入新的工作职能然后按 Enter 来最多再添加三个工作职能。</span><span class="sxs-lookup"><span data-stu-id="13c8b-132">You can add up to three more job functions by entering the new job function in the field and then pressing Enter.</span></span>

<span data-ttu-id="13c8b-133">Attract 包含一组默认的**公司行业**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-133">Attract includes a default set of **Company industry**.</span></span> <span data-ttu-id="13c8b-134">您可以通过在字段中输入新的公司行业然后按 Enter 来最多再添加三个公司行业。</span><span class="sxs-lookup"><span data-stu-id="13c8b-134">You can add up to three more company industries by entering the new company industry in the field and then pressing Enter.</span></span>

## <a name="hiring-team"></a><span data-ttu-id="13c8b-135">招聘团队</span><span class="sxs-lookup"><span data-stu-id="13c8b-135">Hiring team</span></span>

<span data-ttu-id="13c8b-136">**招聘团队**选项卡包含工作所涉及的个人的列表。</span><span class="sxs-lookup"><span data-stu-id="13c8b-136">The **Hiring team** tab contains the list of individuals who will be involved in the job.</span></span> <span data-ttu-id="13c8b-137">在用户被添加到招聘团队时，必须为他们分配在招聘团队中的角色。</span><span class="sxs-lookup"><span data-stu-id="13c8b-137">When users are added to a hiring team, they must be assigned a role on the hiring team.</span></span> <span data-ttu-id="13c8b-138">角色确定用户有权访问的数据和他们将收到的通知。</span><span class="sxs-lookup"><span data-stu-id="13c8b-138">The role determines the data that the users have access to and the notifications that they receive.</span></span> <span data-ttu-id="13c8b-139">可以选择的角色有**招聘人员**、**招聘经理**、**委托人**和**面试官**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-139">The roles that can be selected are **Recruiter**, **Hiring manager**, **Delegate**, and **Interviewer**.</span></span> <span data-ttu-id="13c8b-140">有关角色权限的详细信息，请参阅“角色管理”文档。</span><span class="sxs-lookup"><span data-stu-id="13c8b-140">For more information about role privileges, see the "Role management" document.</span></span> <span data-ttu-id="13c8b-141">招聘人员和招聘经理可以指派一个或多个委托人来代表他们工作。</span><span class="sxs-lookup"><span data-stu-id="13c8b-141">Recruiters and hiring managers can appoint one or more delegates to work on their behalf.</span></span> <span data-ttu-id="13c8b-142">有关委托人的详细信息，请参阅 [Attract 中的安全和角色管理](./security-attract.md)。</span><span class="sxs-lookup"><span data-stu-id="13c8b-142">For more information about delegates, see [Security and role management in Attract](./security-attract.md).</span></span>

<span data-ttu-id="13c8b-143">招聘团队可以在激活工作后更新。</span><span class="sxs-lookup"><span data-stu-id="13c8b-143">The hiring team can be updated after the job is activated.</span></span>

## <a name="process"></a><span data-ttu-id="13c8b-144">进程</span><span class="sxs-lookup"><span data-stu-id="13c8b-144">Process</span></span>

<span data-ttu-id="13c8b-145">有关招聘流程的默认信息基于创建工作时选择的流程模板。</span><span class="sxs-lookup"><span data-stu-id="13c8b-145">Default information about the hiring process is based on the process template that was selected when the job was created.</span></span> <span data-ttu-id="13c8b-146">如果当时未选择特定模板，将使用默认模板。</span><span class="sxs-lookup"><span data-stu-id="13c8b-146">If a specific template wasn't selected at that time, the default template is used.</span></span> <span data-ttu-id="13c8b-147">在您定义招聘流程时，您可以添加或删除各个阶段，“应聘者”、“申请”和“聘约”阶段除外。</span><span class="sxs-lookup"><span data-stu-id="13c8b-147">When you define the hiring process, you can add or remove various stages, except the Prospect, Application, and Offer stages.</span></span> <span data-ttu-id="13c8b-148">虽然不能删除“应聘者”阶段，但可以将其关闭。</span><span class="sxs-lookup"><span data-stu-id="13c8b-148">Although the Prospect stage can't be removed, it can be turned off.</span></span> <span data-ttu-id="13c8b-149">在每个阶段中，可以添加或移除一个或多个预定义的活动。</span><span class="sxs-lookup"><span data-stu-id="13c8b-149">Within each stage, you can add or remove one or more predefined activities.</span></span>

<span data-ttu-id="13c8b-150">有关可以添加到招聘流程的活动的详细信息，请参阅 [Attract 中的招聘流程活动](./activities-attract.md)。</span><span class="sxs-lookup"><span data-stu-id="13c8b-150">For more information about activities that can be added to the hiring process, see [Hiring process activities in Attract](./activities-attract.md).</span></span>

> [!NOTE]
> <span data-ttu-id="13c8b-151">招聘流程不能在激活工作后更新。</span><span class="sxs-lookup"><span data-stu-id="13c8b-151">The process hiring can't be updated after a job is activated.</span></span>

## <a name="postings"></a><span data-ttu-id="13c8b-152">过帐记录</span><span class="sxs-lookup"><span data-stu-id="13c8b-152">Postings</span></span>

<span data-ttu-id="13c8b-153">在激活工作后，便可以发布工作。</span><span class="sxs-lookup"><span data-stu-id="13c8b-153">After a job is activated, it can be posted.</span></span> <span data-ttu-id="13c8b-154">只有招聘人员和管理员可以发布工作。</span><span class="sxs-lookup"><span data-stu-id="13c8b-154">Only recruiters and admins can post jobs.</span></span> <span data-ttu-id="13c8b-155">工作可以发布到 Talent Careers（ Microsoft Dynamics 365 for Talent 求职站点）或 LinkedIn。</span><span class="sxs-lookup"><span data-stu-id="13c8b-155">The job can be posted to either Talent Careers (a Microsoft Dynamics 365 for Talent career site) or LinkedIn.</span></span> <span data-ttu-id="13c8b-156">Attract 团队将持续努力与工作面板整合者合作。</span><span class="sxs-lookup"><span data-stu-id="13c8b-156">The Attract team continually works to partner with job board aggregators.</span></span> <span data-ttu-id="13c8b-157">因此，此列表一段时间后将扩展。</span><span class="sxs-lookup"><span data-stu-id="13c8b-157">Therefore, this list will expand over time.</span></span>

<span data-ttu-id="13c8b-158">有关工作发布的详细信息，请参阅 [Attract 中的求职站点功能](./career-site.md)。</span><span class="sxs-lookup"><span data-stu-id="13c8b-158">For more information about job postings, see [Career site functionality in Attract](./career-site.md).</span></span>

> [!NOTE]
> <span data-ttu-id="13c8b-159">工作发布功能只随 Attract 的综合招聘附件提供。</span><span class="sxs-lookup"><span data-stu-id="13c8b-159">The job posting functionality is available only with the Comprehensive Hiring Add-on for Attract.</span></span>

## <a name="activate"></a><span data-ttu-id="13c8b-160">启用</span><span class="sxs-lookup"><span data-stu-id="13c8b-160">Activate</span></span>

<span data-ttu-id="13c8b-161">在激活工作后，可以发布工作，并且可以将应聘者和申请人添加到工作中。</span><span class="sxs-lookup"><span data-stu-id="13c8b-161">After a job is activated, it can be posted, and prospects and applicants can be added to it.</span></span> <span data-ttu-id="13c8b-162">向工作添加应聘者的选项在招聘流程中的“应聘者”活动中设置。</span><span class="sxs-lookup"><span data-stu-id="13c8b-162">The option to add prospects to a job is set in the Prospect activity in the hiring process.</span></span>

> [!NOTE]
> <span data-ttu-id="13c8b-163">招聘流程不能在激活工作后更新。</span><span class="sxs-lookup"><span data-stu-id="13c8b-163">The process hiring can't be updated after a job is activated.</span></span>

## <a name="prospects-and-applicants"></a><span data-ttu-id="13c8b-164">应聘者和申请人</span><span class="sxs-lookup"><span data-stu-id="13c8b-164">Prospects and applicants</span></span>

<span data-ttu-id="13c8b-165">向工作添加应聘者的选项在招聘流程中的[应聘者活动](./activities-attract.md#prospect-activity)中设置。</span><span class="sxs-lookup"><span data-stu-id="13c8b-165">The option to add prospects to a job is set in the [Prospect activity](./activities-attract.md#prospect-activity) in the hiring process.</span></span> <span data-ttu-id="13c8b-166">此选项应在激活工作之前设置。</span><span class="sxs-lookup"><span data-stu-id="13c8b-166">This option should be set before you activate the job.</span></span> <span data-ttu-id="13c8b-167">在激活工作后，可以将应聘者和申请人添加到工作中。</span><span class="sxs-lookup"><span data-stu-id="13c8b-167">After a job is activated, prospects and applicants can be added to it.</span></span>

## <a name="approvals"></a><span data-ttu-id="13c8b-168">审核</span><span class="sxs-lookup"><span data-stu-id="13c8b-168">Approvals</span></span>

<span data-ttu-id="13c8b-169">Attract 工作可以提交以供审核。</span><span class="sxs-lookup"><span data-stu-id="13c8b-169">Attract jobs can be submitted for approval.</span></span> <span data-ttu-id="13c8b-170">并非所有工作都需要审核。</span><span class="sxs-lookup"><span data-stu-id="13c8b-170">Not all jobs require approval.</span></span> <span data-ttu-id="13c8b-171">要求在模板级别设置。</span><span class="sxs-lookup"><span data-stu-id="13c8b-171">The requirement is set at the template level.</span></span> <span data-ttu-id="13c8b-172">默认情况下，审核在模板中是关闭的。</span><span class="sxs-lookup"><span data-stu-id="13c8b-172">By default, approvals are turned off on the template.</span></span> <span data-ttu-id="13c8b-173">若要设置审核，请转到流程模板，将**审核**字段设置为“默认”。</span><span class="sxs-lookup"><span data-stu-id="13c8b-173">To set up approvals, go to a process template, and set the **Approval** field to Default.</span></span> <span data-ttu-id="13c8b-174">然后在您创建工作时选择该模板。</span><span class="sxs-lookup"><span data-stu-id="13c8b-174">Then select that template when you create the job.</span></span>

<span data-ttu-id="13c8b-175">在保存工作之后，可以提交工作以供审核。</span><span class="sxs-lookup"><span data-stu-id="13c8b-175">After a job is saved, it can be submitted for approval.</span></span> <span data-ttu-id="13c8b-176">下表列出了使用审核的文档的状态。</span><span class="sxs-lookup"><span data-stu-id="13c8b-176">The following table lists the statuses of a document that uses approvals.</span></span>

| <span data-ttu-id="13c8b-177">状态</span><span class="sxs-lookup"><span data-stu-id="13c8b-177">Status</span></span>   | <span data-ttu-id="13c8b-178">状态</span><span class="sxs-lookup"><span data-stu-id="13c8b-178">State</span></span>                                                               |
|----------|---------------------------------------------------------------------|
| <span data-ttu-id="13c8b-179">草案</span><span class="sxs-lookup"><span data-stu-id="13c8b-179">Draft</span></span>    | <span data-ttu-id="13c8b-180">工作已保存，但未提交到工作流。</span><span class="sxs-lookup"><span data-stu-id="13c8b-180">The job has been saved, but it hasn't been submitted to a workflow.</span></span> |
| <span data-ttu-id="13c8b-181">挂起</span><span class="sxs-lookup"><span data-stu-id="13c8b-181">Pending</span></span>  | <span data-ttu-id="13c8b-182">工作已提交给审核人。</span><span class="sxs-lookup"><span data-stu-id="13c8b-182">The job has been submitted to approvers.</span></span>                            |
| <span data-ttu-id="13c8b-183">已审批</span><span class="sxs-lookup"><span data-stu-id="13c8b-183">Approved</span></span> | <span data-ttu-id="13c8b-184">工作已审核，但未激活。</span><span class="sxs-lookup"><span data-stu-id="13c8b-184">The job has been approved, but it hasn't been activated.</span></span>            |
| <span data-ttu-id="13c8b-185">已拒绝</span><span class="sxs-lookup"><span data-stu-id="13c8b-185">Rejected</span></span> | <span data-ttu-id="13c8b-186">工作被拒绝，无法激活。</span><span class="sxs-lookup"><span data-stu-id="13c8b-186">The job has been rejected, and it can't be activated.</span></span>               |
| <span data-ttu-id="13c8b-187">有效的</span><span class="sxs-lookup"><span data-stu-id="13c8b-187">Active</span></span>   | <span data-ttu-id="13c8b-188">工作已审核并激活。</span><span class="sxs-lookup"><span data-stu-id="13c8b-188">The job has been approved and activated.</span></span>                            |

<span data-ttu-id="13c8b-189">在工作列表中，您可以筛选工作状态。</span><span class="sxs-lookup"><span data-stu-id="13c8b-189">In the job list, you can filter on the job statuses.</span></span>

<span data-ttu-id="13c8b-190">审核可以发送给公司中的任何 Microsoft Azure Active Directory (Azure AD) 用户。</span><span class="sxs-lookup"><span data-stu-id="13c8b-190">Approvals can be sent to any Microsoft Azure Active Directory (Azure AD) user in the company.</span></span> <span data-ttu-id="13c8b-191">审核可以同时发送给列出为审核人的所有人员。</span><span class="sxs-lookup"><span data-stu-id="13c8b-191">The approvals are sent in parallel to all the people who are listed as approvers.</span></span> <span data-ttu-id="13c8b-192">在审核工作后，便可以激活工作。</span><span class="sxs-lookup"><span data-stu-id="13c8b-192">After a job is approved, it can be activated.</span></span>

<span data-ttu-id="13c8b-193">列出为审核人的人员将在 Attract 中收到通知，通知他们有要审核的项目。</span><span class="sxs-lookup"><span data-stu-id="13c8b-193">The people who are listed as approvers will receive a notification in Attract to inform them that they have an item to approve.</span></span> <span data-ttu-id="13c8b-194">审核项目也将出现在仪表板的**已分配给您**部分。</span><span class="sxs-lookup"><span data-stu-id="13c8b-194">An approval item will also appear in the **Assigned to you** section on the dashboard.</span></span> <span data-ttu-id="13c8b-195">在有人接受或审核工作后，招聘团队将收到通知。</span><span class="sxs-lookup"><span data-stu-id="13c8b-195">After someone accepts or approves a job, the hiring team will receive a notification.</span></span> <span data-ttu-id="13c8b-196">最后，在工作被审核时招聘团队将收到通知。</span><span class="sxs-lookup"><span data-stu-id="13c8b-196">Finally, the hiring team will receive a notification when the job is approved.</span></span>

## <a name="create-a-job"></a><span data-ttu-id="13c8b-197">创建工作</span><span class="sxs-lookup"><span data-stu-id="13c8b-197">Create a job</span></span>

<span data-ttu-id="13c8b-198">请遵从这些步骤创建工作。</span><span class="sxs-lookup"><span data-stu-id="13c8b-198">Follow these steps to create a job.</span></span>

1. <span data-ttu-id="13c8b-199">转至**工作**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-199">Go to **Jobs**.</span></span>
2. <span data-ttu-id="13c8b-200">选择**新建**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-200">Select **New**.</span></span>
3. <span data-ttu-id="13c8b-201">在**职务**字段中，输入职务。</span><span class="sxs-lookup"><span data-stu-id="13c8b-201">In the **Job title** field, enter the job title.</span></span> <span data-ttu-id="13c8b-202">在**角色**字段中，输入您的角色。</span><span class="sxs-lookup"><span data-stu-id="13c8b-202">In the **Role** field, enter your role.</span></span>
4. <span data-ttu-id="13c8b-203">在**模板**字段中，选择模板。</span><span class="sxs-lookup"><span data-stu-id="13c8b-203">In the **Template** field, select a template.</span></span> <span data-ttu-id="13c8b-204">或者，选择**跳过**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-204">Alternatively, select **Skip**.</span></span> <span data-ttu-id="13c8b-205">如果您选择**跳过**，将使用标记为默认模板的模板。</span><span class="sxs-lookup"><span data-stu-id="13c8b-205">If you select **Skip**, the template that is marked as the default template is used.</span></span>

    <span data-ttu-id="13c8b-206">如果文档应经过审核流程，请选择**审核流程**字段设置为**默认**的模板。</span><span class="sxs-lookup"><span data-stu-id="13c8b-206">If the document should go through an approval process, select a template where the **Approval process** field is set to **Default**.</span></span>

5. <span data-ttu-id="13c8b-207">在**详细信息**选项卡上，输入工作的详细信息。</span><span class="sxs-lookup"><span data-stu-id="13c8b-207">On the **Details** tab, enter the details of the job.</span></span> <span data-ttu-id="13c8b-208">**职务**、**工作描述**和**位置**字段是必填字段。</span><span class="sxs-lookup"><span data-stu-id="13c8b-208">The **Title**, **Job description**, and **Location** fields are required.</span></span>
6. <span data-ttu-id="13c8b-209">选择**保存**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-209">Select **Save**.</span></span>
7. <span data-ttu-id="13c8b-210">在**招聘团队**选项卡上，添加招聘经理、招聘人员或面试官。</span><span class="sxs-lookup"><span data-stu-id="13c8b-210">On the **Hiring team** tab, add a hiring manager, recruiter, or interviewer.</span></span>
8. <span data-ttu-id="13c8b-211">选择**保存**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-211">Select **Save**.</span></span>
9. <span data-ttu-id="13c8b-212">在**流程**选项卡上，根据需要添加或删除阶段：</span><span class="sxs-lookup"><span data-stu-id="13c8b-212">On the **Process** tab, add or remove stages as you require:</span></span>

    - <span data-ttu-id="13c8b-213">若要添加阶段，请选择 **+ 新阶段**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-213">To add a stage, select **+ New Stage**.</span></span>
    - <span data-ttu-id="13c8b-214">若要删除阶段，将指针悬停在要删除的阶段上，然后选择出现的垃圾桶按钮。</span><span class="sxs-lookup"><span data-stu-id="13c8b-214">To remove a stage, hover the pointer over the stage to remove, and then select the trash can button that appears.</span></span>

        > [!NOTE]
        > <span data-ttu-id="13c8b-215">不能删除“应聘者”、“申请”和“聘约”阶段。</span><span class="sxs-lookup"><span data-stu-id="13c8b-215">The Prospect, Application, and Offer stages can't be removed.</span></span>

10. <span data-ttu-id="13c8b-216">根据需要添加或删除活动：</span><span class="sxs-lookup"><span data-stu-id="13c8b-216">Add or remove activities as you require:</span></span>

    - <span data-ttu-id="13c8b-217">要添加活动，请将其从右侧的列表拖到相应的阶段。</span><span class="sxs-lookup"><span data-stu-id="13c8b-217">To add an activity, drag it from the list on the right to the appropriate stage.</span></span> <span data-ttu-id="13c8b-218">或者，双击活动，然后选择要添加到的阶段。</span><span class="sxs-lookup"><span data-stu-id="13c8b-218">Alternatively, double-click the activity, and then select the stage to add it to.</span></span>
    - <span data-ttu-id="13c8b-219">若要删除活动，展开活动，然后选择活动标题上的垃圾桶按钮。</span><span class="sxs-lookup"><span data-stu-id="13c8b-219">To remove an activity, expand the activity, and then select the trash can button on the activity header.</span></span>

11. <span data-ttu-id="13c8b-220">选择**保存**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-220">Select **Save**.</span></span>
12. <span data-ttu-id="13c8b-221">如果您选择了使用审核流程，请执行以下步骤：</span><span class="sxs-lookup"><span data-stu-id="13c8b-221">If you selected to use an approval process, follow these steps:</span></span>

    1. <span data-ttu-id="13c8b-222">选择 **+ 添加审核人**，然后输入具有 Azure AD 帐户的用户。</span><span class="sxs-lookup"><span data-stu-id="13c8b-222">Select **+ Add approver**, and then enter a user who has an Azure AD account.</span></span> <span data-ttu-id="13c8b-223">您可以添加多个审核人。</span><span class="sxs-lookup"><span data-stu-id="13c8b-223">You can add multiple approvers.</span></span>
    2. <span data-ttu-id="13c8b-224">选择**发送给审核人**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-224">Select **Send to approvers**.</span></span>

    <span data-ttu-id="13c8b-225">工作的**工作状态**字段设置为**待处理**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-225">The **Job status** field of the job is set to **Pending**.</span></span> <span data-ttu-id="13c8b-226">在**工作状态**字段的值更改为**已审核**后，可以激活该工作。</span><span class="sxs-lookup"><span data-stu-id="13c8b-226">After the value of the **Job status** field changes to **Approved**, the job can be activated.</span></span>

13. <span data-ttu-id="13c8b-227">若要激活工作，请选择**激活**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-227">To activate the job, select **Activate**.</span></span>
14. <span data-ttu-id="13c8b-228">要发布工作，请转到**发布**，然后选择 Talent Careers 站点或 LinkedIn 下的**立即发布**。</span><span class="sxs-lookup"><span data-stu-id="13c8b-228">To post the job, go to **Postings**, and then select **Post Now** under the Talent Careers site or LinkedIn.</span></span>
