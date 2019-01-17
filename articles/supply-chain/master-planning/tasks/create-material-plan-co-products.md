---
title: 创建联产品的物料计划
description: 生产规划员为属于配方联产品的物料规划物料要求。
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: DefaultDashboard, SalesOrderProcessingWorkspace, SalesCreateOrder, SalesTable, ReqCreatePlanWorkspace, ReqTransPlanCard, SysQueryForm, ReqTransPo
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 5eea68096b8a44f00f207c0a82f7f38ff16c4a96
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55070"
---
# <a name="create-a-material-plan-for-co-products"></a><span data-ttu-id="a3353-103">创建联产品的物料计划</span><span class="sxs-lookup"><span data-stu-id="a3353-103">Create a material plan for co products</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="a3353-104">生产规划员为属于配方联产品的物料规划物料要求。</span><span class="sxs-lookup"><span data-stu-id="a3353-104">The production planner plans the material requirements for items that are formula co-products.</span></span> <span data-ttu-id="a3353-105">使用 USP2 公司演示数据创建此过程。</span><span class="sxs-lookup"><span data-stu-id="a3353-105">The demo data company used to create this procedure is USP2.</span></span>


## <a name="create-requirement-for-a-co-product"></a><span data-ttu-id="a3353-106">创建联产品的要求</span><span class="sxs-lookup"><span data-stu-id="a3353-106">Create requirement for a co-product</span></span>
1. <span data-ttu-id="a3353-107">转到“默认仪表板”。</span><span class="sxs-lookup"><span data-stu-id="a3353-107">Go to Default dashboard.</span></span>
2. <span data-ttu-id="a3353-108">点击“销售订单处理和查询”。</span><span class="sxs-lookup"><span data-stu-id="a3353-108">Click Sales order processing and inquiry.</span></span>
3. <span data-ttu-id="a3353-109">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="a3353-109">Click New.</span></span>
4. <span data-ttu-id="a3353-110">单击“销售订单”。</span><span class="sxs-lookup"><span data-stu-id="a3353-110">Click Sales order.</span></span>
5. <span data-ttu-id="a3353-111">在“客户帐户”字段中，输入一个值。</span><span class="sxs-lookup"><span data-stu-id="a3353-111">In the Customer account field, type a value.</span></span>
    * <span data-ttu-id="a3353-112">示例：US-001</span><span class="sxs-lookup"><span data-stu-id="a3353-112">Example: US-001</span></span>  
6. <span data-ttu-id="a3353-113">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="a3353-113">Click OK.</span></span>
7. <span data-ttu-id="a3353-114">在“项目编号”字段中，输入一个值。</span><span class="sxs-lookup"><span data-stu-id="a3353-114">In the Item number field, type a value.</span></span>
    * <span data-ttu-id="a3353-115">示例：P6003</span><span class="sxs-lookup"><span data-stu-id="a3353-115">Example: P6003</span></span>  
8. <span data-ttu-id="a3353-116">在“数量”字段中，输入一个数字。</span><span class="sxs-lookup"><span data-stu-id="a3353-116">In the Quantity field, enter a number.</span></span>
    * <span data-ttu-id="a3353-117">示例：50000</span><span class="sxs-lookup"><span data-stu-id="a3353-117">Example: 50000</span></span>  
9. <span data-ttu-id="a3353-118">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="a3353-118">Click Save.</span></span>

## <a name="create-a-material-plan-for-co-products"></a><span data-ttu-id="a3353-119">创建联产品的物料计划</span><span class="sxs-lookup"><span data-stu-id="a3353-119">Create a material plan for co-products</span></span>
1. <span data-ttu-id="a3353-120">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="a3353-120">Close the page.</span></span>
2. <span data-ttu-id="a3353-121">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="a3353-121">Close the page.</span></span>
3. <span data-ttu-id="a3353-122">单击“主计划”。</span><span class="sxs-lookup"><span data-stu-id="a3353-122">Click Master planning.</span></span>
4. <span data-ttu-id="a3353-123">在“计划”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="a3353-123">In the Plan field, click the drop-down button to open the lookup.</span></span>
5. <span data-ttu-id="a3353-124">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="a3353-124">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="a3353-125">示例：主计划</span><span class="sxs-lookup"><span data-stu-id="a3353-125">Example: MasterPlan</span></span>  
6. <span data-ttu-id="a3353-126">单击“运行”。</span><span class="sxs-lookup"><span data-stu-id="a3353-126">Click Run.</span></span>
7. <span data-ttu-id="a3353-127">展开或折叠包含部分的“记录”。</span><span class="sxs-lookup"><span data-stu-id="a3353-127">Expand or collapse the Records to include section.</span></span>
8. <span data-ttu-id="a3353-128">单击“筛选器”。</span><span class="sxs-lookup"><span data-stu-id="a3353-128">Click Filter.</span></span>
9. <span data-ttu-id="a3353-129">在列表中，选择“字段 = 物料编号”的行。</span><span class="sxs-lookup"><span data-stu-id="a3353-129">In the list, select the row for Field = Item number.</span></span>
10. <span data-ttu-id="a3353-130">在“标准”字段中，输入一个值。</span><span class="sxs-lookup"><span data-stu-id="a3353-130">In the Criteria field, type a value.</span></span>
    * <span data-ttu-id="a3353-131">示例：P6003</span><span class="sxs-lookup"><span data-stu-id="a3353-131">Example: P6003</span></span>  
11. <span data-ttu-id="a3353-132">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="a3353-132">Click OK.</span></span>
12. <span data-ttu-id="a3353-133">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="a3353-133">Click OK.</span></span>
13. <span data-ttu-id="a3353-134">单击“计划订单”。</span><span class="sxs-lookup"><span data-stu-id="a3353-134">Click Planned orders.</span></span>
14. <span data-ttu-id="a3353-135">使用“快速筛选器”以查找记录。</span><span class="sxs-lookup"><span data-stu-id="a3353-135">Use the Quick Filter to find records.</span></span> <span data-ttu-id="a3353-136">例如，使用值“P6000”在“物料编号”字段中进行筛选。</span><span class="sxs-lookup"><span data-stu-id="a3353-136">For example, filter on the Item number field with a value of 'P6000'.</span></span>
    * <span data-ttu-id="a3353-137">根据配方物料筛选，即含有您已创建销售订单的物料的联产品的配方物料。</span><span class="sxs-lookup"><span data-stu-id="a3353-137">Filter by the formula item that has as co-product of the item that you created a sales order for.</span></span>  
15. <span data-ttu-id="a3353-138">在列表中，标记所选的行。</span><span class="sxs-lookup"><span data-stu-id="a3353-138">In the list, mark the selected row.</span></span>
    * <span data-ttu-id="a3353-139">选择筛选器返回的任何行。</span><span class="sxs-lookup"><span data-stu-id="a3353-139">Select any of the rows returned by the filter.</span></span>  
16. <span data-ttu-id="a3353-140">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="a3353-140">In the list, click the link in the selected row.</span></span>
17. <span data-ttu-id="a3353-141">展开或折叠“限定”部分。</span><span class="sxs-lookup"><span data-stu-id="a3353-141">Expand or collapse the Pegging section.</span></span>
18. <span data-ttu-id="a3353-142">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="a3353-142">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="a3353-143">计划订单受到联产品销售订单的限定。</span><span class="sxs-lookup"><span data-stu-id="a3353-143">The planned order is pegged to the sales order for the co-product.</span></span>  
19. <span data-ttu-id="a3353-144">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="a3353-144">Close the page.</span></span>

## <a name="create-requirement-for-a-co-product"></a><span data-ttu-id="a3353-145">创建联产品的要求</span><span class="sxs-lookup"><span data-stu-id="a3353-145">Create requirement for a co-product</span></span>
1. <span data-ttu-id="a3353-146">转到“默认仪表板”。</span><span class="sxs-lookup"><span data-stu-id="a3353-146">Go to Default dashboard.</span></span>
2. <span data-ttu-id="a3353-147">点击“销售订单处理和查询”。</span><span class="sxs-lookup"><span data-stu-id="a3353-147">Click Sales order processing and inquiry.</span></span>
3. <span data-ttu-id="a3353-148">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="a3353-148">Click New.</span></span>
4. <span data-ttu-id="a3353-149">单击“销售订单”。</span><span class="sxs-lookup"><span data-stu-id="a3353-149">Click Sales order.</span></span>
5. <span data-ttu-id="a3353-150">在“客户帐户”字段中，输入一个值。</span><span class="sxs-lookup"><span data-stu-id="a3353-150">In the Customer account field, type a value.</span></span>
    * <span data-ttu-id="a3353-151">示例：US-001</span><span class="sxs-lookup"><span data-stu-id="a3353-151">Example: US-001</span></span>  
6. <span data-ttu-id="a3353-152">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="a3353-152">Click OK.</span></span>
7. <span data-ttu-id="a3353-153">在“项目编号”字段中，输入一个值。</span><span class="sxs-lookup"><span data-stu-id="a3353-153">In the Item number field, type a value.</span></span>
    * <span data-ttu-id="a3353-154">示例：P6003</span><span class="sxs-lookup"><span data-stu-id="a3353-154">Example: P6003</span></span>  
8. <span data-ttu-id="a3353-155">在“数量”字段中，输入一个数字。</span><span class="sxs-lookup"><span data-stu-id="a3353-155">In the Quantity field, enter a number.</span></span>
    * <span data-ttu-id="a3353-156">示例：50000</span><span class="sxs-lookup"><span data-stu-id="a3353-156">Example: 50000</span></span>  
9. <span data-ttu-id="a3353-157">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="a3353-157">Click Save.</span></span>

## <a name="create-a-material-plan-for-co-products"></a><span data-ttu-id="a3353-158">创建联产品的物料计划</span><span class="sxs-lookup"><span data-stu-id="a3353-158">Create a material plan for co-products</span></span>
1. <span data-ttu-id="a3353-159">在“计划”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="a3353-159">In the Plan field, click the drop-down button to open the lookup.</span></span>
2. <span data-ttu-id="a3353-160">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="a3353-160">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="a3353-161">示例：主计划</span><span class="sxs-lookup"><span data-stu-id="a3353-161">Example: MasterPlan</span></span>  
3. <span data-ttu-id="a3353-162">单击“运行”。</span><span class="sxs-lookup"><span data-stu-id="a3353-162">Click Run.</span></span>
4. <span data-ttu-id="a3353-163">展开或折叠包含部分的“记录”。</span><span class="sxs-lookup"><span data-stu-id="a3353-163">Expand or collapse the Records to include section.</span></span>
5. <span data-ttu-id="a3353-164">单击“筛选器”。</span><span class="sxs-lookup"><span data-stu-id="a3353-164">Click Filter.</span></span>
6. <span data-ttu-id="a3353-165">在列表中，选择“字段 = 物料编号”的行。</span><span class="sxs-lookup"><span data-stu-id="a3353-165">In the list, select the row for Field = Item number.</span></span>
7. <span data-ttu-id="a3353-166">在“标准”字段中，输入一个值。</span><span class="sxs-lookup"><span data-stu-id="a3353-166">In the Criteria field, type a value.</span></span>
    * <span data-ttu-id="a3353-167">示例：P6003</span><span class="sxs-lookup"><span data-stu-id="a3353-167">Example: P6003</span></span>  
8. <span data-ttu-id="a3353-168">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="a3353-168">Click OK.</span></span>
9. <span data-ttu-id="a3353-169">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="a3353-169">Click OK.</span></span>
10. <span data-ttu-id="a3353-170">单击“计划订单”。</span><span class="sxs-lookup"><span data-stu-id="a3353-170">Click Planned orders.</span></span>
11. <span data-ttu-id="a3353-171">使用“快速筛选器”以查找记录。</span><span class="sxs-lookup"><span data-stu-id="a3353-171">Use the Quick Filter to find records.</span></span> <span data-ttu-id="a3353-172">例如，使用值“P6000”在“物料编号”字段中进行筛选。</span><span class="sxs-lookup"><span data-stu-id="a3353-172">For example, filter on the Item number field with a value of 'P6000'.</span></span>
    * <span data-ttu-id="a3353-173">根据配方物料筛选，即含有您已创建销售订单的物料的联产品的配方物料。</span><span class="sxs-lookup"><span data-stu-id="a3353-173">Filter by the formula item that has as co-product of the item that you created a sales order for.</span></span>  
12. <span data-ttu-id="a3353-174">在列表中，标记所选的行。</span><span class="sxs-lookup"><span data-stu-id="a3353-174">In the list, mark the selected row.</span></span>
    * <span data-ttu-id="a3353-175">选择筛选器返回的任何行。</span><span class="sxs-lookup"><span data-stu-id="a3353-175">Select any of the rows returned by the filter.</span></span>  
13. <span data-ttu-id="a3353-176">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="a3353-176">In the list, click the link in the selected row.</span></span>
14. <span data-ttu-id="a3353-177">展开或折叠“限定”部分。</span><span class="sxs-lookup"><span data-stu-id="a3353-177">Expand or collapse the Pegging section.</span></span>
15. <span data-ttu-id="a3353-178">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="a3353-178">In the list, click the link in the selected row.</span></span>
    * <span data-ttu-id="a3353-179">计划订单受到联产品销售订单的限定。</span><span class="sxs-lookup"><span data-stu-id="a3353-179">The planned order is pegged to the sales order for the co-product.</span></span>  
16. <span data-ttu-id="a3353-180">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="a3353-180">Close the page.</span></span>
17. <span data-ttu-id="a3353-181">单击“主计划”。</span><span class="sxs-lookup"><span data-stu-id="a3353-181">Click Master planning.</span></span>
18. <span data-ttu-id="a3353-182">转到“主计划”>“设置”>“主计划参数”。</span><span class="sxs-lookup"><span data-stu-id="a3353-182">Go to Master planning > Setup > Master planning parameters.</span></span>
19. <span data-ttu-id="a3353-183">在“禁用所有计划过程”字段中选择“否”。</span><span class="sxs-lookup"><span data-stu-id="a3353-183">Select No in the Disable all planning processes field.</span></span>
20. <span data-ttu-id="a3353-184">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="a3353-184">Close the page.</span></span>

