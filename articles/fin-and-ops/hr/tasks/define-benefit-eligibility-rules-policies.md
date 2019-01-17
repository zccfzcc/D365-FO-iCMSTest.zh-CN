---
title: 定义福利资格规则和策略
description: 此记录将显示您创建福利资格规则和政策并将规则分配给福利的方法。
author: kherr75
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysPolicySourceDocumentRuleType, SysPolicyListPage, SysPolicy, HcmBenefitEligibilityPolicy, HcmBenefit
audience: Application User
ms.reviewer: rschloma
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: kherr
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 5893b492bdfdc498465700a54fa6af88e88ed465
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55766"
---
# <a name="define-benefit-eligibility-rules-and-policies"></a><span data-ttu-id="accda-103">定义福利资格规则和策略</span><span class="sxs-lookup"><span data-stu-id="accda-103">Define benefit eligibility rules and policies</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="accda-104">此记录将显示您创建福利资格规则和政策并将规则分配给福利的方法。</span><span class="sxs-lookup"><span data-stu-id="accda-104">This recording will show you how you can create benefit eligibility rules and policies and then assign rules to Benefits.</span></span>  

<span data-ttu-id="accda-105">创建此记录时使用的演示数据公司为 USMF。</span><span class="sxs-lookup"><span data-stu-id="accda-105">The demo data company used to create this recording is USMF.</span></span>


## <a name="create-benefit-eligibility-policy-rule-type"></a><span data-ttu-id="accda-106">创建福利资格政策规则类型</span><span class="sxs-lookup"><span data-stu-id="accda-106">Create benefit eligibility policy rule type</span></span>
1. <span data-ttu-id="accda-107">转到“人力资源”>“福利”>“资格”>“福利资格政策规则类型”。</span><span class="sxs-lookup"><span data-stu-id="accda-107">Go to Human resources > Benefits > Eligibility > Benefit eligibility policy rule types.</span></span>
2. <span data-ttu-id="accda-108">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="accda-108">Click New.</span></span>
3. <span data-ttu-id="accda-109">在“规则名称”字段中，输入一个值。</span><span class="sxs-lookup"><span data-stu-id="accda-109">In the Rule name field, type a value.</span></span>
4. <span data-ttu-id="accda-110">在“描述”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="accda-110">In the Description field, type a value.</span></span>
5. <span data-ttu-id="accda-111">在“查询名称”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="accda-111">In the Query name field, click the drop-down button to open the lookup.</span></span>
6. <span data-ttu-id="accda-112">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="accda-112">In the list, click the link in the selected row.</span></span>
7. <span data-ttu-id="accda-113">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="accda-113">Click Save.</span></span>
8. <span data-ttu-id="accda-114">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="accda-114">Close the page.</span></span>

## <a name="benefit-eligibility-policy"></a><span data-ttu-id="accda-115">福利资格策略</span><span class="sxs-lookup"><span data-stu-id="accda-115">Benefit eligibility policy</span></span>
1. <span data-ttu-id="accda-116">转到“人力资源”>“福利”>“资格”>“福利资格政策”。</span><span class="sxs-lookup"><span data-stu-id="accda-116">Go to Human resources > Benefits > Eligibility > Benefit eligibility policies.</span></span>
2. <span data-ttu-id="accda-117">选择一个现有的福利政策。</span><span class="sxs-lookup"><span data-stu-id="accda-117">Select an existing benefit policy.</span></span>
3. <span data-ttu-id="accda-118">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="accda-118">In the list, click the link in the selected row.</span></span>
4. <span data-ttu-id="accda-119">切换“政策组织”部分的扩展。</span><span class="sxs-lookup"><span data-stu-id="accda-119">Toggle the expansion of the Policy organizations sections.</span></span>  <span data-ttu-id="accda-120">在此处可以添加或删除您想要加入政策内的所有组织。</span><span class="sxs-lookup"><span data-stu-id="accda-120">Here you can add or remove any organizations you want to include in the policy.</span></span>
5. <span data-ttu-id="accda-121">展开或折叠“政策规则”部分。</span><span class="sxs-lookup"><span data-stu-id="accda-121">Expand or collapse the Policy rules section.</span></span>
6. <span data-ttu-id="accda-122">在列表中，查找并选择以前创建的政策规则。</span><span class="sxs-lookup"><span data-stu-id="accda-122">In the list find the policy rule previously created.</span></span>
7. <span data-ttu-id="accda-123">单击“创建政策规则”。</span><span class="sxs-lookup"><span data-stu-id="accda-123">Click Create policy rule.</span></span>
8. <span data-ttu-id="accda-124">在“生效日期”字段中，输入您希望政策开始生效的日期。</span><span class="sxs-lookup"><span data-stu-id="accda-124">In the Effective date field, enter the date in which you want the policy to become effective.</span></span>
    * <span data-ttu-id="accda-125">如果您希望这些更改生效，则设置生效日期和结束日期，以允许您以后对策略规则作出更改，并且将来无需返回到策略。</span><span class="sxs-lookup"><span data-stu-id="accda-125">Setting effective and end dates allows you to make future changes to policy rules and removing the need to come back to the policy when you want those changes to take effect.</span></span>  
9. 
    * <span data-ttu-id="accda-126">例如，如果您希望规则仅适用于销售经理，您可以创建 Where 子句进行规定：Where 职位描述等于销售经理。</span><span class="sxs-lookup"><span data-stu-id="accda-126">For example if you wanted the rule to only apply to Sales Managers you could create the Where clause to say: Where position description equals Sales Manager.</span></span>  <span data-ttu-id="accda-127">您可以在规则中设置 And 或 Or 或多个 Where 语句。</span><span class="sxs-lookup"><span data-stu-id="accda-127">You can And or Or multiple Where statements together in the rule.</span></span>  
10. <span data-ttu-id="accda-128">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="accda-128">Click OK.</span></span>
11. <span data-ttu-id="accda-129">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="accda-129">Close the page.</span></span>
12. <span data-ttu-id="accda-130">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="accda-130">Close the page.</span></span>

## <a name="assign-rule-to-benefit"></a><span data-ttu-id="accda-131">分配福利规则</span><span class="sxs-lookup"><span data-stu-id="accda-131">Assign rule to benefit</span></span>
1. <span data-ttu-id="accda-132">转到“人力资源”>“福利”>“福利”。</span><span class="sxs-lookup"><span data-stu-id="accda-132">Go to Human resources > Benefits > Benefits.</span></span>
2. <span data-ttu-id="accda-133">在列表中，找到并选择所需记录。</span><span class="sxs-lookup"><span data-stu-id="accda-133">In the list, find and select the desired record.</span></span>
3. <span data-ttu-id="accda-134">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="accda-134">In the list, click the link in the selected row.</span></span>
4. <span data-ttu-id="accda-135">展开或折叠“资格规则”部分。</span><span class="sxs-lookup"><span data-stu-id="accda-135">Expand or collapse the Eligibility rules section.</span></span>
5. <span data-ttu-id="accda-136">单击“编辑”。</span><span class="sxs-lookup"><span data-stu-id="accda-136">Click Edit.</span></span>
6. <span data-ttu-id="accda-137">在“资格”字段中，从列表选择“规则”。</span><span class="sxs-lookup"><span data-stu-id="accda-137">In the Eligibility field, select Rule based from the list.</span></span>
7. <span data-ttu-id="accda-138">在“规则类型”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="accda-138">In the Rule type field, click the drop down button to open the lookup.</span></span>
8. <span data-ttu-id="accda-139">在列表中，查找并选择以前创建的规则。</span><span class="sxs-lookup"><span data-stu-id="accda-139">In the list find and select the rule you previously created.</span></span>
9. <span data-ttu-id="accda-140">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="accda-140">In the list, click the link in the selected row.</span></span>
10. <span data-ttu-id="accda-141">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="accda-141">Click Save.</span></span>
11. <span data-ttu-id="accda-142">关闭窗体。</span><span class="sxs-lookup"><span data-stu-id="accda-142">Close the form.</span></span>
