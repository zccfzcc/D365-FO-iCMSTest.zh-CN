---
title: “时间和出勤”中的缺勤登记
description: 本主题说明如何处理“时间和出勤”中的缺勤登记。
author: johanhoffmann
manager: AnnBe
ms.date: 05/26/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: JMGParameters
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 269384
ms.search.region: Global
ms.author: johanho
ms.search.validFrom: 2017-09-20
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: a95be5a95bd99b0d7ac2fed1c265760573a4a1c6
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55997"
---
# <a name="absence-registration-in-time-and-attendance"></a><span data-ttu-id="fc34a-103">“时间和出勤”中的缺勤登记</span><span class="sxs-lookup"><span data-stu-id="fc34a-103">Absence registration in Time and attendance</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="fc34a-104">此主题描述缺勤的概念并说明如何处理“时间和出勤”中的缺勤。</span><span class="sxs-lookup"><span data-stu-id="fc34a-104">This topic describes the concepts for absence and explains how to handle absence in Time and attendance.</span></span>

## <a name="absence-that-is-based-on-regular-work-hours"></a><span data-ttu-id="fc34a-105">基于正常工作时间的缺勤</span><span class="sxs-lookup"><span data-stu-id="fc34a-105">Absence that is based on regular work hours</span></span>

<span data-ttu-id="fc34a-106">工作人员在其正常工作时间不工作的任何工时都被视为缺勤。</span><span class="sxs-lookup"><span data-stu-id="fc34a-106">Workers are considered absent for any hours that they don't work during their regular work hours.</span></span> <span data-ttu-id="fc34a-107">正常工时在工作人员的标准时间模板中定义。</span><span class="sxs-lookup"><span data-stu-id="fc34a-107">Regular work hours are defined in a worker's standard time profile.</span></span>

<span data-ttu-id="fc34a-108">例如，工作人员使用的工作日模板的上班打卡时间是上午 7:00，下班打卡时间是下午 3:00。</span><span class="sxs-lookup"><span data-stu-id="fc34a-108">For example, a worker is working on a day profile that has clock-in at 7:00 AM and clock-out at 3:00 PM.</span></span> <span data-ttu-id="fc34a-109">如果工作人员在上午 9:00 打卡，他在当天上午 7:00 到 9:00 这段时间会被视为缺勤。</span><span class="sxs-lookup"><span data-stu-id="fc34a-109">If the worker clocks in at 9:00 AM, he is considered absent from 7:00 AM to 9:00 AM on that day.</span></span>

<span data-ttu-id="fc34a-110">在这种情况下，工作人员会被提示输入其缺勤原因。</span><span class="sxs-lookup"><span data-stu-id="fc34a-110">In this case, workers are prompted to enter a reason for their absence.</span></span> <span data-ttu-id="fc34a-111">他们可以通过选择考勤代码来指定原因。</span><span class="sxs-lookup"><span data-stu-id="fc34a-111">They can specify a reason by selecting an absence code.</span></span>

## <a name="absence-codes"></a><span data-ttu-id="fc34a-112">考勤代码</span><span class="sxs-lookup"><span data-stu-id="fc34a-112">Absence codes</span></span>

<span data-ttu-id="fc34a-113">缺勤代码定义缺勤的各种类型。</span><span class="sxs-lookup"><span data-stu-id="fc34a-113">Absence codes define the various types of absence.</span></span> <span data-ttu-id="fc34a-114">缺勤代码由公司定义。</span><span class="sxs-lookup"><span data-stu-id="fc34a-114">Absence codes are defined by the company.</span></span>

<span data-ttu-id="fc34a-115">缺勤代码可能应用不同规则。</span><span class="sxs-lookup"><span data-stu-id="fc34a-115">Various rules can be applied to absence codes.</span></span> <span data-ttu-id="fc34a-116">例如，可以将缺勤代码配置为扣减或准予付薪。</span><span class="sxs-lookup"><span data-stu-id="fc34a-116">For example, an absence code can be configured to deduct or grant pay.</span></span>

<span data-ttu-id="fc34a-117">例如，公司定义了工作人员在迟到且没有正当理由时使用的**迟到**缺勤代码。</span><span class="sxs-lookup"><span data-stu-id="fc34a-117">For example, a company defines a **Late** absence code that workers use if they come in late and don't have a good reason.</span></span> <span data-ttu-id="fc34a-118">公司还定义了工作人员用于参加内部课程所花费时间的**内部课程**缺勤代码。</span><span class="sxs-lookup"><span data-stu-id="fc34a-118">The company also defines an **Internal course** absence code that workers use for time that they spend attending internal courses.</span></span> <span data-ttu-id="fc34a-119">这些缺勤代码可以进行设置，以便**迟到**时从工作人员的付薪中减扣，而**内部课程**不减扣。</span><span class="sxs-lookup"><span data-stu-id="fc34a-119">These absence codes can be set up so that **Late** deducts from a worker's pay but **Internal course** doesn't deduct from a worker's pay.</span></span>

<span data-ttu-id="fc34a-120">您可以设置自动缺勤代码。</span><span class="sxs-lookup"><span data-stu-id="fc34a-120">You can set up automatic absence codes.</span></span> <span data-ttu-id="fc34a-121">这些缺勤代码可用于在未登记缺勤时计算工作人员的工时。</span><span class="sxs-lookup"><span data-stu-id="fc34a-121">These absence codes can be used to calculate a worker's time when no absence is registered.</span></span> <span data-ttu-id="fc34a-122">工作人员的时间模板确定是使用标准工时还是弹性工时的缺勤代码。</span><span class="sxs-lookup"><span data-stu-id="fc34a-122">The worker's time profile determines whether the absence code for standard time or flex time is used.</span></span>

### <a name="set-up-standard-time-and-flex-time"></a><span data-ttu-id="fc34a-123">设置标准工时和弹性工时</span><span class="sxs-lookup"><span data-stu-id="fc34a-123">Set up standard time and flex time</span></span>

- <span data-ttu-id="fc34a-124">通过使用**时间和出勤参数**页的**自动插入缺勤**和**自动插入弹性-** 选项来配置标准工时和弹性工时的参数。</span><span class="sxs-lookup"><span data-stu-id="fc34a-124">Configure the parameters for standard time and flex time by using the **Auto insert absence** and **Auto insert Flex-** options on the **Time and attendance parameters** page.</span></span>

## <a name="absence-groups"></a><span data-ttu-id="fc34a-125">缺勤组</span><span class="sxs-lookup"><span data-stu-id="fc34a-125">Absence groups</span></span>

<span data-ttu-id="fc34a-126">缺勤代码被分组到缺勤组。</span><span class="sxs-lookup"><span data-stu-id="fc34a-126">Absence codes are grouped into absence groups.</span></span> <span data-ttu-id="fc34a-127">您可以使用缺勤组将具有共同特征的缺勤代码分组。</span><span class="sxs-lookup"><span data-stu-id="fc34a-127">You use absence groups to group absence codes that have common characteristics.</span></span> <span data-ttu-id="fc34a-128">示例包括正常缺勤或由于看医生、陪审员义务或孩子生病所导致缺勤的缺勤代码。</span><span class="sxs-lookup"><span data-stu-id="fc34a-128">Examples include absence codes for a legal absence, or absence because of a doctor's appointment, jury duty, or a sick child.</span></span>

## <a name="planned-absence"></a><span data-ttu-id="fc34a-129">计划缺勤</span><span class="sxs-lookup"><span data-stu-id="fc34a-129">Planned absence</span></span>

<span data-ttu-id="fc34a-130">如果您知道某个工作人员将在某个时间段内缺勤（如预计休假），您可以使用计划缺勤。</span><span class="sxs-lookup"><span data-stu-id="fc34a-130">If you know that a worker will be absent for a period, such as an upcoming vacation, you can use planned absence.</span></span> <span data-ttu-id="fc34a-131">您通过配置考勤代码来设置计划缺勤，以便考虑计划缺勤。</span><span class="sxs-lookup"><span data-stu-id="fc34a-131">You set up planned absence by configuring the absence code so that it considers the planned absence.</span></span> <span data-ttu-id="fc34a-132">在设置计划缺勤时，当计算用户工时登记时不会向您提示该缺勤期间的缺勤代码。</span><span class="sxs-lookup"><span data-stu-id="fc34a-132">When you set up a planned absence, you aren't prompted for an absence code during the absence period when user time registrations are calculated.</span></span> <span data-ttu-id="fc34a-133">计划缺勤可针对单个工作人员定义，也可以定义批处理作业来批量更新多名工作人员的计划缺勤。</span><span class="sxs-lookup"><span data-stu-id="fc34a-133">Planned absence can be defined for a single worker, or you can define a batch job to bulk update the planned absence for workers.</span></span>

### <a name="set-up-planned-absence"></a><span data-ttu-id="fc34a-134">设置计划缺勤</span><span class="sxs-lookup"><span data-stu-id="fc34a-134">Set up planned absence</span></span>

1. <span data-ttu-id="fc34a-135">选择**人力资源**&gt;**工作人员**&gt;**员工**，然后选择一名员工。</span><span class="sxs-lookup"><span data-stu-id="fc34a-135">Select **Human resources** &gt; **Workers** &gt; **Employees**, and select an employee.</span></span>
2. <span data-ttu-id="fc34a-136">选择**时间**&gt;**分配时间** &gt;**缺勤时间登记**，然后设置计划缺勤。</span><span class="sxs-lookup"><span data-stu-id="fc34a-136">Select **Time** &gt; **Time assignments** &gt; **Time Absence registration**, and set up the planned absence.</span></span>

## <a name="interrupted-planned-absence"></a><span data-ttu-id="fc34a-137">中断的计划缺勤</span><span class="sxs-lookup"><span data-stu-id="fc34a-137">Interrupted planned absence</span></span>

<span data-ttu-id="fc34a-138">如果您在设置计划缺勤时应用**中断**选项，那么当工作人员在计划缺勤期间登录，该计划缺勤将被中断。</span><span class="sxs-lookup"><span data-stu-id="fc34a-138">If you apply the **Interrupt** option when you set up a planned absence, the planned absence will be interrupted if the worker signs in during the planned absence period.</span></span> <span data-ttu-id="fc34a-139">计划缺勤将被标记为**中断**，这不会对将来计算造成任何影响。</span><span class="sxs-lookup"><span data-stu-id="fc34a-139">The planned absence will be marked as **Interrupted** and won't have any effect on future calculations.</span></span>

### <a name="set-up-a-planned-absence-for-interruption"></a><span data-ttu-id="fc34a-140">设置要中断的计划缺勤</span><span class="sxs-lookup"><span data-stu-id="fc34a-140">Set up a planned absence for interruption</span></span>

1. <span data-ttu-id="fc34a-141">打开**缺勤时间登记**页，如设置计划缺勤的过程中所述。</span><span class="sxs-lookup"><span data-stu-id="fc34a-141">Open the **Time Absence registration** page as described in the procedure for setting up planned absence.</span></span>
2. <span data-ttu-id="fc34a-142">选择**中断**。</span><span class="sxs-lookup"><span data-stu-id="fc34a-142">Select **Interrupt**.</span></span>

<span data-ttu-id="fc34a-143">在工时通过车间终端或车间设备登记时应用**中断**选项。</span><span class="sxs-lookup"><span data-stu-id="fc34a-143">The **Interrupt** option applies when time is registered through the shop floor terminal or the shop floor device.</span></span> <span data-ttu-id="fc34a-144">如果登记在计算和审核页面或**电子工时记录卡**页输入，则不应用此选项。</span><span class="sxs-lookup"><span data-stu-id="fc34a-144">The option doesn't apply if the registrations are entered on the calculation and approval pages, or on the **Electronic timecard** page.</span></span>

## <a name="examples-of-the-use-of-absence-in-a-flex-profile"></a><span data-ttu-id="fc34a-145">在弹性模板中使用缺勤的示例</span><span class="sxs-lookup"><span data-stu-id="fc34a-145">Examples of the use of absence in a flex profile</span></span>

<span data-ttu-id="fc34a-146">以下三个示例显示如何在具有弹性期间的模板中计算缺勤。</span><span class="sxs-lookup"><span data-stu-id="fc34a-146">The following three examples show how absence is calculated in a profile that has flex periods.</span></span>

<span data-ttu-id="fc34a-147">这些示例使用以下模板。</span><span class="sxs-lookup"><span data-stu-id="fc34a-147">The examples use the following profile.</span></span>

| <span data-ttu-id="fc34a-148">上班打卡</span><span class="sxs-lookup"><span data-stu-id="fc34a-148">Clock-in</span></span> | <span data-ttu-id="fc34a-149">标准时间</span><span class="sxs-lookup"><span data-stu-id="fc34a-149">Standard time</span></span>    | <span data-ttu-id="fc34a-150">休息</span><span class="sxs-lookup"><span data-stu-id="fc34a-150">Break</span></span>             | <span data-ttu-id="fc34a-151">标准时间</span><span class="sxs-lookup"><span data-stu-id="fc34a-151">Standard time</span></span> | <span data-ttu-id="fc34a-152">弹性-</span><span class="sxs-lookup"><span data-stu-id="fc34a-152">Flex-</span></span>        | <span data-ttu-id="fc34a-153">下班打卡</span><span class="sxs-lookup"><span data-stu-id="fc34a-153">Clock-out</span></span> | <span data-ttu-id="fc34a-154">弹性+</span><span class="sxs-lookup"><span data-stu-id="fc34a-154">Flex+</span></span>        |
|----------|------------------|-------------------|---------------|--------------|-----------|--------------|
| <span data-ttu-id="fc34a-155">上午 8 点</span><span class="sxs-lookup"><span data-stu-id="fc34a-155">8 AM</span></span>     | <span data-ttu-id="fc34a-156">上午 9 点到 11:30</span><span class="sxs-lookup"><span data-stu-id="fc34a-156">9 AM to 11:30 AM</span></span> | <span data-ttu-id="fc34a-157">中午 11:30 到 12 点</span><span class="sxs-lookup"><span data-stu-id="fc34a-157">11:30 AM to 12 PM</span></span> | <span data-ttu-id="fc34a-158">中午 12 点到下午 3 点</span><span class="sxs-lookup"><span data-stu-id="fc34a-158">12 PM to 3 PM</span></span> | <span data-ttu-id="fc34a-159">下午 3 点到 4 点</span><span class="sxs-lookup"><span data-stu-id="fc34a-159">3 PM to 4 PM</span></span> | <span data-ttu-id="fc34a-160">下午 4 点</span><span class="sxs-lookup"><span data-stu-id="fc34a-160">4 PM</span></span>      | <span data-ttu-id="fc34a-161">下午 4 点到 6 点</span><span class="sxs-lookup"><span data-stu-id="fc34a-161">4 PM to 6 PM</span></span> |

### <a name="example-1-signing-out-during-a-flex--period"></a><span data-ttu-id="fc34a-162">示例 1：在“弹性-”期间注销</span><span class="sxs-lookup"><span data-stu-id="fc34a-162">Example 1: Signing out during a Flex- period</span></span>

<span data-ttu-id="fc34a-163">工作人员在上午 8:00 上班打卡，在下午 3:30 下班打卡。</span><span class="sxs-lookup"><span data-stu-id="fc34a-163">The worker clocks in at 8:00 AM and clocks out at 3:30 PM.</span></span> <span data-ttu-id="fc34a-164">在这种情况下，因为工作人员在“弹性-”期间下班打卡，不会计算缺勤时间，将从工作人员的弹性结余中扣减半小时。</span><span class="sxs-lookup"><span data-stu-id="fc34a-164">In this case, because the worker clocks out during a Flex- period, no absence is calculated, and half an hour is deducted from the worker's flex balance.</span></span>

### <a name="example-2-signing-out-in-during-standard-time-period"></a><span data-ttu-id="fc34a-165">示例 2：在“标准时间”期间注销</span><span class="sxs-lookup"><span data-stu-id="fc34a-165">Example 2: Signing out in during Standard time period</span></span>

<span data-ttu-id="fc34a-166">工作人员在上午 8:00 上班打卡，在下午 2:30 下班打卡。</span><span class="sxs-lookup"><span data-stu-id="fc34a-166">The worker clocks in at 8:00 AM and clocks out at 2:30 PM.</span></span> <span data-ttu-id="fc34a-167">在这种情况下，因为工作人员在“标准时间”期间注销，从下午 2:30 到 4 点将被计算为缺勤时间，并会登记 1.5 小时的缺勤时间。</span><span class="sxs-lookup"><span data-stu-id="fc34a-167">In this case, because the worker clocks out during the Standard time period, absence is calculated from 2:30 PM to 4 PM, and an absence period of 1.5 hours is registered.</span></span> <span data-ttu-id="fc34a-168">需要填写该期间的缺勤代码。</span><span class="sxs-lookup"><span data-stu-id="fc34a-168">An absence code for that period is required.</span></span>

### <a name="example-3-signing-out-during-a-flex-period"></a><span data-ttu-id="fc34a-169">示例 3：在“弹性+”期间注销</span><span class="sxs-lookup"><span data-stu-id="fc34a-169">Example 3: Signing out during a Flex+ period</span></span>

<span data-ttu-id="fc34a-170">工作人员在上午 8:00 上班打卡，在下午 4:30 下班打卡。</span><span class="sxs-lookup"><span data-stu-id="fc34a-170">The worker clocks in at 8:00 AM and clocks out at 4:30 PM.</span></span> <span data-ttu-id="fc34a-171">在这种情况下，因为工作人员在“弹性+”期间下班打卡，不会计算缺勤时间，工作人员的弹性结余将增加半小时。</span><span class="sxs-lookup"><span data-stu-id="fc34a-171">In this case, because the worker clocks out during a Flex+ period, no absence is calculated, and half an hour is added to the worker's flex balance.</span></span>

## <a name="absence-in-the-calculation-and-approval-process"></a><span data-ttu-id="fc34a-172">计算和审核流程中的缺勤</span><span class="sxs-lookup"><span data-stu-id="fc34a-172">Absence in the calculation and approval process</span></span>

<span data-ttu-id="fc34a-173">必须先计算和审核工作人员工时登记，然后才能将其作为付薪项转移到工资系统。</span><span class="sxs-lookup"><span data-stu-id="fc34a-173">Worker time registrations must be calculated and approved before they can be transferred to a payroll system as pay items.</span></span>

<span data-ttu-id="fc34a-174">审核人可以更改工作人员的工时登记。</span><span class="sxs-lookup"><span data-stu-id="fc34a-174">An approver can change a worker's time registrations.</span></span> <span data-ttu-id="fc34a-175">审核人甚至可以更改工作人员已登记的任何缺勤。</span><span class="sxs-lookup"><span data-stu-id="fc34a-175">The approver can even change any absence that the worker has registered.</span></span> <span data-ttu-id="fc34a-176">如果审核人手动输入具有缺勤代码的时段，则该期间的缺勤代码不会被“时间和出勤参数”中的默认缺勤代码覆盖。</span><span class="sxs-lookup"><span data-stu-id="fc34a-176">If the approver manually enters a time period that has an absence code, the absence code for that period isn't overridden by the default absence code from the Time and attendance parameters.</span></span>

<span data-ttu-id="fc34a-177">例如，工作人员在上午 10 点上班打卡并选择指示她迟到的缺勤代码。</span><span class="sxs-lookup"><span data-stu-id="fc34a-177">For example, a worker clocks in at 10 AM and selects an absence code that indicates that she is late.</span></span> <span data-ttu-id="fc34a-178">后来，该工作人员告知她的主管她从上午 8 点到 10 点之间是去看医生。</span><span class="sxs-lookup"><span data-stu-id="fc34a-178">Later, the worker informs her supervisor that she had a doctor's appointment from 8 AM to 10 AM.</span></span> <span data-ttu-id="fc34a-179">看医生不应扣减工作人员的付薪。</span><span class="sxs-lookup"><span data-stu-id="fc34a-179">A doctor's appointment should not cause a deduction in the worker's pay.</span></span> <span data-ttu-id="fc34a-180">因此，在这种情况下，主管可以手动输入指示这两个小时是病假的缺勤代码，以此来调整从上午 8 点到 10 点的两小时缺勤。</span><span class="sxs-lookup"><span data-stu-id="fc34a-180">Therefore, in this case, the supervisor can adjust the two hours of absence from 8 AM to 10 AM by manually entering an absence code that indicates illness for those two hours.</span></span>

### <a name="calculate-and-approve-absence"></a><span data-ttu-id="fc34a-181">计算和审核缺勤</span><span class="sxs-lookup"><span data-stu-id="fc34a-181">Calculate and approve absence</span></span>

- <span data-ttu-id="fc34a-182">选择**出勤时间** &gt; **查看和审核** &gt; **审核或计算**。</span><span class="sxs-lookup"><span data-stu-id="fc34a-182">Select **Time attendance** &gt; **Review and approve** &gt; **Approve or Calculate**.</span></span>