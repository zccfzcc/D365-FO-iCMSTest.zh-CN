---
title: 设置供应商发票策略
description: 在您通过使用供应商发票页面过帐供应商发票，以及打开供应商发票政策违规页面时，将运行供应商发票政策。
author: ShivamPandey-msft
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: VendParameters,  SysPolicyListPage, SysPolicyParameters, SysPolicySourceDocumentRuleType, SysPolicy, SysPolicySourceDocumentRule, SysQueryForm, SysQueryTableLookUp, SysQueryPrefixLookUp, SysQueryFieldLookUp
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 4fe8495c20cc3342d396982b9c757e6dac1a5cb7
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56003"
---
# <a name="set-up-vendor-invoice-policies"></a><span data-ttu-id="4dc67-103">设置供应商发票策略</span><span class="sxs-lookup"><span data-stu-id="4dc67-103">Set up vendor invoice policies</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="4dc67-104">在您通过使用供应商发票页面过帐供应商发票，以及打开供应商发票政策违规页面时，将运行供应商发票政策。</span><span class="sxs-lookup"><span data-stu-id="4dc67-104">Vendor invoice policies are run when you post a vendor invoice by using the Vendor invoice page and when you open the vendor invoice Policy violations page.</span></span> <span data-ttu-id="4dc67-105">您还可以配置供应商发票工作流每次运行供应商发票策略发票您提交到工作流。</span><span class="sxs-lookup"><span data-stu-id="4dc67-105">You can also configure the vendor invoice workflow to run vendor invoice policies every time that you submit an invoice to workflow.</span></span> 

<span data-ttu-id="4dc67-106">供应商发票此策略不适用于在发票登记簿或发票日志中创建的发票。</span><span class="sxs-lookup"><span data-stu-id="4dc67-106">Vendor invoice policies do not apply to invoices that were created in the invoice register or invoice journal.</span></span> 

<span data-ttu-id="4dc67-107">发票匹配验证并不使用供应商发票政策，但是，需在应付账款参数页面进行设置。</span><span class="sxs-lookup"><span data-stu-id="4dc67-107">Invoice matching validation does not use vendor invoice policies, but is instead set up in the Accounts payable parameters page.</span></span>

<span data-ttu-id="4dc67-108">此记录使用 USMF 公司演示。</span><span class="sxs-lookup"><span data-stu-id="4dc67-108">This recording uses the USMF demo company.</span></span> <span data-ttu-id="4dc67-109">应付账款经理或会计经理将执行以下步骤。</span><span class="sxs-lookup"><span data-stu-id="4dc67-109">The accounts payable manager or accounting manager role would perform these steps.</span></span> <span data-ttu-id="4dc67-110">在您开始前，请确保选择发票匹配 Configuration Key。</span><span class="sxs-lookup"><span data-stu-id="4dc67-110">Before you begin, make sure that the Invoice matching configuration key is selected.</span></span>


## <a name="prepare-to-create-vendor-invoice-policies"></a><span data-ttu-id="4dc67-111">准备为供应商发票策略</span><span class="sxs-lookup"><span data-stu-id="4dc67-111">Prepare to create vendor invoice policies</span></span>
1. <span data-ttu-id="4dc67-112">转到“应付账款”>“设置”>“应付账款参数”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-112">Go to Accounts payable > Setup > Accounts payable parameters.</span></span>
2. <span data-ttu-id="4dc67-113">单击“发票验证”选项卡。</span><span class="sxs-lookup"><span data-stu-id="4dc67-113">Click the Invoice validation tab.</span></span>
3. <span data-ttu-id="4dc67-114">选择或清除“自动更新发票抬头状态”复选框。</span><span class="sxs-lookup"><span data-stu-id="4dc67-114">Select or clear the Automatically update invoice header status check box.</span></span>
4. <span data-ttu-id="4dc67-115">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-115">Click OK.</span></span>
5. <span data-ttu-id="4dc67-116">在“过帐发票差异”字段中，选择一个选项。</span><span class="sxs-lookup"><span data-stu-id="4dc67-116">In the Post invoice with discrepancies field, select an option.</span></span>
6. <span data-ttu-id="4dc67-117">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="4dc67-117">Close the page.</span></span>
7. <span data-ttu-id="4dc67-118">转到“应付账款”>“政策设置”>“供应商发票政策”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-118">Go to Accounts payable > Policy setup > Vendor invoice policies.</span></span>
8. <span data-ttu-id="4dc67-119">单击“参数”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-119">Click Parameters.</span></span>
9. <span data-ttu-id="4dc67-120">单击“btnAdd”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-120">Click btnAdd.</span></span>
10. <span data-ttu-id="4dc67-121">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="4dc67-121">Close the page.</span></span>

## <a name="create-policy-rule-types-for-vendor-invoices"></a><span data-ttu-id="4dc67-122">创建或更新供应商发票政策规则类型</span><span class="sxs-lookup"><span data-stu-id="4dc67-122">Create policy rule types for vendor invoices</span></span>
1. <span data-ttu-id="4dc67-123">转到“应付账款”>“政策设置”>“供应商发票政策规则类型”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-123">Go to Accounts payable > Policy setup > Vendor invoice policy rule types.</span></span>
2. <span data-ttu-id="4dc67-124">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-124">Click New.</span></span>
3. <span data-ttu-id="4dc67-125">在“规则名称”字段中，输入一个值。</span><span class="sxs-lookup"><span data-stu-id="4dc67-125">In the Rule name field, type a value.</span></span>
4. <span data-ttu-id="4dc67-126">在“描述”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="4dc67-126">In the Description field, type a value.</span></span>
5. <span data-ttu-id="4dc67-127">在“查询名称”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="4dc67-127">In the Query name field, click the drop-down button to open the lookup.</span></span>
6. <span data-ttu-id="4dc67-128">在列表中，找到并选择所需记录。</span><span class="sxs-lookup"><span data-stu-id="4dc67-128">In the list, find and select the desired record.</span></span>
7. <span data-ttu-id="4dc67-129">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="4dc67-129">In the list, click the link in the selected row.</span></span>
8. <span data-ttu-id="4dc67-130">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-130">Click Save.</span></span>
9. <span data-ttu-id="4dc67-131">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="4dc67-131">Close the page.</span></span>

## <a name="define-a-vendor-invoice-policy"></a><span data-ttu-id="4dc67-132">定义一个供应商发票策略</span><span class="sxs-lookup"><span data-stu-id="4dc67-132">Define a vendor invoice policy</span></span>
1. <span data-ttu-id="4dc67-133">转到“应付账款”>“政策设置”>“供应商发票政策”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-133">Go to Accounts payable > Policy setup > Vendor invoice policies.</span></span>
2. <span data-ttu-id="4dc67-134">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-134">Click New.</span></span>
3. <span data-ttu-id="4dc67-135">在“名称”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="4dc67-135">In the Name field, type a value.</span></span>
4. <span data-ttu-id="4dc67-136">在“描述”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="4dc67-136">In the Description field, type a value.</span></span>
5. <span data-ttu-id="4dc67-137">展开或折叠“政策组织”部分。</span><span class="sxs-lookup"><span data-stu-id="4dc67-137">Expand or collapse the Policy organizations section.</span></span>
6. <span data-ttu-id="4dc67-138">在树结构中，选择“美国 Contoso 娱乐系统”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-138">In the tree, select 'Contoso Entertainment System USA'.</span></span>
7. <span data-ttu-id="4dc67-139">单击“添加”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-139">Click Add.</span></span>
8. <span data-ttu-id="4dc67-140">展开或折叠“政策规则”部分。</span><span class="sxs-lookup"><span data-stu-id="4dc67-140">Expand or collapse the Policy rules section.</span></span>
9. <span data-ttu-id="4dc67-141">单击“创建政策规则”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-141">Click Create policy rule.</span></span>
10. <span data-ttu-id="4dc67-142">在“政策规则描述”字段中，输入一项描述。</span><span class="sxs-lookup"><span data-stu-id="4dc67-142">In the Policy rule description field, type a value.</span></span>
11. <span data-ttu-id="4dc67-143">单击“筛选器”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-143">Click Filter.</span></span>
12. <span data-ttu-id="4dc67-144">单击“添加”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-144">Click Add.</span></span>
13. <span data-ttu-id="4dc67-145">在列表中，标记所选的行。</span><span class="sxs-lookup"><span data-stu-id="4dc67-145">In the list, mark the selected row.</span></span>
14. <span data-ttu-id="4dc67-146">在“表格”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="4dc67-146">In the Table field, click the drop-down button to open the lookup.</span></span>
15. <span data-ttu-id="4dc67-147">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="4dc67-147">In the list, click the link in the selected row.</span></span>
16. <span data-ttu-id="4dc67-148">在“派生表”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="4dc67-148">In the Derived table field, click the drop-down button to open the lookup.</span></span>
17. <span data-ttu-id="4dc67-149">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="4dc67-149">In the list, click the link in the selected row.</span></span>
18. <span data-ttu-id="4dc67-150">在名为“字段”的字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="4dc67-150">In the Field field, click the drop-down button to open the lookup.</span></span>
19. <span data-ttu-id="4dc67-151">在名为“字段”的字段中，输入一个值。</span><span class="sxs-lookup"><span data-stu-id="4dc67-151">In the Field field, type a value.</span></span>
20. <span data-ttu-id="4dc67-152">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="4dc67-152">Close the page.</span></span>
21. <span data-ttu-id="4dc67-153">在“标准”字段中，输入一个值。</span><span class="sxs-lookup"><span data-stu-id="4dc67-153">In the Criteria field, type a value.</span></span>
22. <span data-ttu-id="4dc67-154">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-154">Click OK.</span></span>
23. <span data-ttu-id="4dc67-155">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="4dc67-155">Click OK.</span></span>
24. <span data-ttu-id="4dc67-156">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="4dc67-156">Close the page.</span></span>
25. <span data-ttu-id="4dc67-157">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="4dc67-157">Close the page.</span></span>
