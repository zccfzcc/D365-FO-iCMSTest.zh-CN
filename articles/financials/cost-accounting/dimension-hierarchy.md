---
title: 维度层次结构
description: 此主题提供有关维度层次结构的信息。 您使用维度层次结构定义成本核算中的报告结构、成本策略和安全设置。
author: AndersGirke
manager: AnnBe
ms.date: 06/16/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CAMDimensionHierarchy,
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: global
ms.search.industry: Manufacturing
ms.author: shylaw
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: 055da6698a192aacc91e29fb3d6f690152ed9623
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56228"
---
# <a name="dimension-hierarchy"></a><span data-ttu-id="9a394-104">维度层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-104">Dimension hierarchy</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="9a394-105">此主题提供有关维度层次结构的信息。</span><span class="sxs-lookup"><span data-stu-id="9a394-105">This topic provides information about dimension hierarchies.</span></span> <span data-ttu-id="9a394-106">您使用维度层次结构定义成本核算中的报告结构、成本策略和安全设置。</span><span class="sxs-lookup"><span data-stu-id="9a394-106">You use a dimension hierarchy to define the reporting structure, cost policies, and security setup in Cost accounting.</span></span>  

## <a name="overview"></a><span data-ttu-id="9a394-107">概览</span><span class="sxs-lookup"><span data-stu-id="9a394-107">Overview</span></span>

<span data-ttu-id="9a394-108">维度层次结构用于成本核算的多个位置。</span><span class="sxs-lookup"><span data-stu-id="9a394-108">Dimension hierarchies are used in various places in Cost accounting.</span></span> <span data-ttu-id="9a394-109">通过维度层次结构可以定义以下信息：</span><span class="sxs-lookup"><span data-stu-id="9a394-109">A dimension hierarchy lets you define the following information:</span></span>

-  <span data-ttu-id="9a394-110">适应组织要求的报告结构</span><span class="sxs-lookup"><span data-stu-id="9a394-110">The reporting structure that fits into the organization's requirements</span></span>
-  <span data-ttu-id="9a394-111">成本策略</span><span class="sxs-lookup"><span data-stu-id="9a394-111">Cost policies</span></span>
-  <span data-ttu-id="9a394-112">安全设置</span><span class="sxs-lookup"><span data-stu-id="9a394-112">The security setup</span></span>

<span data-ttu-id="9a394-113">以下是维度层次结构的示例。</span><span class="sxs-lookup"><span data-stu-id="9a394-113">Here is an example of a dimension hierarchy.</span></span>

![维度层次结构的示例](./media/dimension-hierarchy.png)

<span data-ttu-id="9a394-115">可以为以下维度类型创建维度层次结构：</span><span class="sxs-lookup"><span data-stu-id="9a394-115">A dimension hierarchy can be created for the following types of dimensions:</span></span>

-  <span data-ttu-id="9a394-116">成本元素维度</span><span class="sxs-lookup"><span data-stu-id="9a394-116">Cost element dimensions</span></span>
-  <span data-ttu-id="9a394-117">成本对象维度</span><span class="sxs-lookup"><span data-stu-id="9a394-117">Cost object dimensions</span></span>
-  <span data-ttu-id="9a394-118">统计维度</span><span class="sxs-lookup"><span data-stu-id="9a394-118">Statistical dimensions</span></span>

> [!NOTE]
> - <span data-ttu-id="9a394-119">如果要求不同视角，您可以为相同维度创建多个维度层次结构。</span><span class="sxs-lookup"><span data-stu-id="9a394-119">You can create multiple dimension hierarchies for the same dimension if different perspectives are required.</span></span>
> - <span data-ttu-id="9a394-120">一个维度层次结构只能与一个维度相关联。</span><span class="sxs-lookup"><span data-stu-id="9a394-120">A dimension hierarchy can be associated with only one dimension.</span></span>
> - <span data-ttu-id="9a394-121">一个维度层次结构的结构中可以有无限个级别。</span><span class="sxs-lookup"><span data-stu-id="9a394-121">A dimension hierarchy can have unlimited levels in its structure.</span></span> <span data-ttu-id="9a394-122">所有级别在**成本控制**工作区中可用。</span><span class="sxs-lookup"><span data-stu-id="9a394-122">All the levels will be available in the **Cost control** workspace.</span></span> <span data-ttu-id="9a394-123">出于报告目的使用 Microsoft Excel 或 Microsoft Power BI 时，仅导出维度层次结构的前 15 个级别。</span><span class="sxs-lookup"><span data-stu-id="9a394-123">When you use Microsoft Excel or Microsoft Power BI for reporting purposes, only the first 15 levels of the dimension hierarchy are exported.</span></span> <span data-ttu-id="9a394-124">存在此限制是因为 Excel 和 Power BI 均要求固定架构。</span><span class="sxs-lookup"><span data-stu-id="9a394-124">This limitation exists because both Excel and Power BI require a fixed schema.</span></span>
> - <span data-ttu-id="9a394-125">维度层次结构没有日期限制。</span><span class="sxs-lookup"><span data-stu-id="9a394-125">A dimension hierarchy isn't date-effective.</span></span> <span data-ttu-id="9a394-126">因此，对维度层次结构的任何更改立即保存到记录，且您无法比较此日期之前的维度层次结构和此日期之后的维度层次结构。</span><span class="sxs-lookup"><span data-stu-id="9a394-126">Therefore, any change to a dimension hierarchy is immediately saved to the record, and you can't compare the before date and after date.</span></span>

## <a name="dimension-hierarchy-type"></a><span data-ttu-id="9a394-127">维度层次结构类型</span><span class="sxs-lookup"><span data-stu-id="9a394-127">Dimension hierarchy type</span></span>

<span data-ttu-id="9a394-128">创建新的维度层次结构时，必须选择层次结构类型。</span><span class="sxs-lookup"><span data-stu-id="9a394-128">When you create a new dimension hierarchy, you must select a hierarchy type.</span></span> <span data-ttu-id="9a394-129">转到**成本核算** > **维度** > **维度层次结构**。</span><span class="sxs-lookup"><span data-stu-id="9a394-129">Go to **Cost accounting** > **Dimensions** > **Dimension hierarchies**.</span></span> <span data-ttu-id="9a394-130">单击**新建**，然后选择维度层次结构类型。</span><span class="sxs-lookup"><span data-stu-id="9a394-130">Click **New**, and select a dimension hierarchy type.</span></span> <span data-ttu-id="9a394-131">您可以选择**维度分类层次结构**或**维度分级层次结构**。</span><span class="sxs-lookup"><span data-stu-id="9a394-131">You can select either **Dimension categorization hierarchy** or **Dimension classification hierarchy**.</span></span>

### <a name="dimension-categorization-hierarchy"></a><span data-ttu-id="9a394-132">维度分类层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-132">Dimension categorization hierarchy</span></span>

<span data-ttu-id="9a394-133">**维度分类层次结构**类型用于报告目的。</span><span class="sxs-lookup"><span data-stu-id="9a394-133">The **Dimension categorization hierarchy** type is used for reporting purposes.</span></span> <span data-ttu-id="9a394-134">它仅支持成本元素维度。</span><span class="sxs-lookup"><span data-stu-id="9a394-134">It supports only the cost element dimensions.</span></span> <span data-ttu-id="9a394-135">当您选择此类型时，以下规则适用：</span><span class="sxs-lookup"><span data-stu-id="9a394-135">When you select this type, the following rules apply:</span></span>

-  <span data-ttu-id="9a394-136">一个维度成员在层次结构中可关联多次。</span><span class="sxs-lookup"><span data-stu-id="9a394-136">A dimension member can be associated more than one time in the hierarchy structure.</span></span>
-  <span data-ttu-id="9a394-137">您可以通过将成本行为分配到叶节点的方式将成本元素维度成员放置到不同的节点。</span><span class="sxs-lookup"><span data-stu-id="9a394-137">You can put a cost element dimension member in different nodes by assigning a cost behavior to the leaf node.</span></span>

### <a name="dimension-classification-hierarchy"></a><span data-ttu-id="9a394-138">维度分类层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-138">Dimension classification hierarchy</span></span>

<span data-ttu-id="9a394-139">**维度分级层次结构**类型用于定义规则和用于报告目的。</span><span class="sxs-lookup"><span data-stu-id="9a394-139">The **Dimension classification hierarchy** type is used to define rules and for reporting purposes.</span></span> <span data-ttu-id="9a394-140">它支持所有维度，例如成本对象、成本元素和统计维度。</span><span class="sxs-lookup"><span data-stu-id="9a394-140">It supports all dimensions, such as cost objects, cost elements, and statistical dimensions.</span></span> <span data-ttu-id="9a394-141">当您选择此类型时，一个维度成员在层次结构中仅可关联一次。</span><span class="sxs-lookup"><span data-stu-id="9a394-141">When you select this type, a dimension member can be associated only one time in the hierarchy structure.</span></span>

## <a name="create-and-maintain-a-dimension-hierarchy"></a><span data-ttu-id="9a394-142">创建并维护维度层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-142">Create and maintain a dimension hierarchy</span></span>

<span data-ttu-id="9a394-143">维度层次结构创建为具有节点和叶节点关系的树结构。</span><span class="sxs-lookup"><span data-stu-id="9a394-143">A dimension hierarchy is created as a tree structure that has node and leaf node relationships.</span></span>

-  <span data-ttu-id="9a394-144">一个节点可以具有 1:_n_ 个子节点。</span><span class="sxs-lookup"><span data-stu-id="9a394-144">A node can have 1:_n_ subnodes.</span></span>
-  <span data-ttu-id="9a394-145">一个节点不能同时分配有子节点和叶节点。</span><span class="sxs-lookup"><span data-stu-id="9a394-145">A node can’t have both subnodes and leaf nodes assigned to it.</span></span>
-  <span data-ttu-id="9a394-146">叶节点只能在层次结构的最低级别进行分配。</span><span class="sxs-lookup"><span data-stu-id="9a394-146">A leaf node can be assigned only at the lowest level in the hierarchy.</span></span>

### <a name="example"></a><span data-ttu-id="9a394-147">示例</span><span class="sxs-lookup"><span data-stu-id="9a394-147">Example</span></span>

<span data-ttu-id="9a394-148">一个小公司具有以下组织结构，其中财务和人力资源属于管理部门，装配和包装属于生产部门。</span><span class="sxs-lookup"><span data-stu-id="9a394-148">A small company has the following organization structure, where Finance and Human resources are departments under Admin, and Assembly and Packaging are departments under Production.</span></span>

![组织结构的示例](./media/dimension-hierarchy-org.png)

<span data-ttu-id="9a394-150">成本对象维度表示组织中的所有成本中心。</span><span class="sxs-lookup"><span data-stu-id="9a394-150">A cost object dimension represents all the cost centers in the organization.</span></span>

- <span data-ttu-id="9a394-151">成本对象维度</span><span class="sxs-lookup"><span data-stu-id="9a394-151">Cost object dimension</span></span>
    - <span data-ttu-id="9a394-152">成本中心</span><span class="sxs-lookup"><span data-stu-id="9a394-152">Cost centers</span></span>

<span data-ttu-id="9a394-153">表示所有成本中心的成本对象维度可以按此处所示进行设置。</span><span class="sxs-lookup"><span data-stu-id="9a394-153">The cost object dimension that represents all the cost centers can be set up as shown here.</span></span>

| <span data-ttu-id="9a394-154">成本中心</span><span class="sxs-lookup"><span data-stu-id="9a394-154">Cost centers</span></span> | <span data-ttu-id="9a394-155">说明</span><span class="sxs-lookup"><span data-stu-id="9a394-155">Description</span></span> |
|--------------|-------------|
| <span data-ttu-id="9a394-156">CC001</span><span class="sxs-lookup"><span data-stu-id="9a394-156">CC001</span></span>        | <span data-ttu-id="9a394-157">HR</span><span class="sxs-lookup"><span data-stu-id="9a394-157">HR</span></span>          |
| <span data-ttu-id="9a394-158">CC002</span><span class="sxs-lookup"><span data-stu-id="9a394-158">CC002</span></span>        | <span data-ttu-id="9a394-159">财务</span><span class="sxs-lookup"><span data-stu-id="9a394-159">Finance</span></span>     |
| <span data-ttu-id="9a394-160">CC003</span><span class="sxs-lookup"><span data-stu-id="9a394-160">CC003</span></span>        | <span data-ttu-id="9a394-161">税金</span><span class="sxs-lookup"><span data-stu-id="9a394-161">Tax</span></span>         |
| <span data-ttu-id="9a394-162">CC007</span><span class="sxs-lookup"><span data-stu-id="9a394-162">CC007</span></span>        | <span data-ttu-id="9a394-163">AR/AP</span><span class="sxs-lookup"><span data-stu-id="9a394-163">AR/AP</span></span>       |
| <span data-ttu-id="9a394-164">CC005</span><span class="sxs-lookup"><span data-stu-id="9a394-164">CC005</span></span>        | <span data-ttu-id="9a394-165">程序集</span><span class="sxs-lookup"><span data-stu-id="9a394-165">Assembly</span></span>    |
| <span data-ttu-id="9a394-166">CC006</span><span class="sxs-lookup"><span data-stu-id="9a394-166">CC006</span></span>        | <span data-ttu-id="9a394-167">包装</span><span class="sxs-lookup"><span data-stu-id="9a394-167">Packaging</span></span>   |

<span data-ttu-id="9a394-168">成本元素维度表示组织中的所有成本元素。</span><span class="sxs-lookup"><span data-stu-id="9a394-168">A cost element dimension represents all the cost elements in the organization.</span></span>

- <span data-ttu-id="9a394-169">成本元素维度</span><span class="sxs-lookup"><span data-stu-id="9a394-169">Cost element dimension</span></span>
    - <span data-ttu-id="9a394-170">成本元素</span><span class="sxs-lookup"><span data-stu-id="9a394-170">Cost elements</span></span>

<span data-ttu-id="9a394-171">表示所有成本元素的成本元素维度可以按此处所示进行设置。</span><span class="sxs-lookup"><span data-stu-id="9a394-171">The cost element dimension that represents all the cost elements can be set up as shown here.</span></span>

| <span data-ttu-id="9a394-172">成本元素</span><span class="sxs-lookup"><span data-stu-id="9a394-172">Cost elements</span></span> | <span data-ttu-id="9a394-173">说明</span><span class="sxs-lookup"><span data-stu-id="9a394-173">Description</span></span> |
|---------------|-------------|
| <span data-ttu-id="9a394-174">10001</span><span class="sxs-lookup"><span data-stu-id="9a394-174">10001</span></span>         | <span data-ttu-id="9a394-175">电</span><span class="sxs-lookup"><span data-stu-id="9a394-175">Electricity</span></span> |
| <span data-ttu-id="9a394-176">10010</span><span class="sxs-lookup"><span data-stu-id="9a394-176">10010</span></span>         | <span data-ttu-id="9a394-177">清洗</span><span class="sxs-lookup"><span data-stu-id="9a394-177">Cleaning</span></span>    |
| <span data-ttu-id="9a394-178">10011</span><span class="sxs-lookup"><span data-stu-id="9a394-178">10011</span></span>         | <span data-ttu-id="9a394-179">加热</span><span class="sxs-lookup"><span data-stu-id="9a394-179">Heating</span></span>     |
| <span data-ttu-id="9a394-180">40001</span><span class="sxs-lookup"><span data-stu-id="9a394-180">40001</span></span>         | <span data-ttu-id="9a394-181">COGS</span><span class="sxs-lookup"><span data-stu-id="9a394-181">COGS</span></span>        |

<span data-ttu-id="9a394-182">符合组织报告要求的维度层次结构可以按此处所示进行设置。</span><span class="sxs-lookup"><span data-stu-id="9a394-182">A dimension hierarchy that meets the organizational reporting requirements can be set up as shown here.</span></span>

<span data-ttu-id="9a394-183">**维度层次结构明细**</span><span class="sxs-lookup"><span data-stu-id="9a394-183">**Dimension hierarchy details**</span></span>

| <span data-ttu-id="9a394-184">维度层次结构名称</span><span class="sxs-lookup"><span data-stu-id="9a394-184">Dimension hierarchy name</span></span> | <span data-ttu-id="9a394-185">维度</span><span class="sxs-lookup"><span data-stu-id="9a394-185">Dimension</span></span>    | <span data-ttu-id="9a394-186">维度层次结构类型名称</span><span class="sxs-lookup"><span data-stu-id="9a394-186">Dimension hierarchy type name</span></span>      | <span data-ttu-id="9a394-187">访问列表层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-187">Access list hierarchy</span></span> |
|--------------------------|--------------|------------------------------------|-----------------------|
| <span data-ttu-id="9a394-188">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-188">Organization</span></span>             | <span data-ttu-id="9a394-189">成本中心</span><span class="sxs-lookup"><span data-stu-id="9a394-189">Cost centers</span></span> | <span data-ttu-id="9a394-190">维度分类层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-190">Dimension classification hierarchy</span></span> | <span data-ttu-id="9a394-191">无</span><span class="sxs-lookup"><span data-stu-id="9a394-191">No</span></span>                    |

<span data-ttu-id="9a394-192">用于报告的维度层次结构可以按此处所示进行设置。</span><span class="sxs-lookup"><span data-stu-id="9a394-192">The dimension hierarchy for reporting can be set up as shown here.</span></span>

|                   | <span data-ttu-id="9a394-193">维度成员范围</span><span class="sxs-lookup"><span data-stu-id="9a394-193">Dimension member ranges</span></span>   |                         |
|-------------------|---------------------------|-------------------------|
| <span data-ttu-id="9a394-194">**节点**</span><span class="sxs-lookup"><span data-stu-id="9a394-194">**Nodes**</span></span>         | <span data-ttu-id="9a394-195">**起始维度成员**</span><span class="sxs-lookup"><span data-stu-id="9a394-195">**From dimension member**</span></span> | <span data-ttu-id="9a394-196">**截止维度成员**</span><span class="sxs-lookup"><span data-stu-id="9a394-196">**To dimension member**</span></span> |
| <span data-ttu-id="9a394-197">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-197">Organization</span></span>      |                           |                         |
| <span data-ttu-id="9a394-198">&nbsp;&nbsp;管理</span><span class="sxs-lookup"><span data-stu-id="9a394-198">&nbsp;&nbsp;Admin</span></span>         |                           |                         |
|<span data-ttu-id="9a394-199">&nbsp;&nbsp;&nbsp;&nbsp;财务</span><span class="sxs-lookup"><span data-stu-id="9a394-199">&nbsp;&nbsp;&nbsp;&nbsp;Finance</span></span>   | <span data-ttu-id="9a394-200">CC002</span><span class="sxs-lookup"><span data-stu-id="9a394-200">CC002</span></span>                     | <span data-ttu-id="9a394-201">CC003</span><span class="sxs-lookup"><span data-stu-id="9a394-201">CC003</span></span>                   |
|                   | <span data-ttu-id="9a394-202">CC007</span><span class="sxs-lookup"><span data-stu-id="9a394-202">CC007</span></span>                     | <span data-ttu-id="9a394-203">CC007</span><span class="sxs-lookup"><span data-stu-id="9a394-203">CC007</span></span>                   |
| <span data-ttu-id="9a394-204">&nbsp;&nbsp;&nbsp;&nbsp;HR</span><span class="sxs-lookup"><span data-stu-id="9a394-204">&nbsp;&nbsp;&nbsp;&nbsp;HR</span></span>        | <span data-ttu-id="9a394-205">CC001</span><span class="sxs-lookup"><span data-stu-id="9a394-205">CC001</span></span>                     | <span data-ttu-id="9a394-206">CC001</span><span class="sxs-lookup"><span data-stu-id="9a394-206">CC001</span></span>                   |
| <span data-ttu-id="9a394-207">&nbsp;&nbsp;生产</span><span class="sxs-lookup"><span data-stu-id="9a394-207">&nbsp;&nbsp;Production</span></span>    |                           |                         |
| <span data-ttu-id="9a394-208">&nbsp;&nbsp;&nbsp;&nbsp;包装</span><span class="sxs-lookup"><span data-stu-id="9a394-208">&nbsp;&nbsp;&nbsp;&nbsp;Packaging</span></span> | <span data-ttu-id="9a394-209">CC005</span><span class="sxs-lookup"><span data-stu-id="9a394-209">CC005</span></span>                     | <span data-ttu-id="9a394-210">CC005</span><span class="sxs-lookup"><span data-stu-id="9a394-210">CC005</span></span>                   |
| <span data-ttu-id="9a394-211">&nbsp;&nbsp;&nbsp;&nbsp;程序集</span><span class="sxs-lookup"><span data-stu-id="9a394-211">&nbsp;&nbsp;&nbsp;&nbsp;Assembly</span></span>  | <span data-ttu-id="9a394-212">CC006</span><span class="sxs-lookup"><span data-stu-id="9a394-212">CC006</span></span>                     | <span data-ttu-id="9a394-213">CC006</span><span class="sxs-lookup"><span data-stu-id="9a394-213">CC006</span></span>                   |

<span data-ttu-id="9a394-214">符合策略要求的维度层次结构可以按此处所示进行设置。</span><span class="sxs-lookup"><span data-stu-id="9a394-214">A dimension hierarchy that meets the policy requirement can be set up as shown here.</span></span>

<span data-ttu-id="9a394-215">**维度层次结构明细**</span><span class="sxs-lookup"><span data-stu-id="9a394-215">**Dimension hierarchy details**</span></span>

| <span data-ttu-id="9a394-216">维度层次结构名称</span><span class="sxs-lookup"><span data-stu-id="9a394-216">Dimension hierarchy name</span></span> | <span data-ttu-id="9a394-217">维度</span><span class="sxs-lookup"><span data-stu-id="9a394-217">Dimension</span></span>     | <span data-ttu-id="9a394-218">维度层次结构类型名称</span><span class="sxs-lookup"><span data-stu-id="9a394-218">Dimension hierarchy type name</span></span>      |
|--------------------------|---------------|------------------------------------|
| <span data-ttu-id="9a394-219">成本行为</span><span class="sxs-lookup"><span data-stu-id="9a394-219">Cost behavior</span></span>            | <span data-ttu-id="9a394-220">成本元素</span><span class="sxs-lookup"><span data-stu-id="9a394-220">Cost elements</span></span> | <span data-ttu-id="9a394-221">维度分类层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-221">Dimension classification hierarchy</span></span> |

<span data-ttu-id="9a394-222">用于策略的维度层次结构可以按此处所示进行设置。</span><span class="sxs-lookup"><span data-stu-id="9a394-222">The dimension hierarchy for the policy can be set up as shown here.</span></span>

|                   | <span data-ttu-id="9a394-223">维度成员范围</span><span class="sxs-lookup"><span data-stu-id="9a394-223">Dimension member ranges</span></span>   |                         |
|-------------------|---------------------------|-------------------------|
| <span data-ttu-id="9a394-224">**节点**</span><span class="sxs-lookup"><span data-stu-id="9a394-224">**Nodes**</span></span>         | <span data-ttu-id="9a394-225">**起始维度成员**</span><span class="sxs-lookup"><span data-stu-id="9a394-225">**From dimension member**</span></span> | <span data-ttu-id="9a394-226">**截止维度成员**</span><span class="sxs-lookup"><span data-stu-id="9a394-226">**To dimension member**</span></span> |
| <span data-ttu-id="9a394-227">成本行为</span><span class="sxs-lookup"><span data-stu-id="9a394-227">Cost behavior</span></span>     |                           |                         |
| <span data-ttu-id="9a394-228">&nbsp;&nbsp;固定成本</span><span class="sxs-lookup"><span data-stu-id="9a394-228">&nbsp;&nbsp;Fixed cost</span></span>    | <span data-ttu-id="9a394-229">10001</span><span class="sxs-lookup"><span data-stu-id="9a394-229">10001</span></span>                     | <span data-ttu-id="9a394-230">10011</span><span class="sxs-lookup"><span data-stu-id="9a394-230">10011</span></span>                   |
|<span data-ttu-id="9a394-231">&nbsp;&nbsp;可变成本</span><span class="sxs-lookup"><span data-stu-id="9a394-231">&nbsp;&nbsp;Variable cost</span></span> | <span data-ttu-id="9a394-232">40001</span><span class="sxs-lookup"><span data-stu-id="9a394-232">40001</span></span>                     | <span data-ttu-id="9a394-233">40010</span><span class="sxs-lookup"><span data-stu-id="9a394-233">40010</span></span>                   |

> [!NOTE]
> <span data-ttu-id="9a394-234">在**维度成员范围**下，一个节点可以包含 1:_n_ 个维度成员范围。</span><span class="sxs-lookup"><span data-stu-id="9a394-234">Under **Dimension member ranges**, a node can contain 1:_n_ dimension member ranges.</span></span> <span data-ttu-id="9a394-235">您可以插入尚未作为维度成员存在的维度成员 ID。</span><span class="sxs-lookup"><span data-stu-id="9a394-235">You can insert dimension member IDs that don’t yet exist as dimension members.</span></span> <span data-ttu-id="9a394-236">此方法使层次结构可以弹性地适应未来的需求。</span><span class="sxs-lookup"><span data-stu-id="9a394-236">This approach makes the hierarchy resilient for the future.</span></span>  

### <a name="copy-a-hierarchy"></a><span data-ttu-id="9a394-237">复制层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-237">Copy a hierarchy</span></span>

<span data-ttu-id="9a394-238">您可以复制当前维度层次结构作为新维度层次结构的起始点。</span><span class="sxs-lookup"><span data-stu-id="9a394-238">You can copy a current dimension hierarchy as the starting point for a new dimension hierarchy.</span></span> <span data-ttu-id="9a394-239">如果您要比较之前的维度层次结构与新的维度层次结构，则此方法很有用。</span><span class="sxs-lookup"><span data-stu-id="9a394-239">This approach can be useful if you want to compare the previous dimension hierarchy to the new dimension hierarchy.</span></span>

### <a name="rearrange-nodes-in-a-hierarchy"></a><span data-ttu-id="9a394-240">重新排列层次结构中的节点</span><span class="sxs-lookup"><span data-stu-id="9a394-240">Rearrange nodes in a hierarchy</span></span>

<span data-ttu-id="9a394-241">您可以将节点在结构的当前级别范围内上移和下移。</span><span class="sxs-lookup"><span data-stu-id="9a394-241">You can move a node up and down within its current level in the structure.</span></span> <span data-ttu-id="9a394-242">通过此方法可以重新排列用于报告的节点在**成本控制**工作区中的顺序。</span><span class="sxs-lookup"><span data-stu-id="9a394-242">In this way, you can rearrange the order of nodes for reporting in the **Cost control** workspace.</span></span>

<span data-ttu-id="9a394-243">您可以通过选择目标节点将节点移动到层次结构中的新位置。</span><span class="sxs-lookup"><span data-stu-id="9a394-243">You move a node to a new location in the hierarchy by selecting the target node.</span></span> <span data-ttu-id="9a394-244">可通过两种方式移动节点：</span><span class="sxs-lookup"><span data-stu-id="9a394-244">There are two ways to move a node:</span></span>

- <span data-ttu-id="9a394-245">**下移** - 将所选节点从层次结构中的当前位置移动并插入到选定目标节点的**下方**。</span><span class="sxs-lookup"><span data-stu-id="9a394-245">**Move below** – Move the selected node from its current position in the hierarchy, and insert it **under** the selected target node.</span></span>
- <span data-ttu-id="9a394-246">**后移** - 将所选节点从层次结构中的当前位置移动并插入到它的层次结构级别的选定目标节点的**后面**。</span><span class="sxs-lookup"><span data-stu-id="9a394-246">**Move after** – Move the selected node from its current position in the hierarchy, and insert it **after** the selected target node at its level of the hierarchy.</span></span>

> [!NOTE] 
> <span data-ttu-id="9a394-247">在您将数据导出到 Excel 或 Power BI 时，不维持节点的顺序，因为这些工具默认使用按字母顺序排序。</span><span class="sxs-lookup"><span data-stu-id="9a394-247">The order of the nodes isn't maintained when you export data to Excel or Power BI, because those tools use an alphanumeric sort order by default.</span></span> <span data-ttu-id="9a394-248">您应手动重新排列顺序。</span><span class="sxs-lookup"><span data-stu-id="9a394-248">You should manually rearrange the order.</span></span>

## <a name="define-dimension-hierarchies-for-reporting"></a><span data-ttu-id="9a394-249">定义用于报告的维度层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-249">Define dimension hierarchies for reporting</span></span>

<span data-ttu-id="9a394-250">维度层次结构对于报告十分重要。</span><span class="sxs-lookup"><span data-stu-id="9a394-250">Dimension hierarchies are important for reporting.</span></span> <span data-ttu-id="9a394-251">您可以通过它们定义适应单个组织的特定结构。</span><span class="sxs-lookup"><span data-stu-id="9a394-251">They let you define the specific structure that fits into the individual organization.</span></span> <span data-ttu-id="9a394-252">在维度层次级别的节点级别完成的合并让组织任何级别的利益干系人可以看到任何级别的数据。</span><span class="sxs-lookup"><span data-stu-id="9a394-252">The aggregations that are done at the node level of the dimension hierarchy let stakeholders at any level of the organization see data at any level.</span></span>

<span data-ttu-id="9a394-253">维度层次结构可用于以下报告工具。</span><span class="sxs-lookup"><span data-stu-id="9a394-253">Dimension hierarchies are available in the following reporting tools.</span></span> <span data-ttu-id="9a394-254">此方法有助于保证报告结构中的一致性。</span><span class="sxs-lookup"><span data-stu-id="9a394-254">This approach helps guarantee consistency in the reporting structure.</span></span>

- <span data-ttu-id="9a394-255">**成本控制**工作区（客户端）：</span><span class="sxs-lookup"><span data-stu-id="9a394-255">**Cost control** workspace (Client):</span></span>

    - <span data-ttu-id="9a394-256">通过配置控制。</span><span class="sxs-lookup"><span data-stu-id="9a394-256">Controlled by configuration.</span></span>

- <span data-ttu-id="9a394-257">**成本控制**工作区（移动应用）：</span><span class="sxs-lookup"><span data-stu-id="9a394-257">**Cost control** workspace (Mobile application):</span></span>

    - <span data-ttu-id="9a394-258">通过配置控制。</span><span class="sxs-lookup"><span data-stu-id="9a394-258">Controlled by configuration.</span></span>

- <span data-ttu-id="9a394-259">Excel</span><span class="sxs-lookup"><span data-stu-id="9a394-259">Excel</span></span>

    - <span data-ttu-id="9a394-260">提供选项用于按导出定义选择特定的维度层次结构：</span><span class="sxs-lookup"><span data-stu-id="9a394-260">Provides the option to select specific dimension hierarchies per export definition:</span></span>

        - <span data-ttu-id="9a394-261">一个成本元素维度层次结构（必需）</span><span class="sxs-lookup"><span data-stu-id="9a394-261">One cost element dimension hierarchy (mandatory)</span></span>
        - <span data-ttu-id="9a394-262">一个成本对象维度层次结构（可选）</span><span class="sxs-lookup"><span data-stu-id="9a394-262">One cost object dimension hierarchy (optional)</span></span>
        - <span data-ttu-id="9a394-263">一个统计维度层次结构（可选）</span><span class="sxs-lookup"><span data-stu-id="9a394-263">One statistical dimension hierarchy (optional)</span></span>

- <span data-ttu-id="9a394-264">Power BI：</span><span class="sxs-lookup"><span data-stu-id="9a394-264">Power BI:</span></span>

    - <span data-ttu-id="9a394-265">所有维度层次结构可用。</span><span class="sxs-lookup"><span data-stu-id="9a394-265">All dimension hierarchies are available.</span></span>
    
<span data-ttu-id="9a394-266">如果使用 Excel 或 Power BI 创建报表，则仅导出维度层次结构的前 15 个级别。</span><span class="sxs-lookup"><span data-stu-id="9a394-266">If you create reports by using Excel or Power BI, only the first 15 levels of the dimension hierarchies are exported.</span></span> <span data-ttu-id="9a394-267">存在此限制是因为在 Excel 和 Power BI 中均要求固定架构。</span><span class="sxs-lookup"><span data-stu-id="9a394-267">This limitation exists because a fixed schema is required in Excel and Power BI.</span></span> <span data-ttu-id="9a394-268">如果一个层次结构有 15 个以上级别，则不会导出额外级别。</span><span class="sxs-lookup"><span data-stu-id="9a394-268">If a hierarchy has more than 15 levels, the additional levels won't be exported.</span></span> <span data-ttu-id="9a394-269">标准化表包含层次结构中各维度成员的记录。</span><span class="sxs-lookup"><span data-stu-id="9a394-269">The normalized table contains a record for each dimension member in the hierarchy.</span></span> <span data-ttu-id="9a394-270">因此发生自动化合并。</span><span class="sxs-lookup"><span data-stu-id="9a394-270">Therefore, automated aggregation occurs.</span></span> <span data-ttu-id="9a394-271">此行为有助于保证层次结构中的 15 个可用级别的任何一个级别的余额仍然正确。</span><span class="sxs-lookup"><span data-stu-id="9a394-271">This behavior helps guarantee that the balances at any of the 15 available levels in the hierarchy are still correct.</span></span>

<span data-ttu-id="9a394-272">以下示例显示维度层次结构在报告结构中可能是什么样子。</span><span class="sxs-lookup"><span data-stu-id="9a394-272">The following example shows what a dimension hierarchy might look like in the reporting structure.</span></span>

| <span data-ttu-id="9a394-273">成本对象维度层次结构 - 级别 1</span><span class="sxs-lookup"><span data-stu-id="9a394-273">Cost object dimension hierarchy – Level 1</span></span> | <span data-ttu-id="9a394-274">成本对象维度层次结构 - 级别 2</span><span class="sxs-lookup"><span data-stu-id="9a394-274">Cost object dimension hierarchy – Level 2</span></span> | <span data-ttu-id="9a394-275">成本对象维度层次结构 - 级别 3</span><span class="sxs-lookup"><span data-stu-id="9a394-275">Cost object dimension hierarchy – Level 3</span></span> | <span data-ttu-id="9a394-276">成本对象维度层次结构 - 级别 4</span><span class="sxs-lookup"><span data-stu-id="9a394-276">Cost object dimension hierarchy – Level 4</span></span> | <span data-ttu-id="9a394-277">成本对象维度层次结构 - 级别 15</span><span class="sxs-lookup"><span data-stu-id="9a394-277">Cost object dimension hierarchy – Level 15</span></span> |
|-------------------------------------------|-------------------------------------------|-------------------------------------------|-------------------------------------------|--------------------------------------------|
| <span data-ttu-id="9a394-278">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-278">Organization</span></span>                              | <span data-ttu-id="9a394-279">管理</span><span class="sxs-lookup"><span data-stu-id="9a394-279">Admin</span></span>                                     | <span data-ttu-id="9a394-280">财务</span><span class="sxs-lookup"><span data-stu-id="9a394-280">Finance</span></span>                                   | <span data-ttu-id="9a394-281">CC002</span><span class="sxs-lookup"><span data-stu-id="9a394-281">CC002</span></span>                                     |                                            |
| <span data-ttu-id="9a394-282">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-282">Organization</span></span>                              | <span data-ttu-id="9a394-283">管理</span><span class="sxs-lookup"><span data-stu-id="9a394-283">Admin</span></span>                                     | <span data-ttu-id="9a394-284">财务</span><span class="sxs-lookup"><span data-stu-id="9a394-284">Finance</span></span>                                   | <span data-ttu-id="9a394-285">CC003</span><span class="sxs-lookup"><span data-stu-id="9a394-285">CC003</span></span>                                     |                                            |
| <span data-ttu-id="9a394-286">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-286">Organization</span></span>                              | <span data-ttu-id="9a394-287">管理</span><span class="sxs-lookup"><span data-stu-id="9a394-287">Admin</span></span>                                     | <span data-ttu-id="9a394-288">财务</span><span class="sxs-lookup"><span data-stu-id="9a394-288">Finance</span></span>                                   | <span data-ttu-id="9a394-289">CC007</span><span class="sxs-lookup"><span data-stu-id="9a394-289">CC007</span></span>                                     |                                            |
| <span data-ttu-id="9a394-290">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-290">Organization</span></span>                              | <span data-ttu-id="9a394-291">管理</span><span class="sxs-lookup"><span data-stu-id="9a394-291">Admin</span></span>                                     | <span data-ttu-id="9a394-292">HR</span><span class="sxs-lookup"><span data-stu-id="9a394-292">HR</span></span>                                        | <span data-ttu-id="9a394-293">CC001</span><span class="sxs-lookup"><span data-stu-id="9a394-293">CC001</span></span>                                     |                                            |
| <span data-ttu-id="9a394-294">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-294">Organization</span></span>                              | <span data-ttu-id="9a394-295">生产</span><span class="sxs-lookup"><span data-stu-id="9a394-295">Production</span></span>                                | <span data-ttu-id="9a394-296">包装</span><span class="sxs-lookup"><span data-stu-id="9a394-296">Packaging</span></span>                                 | <span data-ttu-id="9a394-297">CC005</span><span class="sxs-lookup"><span data-stu-id="9a394-297">CC005</span></span>                                     |                                            |
| <span data-ttu-id="9a394-298">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-298">Organization</span></span>                              | <span data-ttu-id="9a394-299">生产</span><span class="sxs-lookup"><span data-stu-id="9a394-299">Production</span></span>                                | <span data-ttu-id="9a394-300">程序集</span><span class="sxs-lookup"><span data-stu-id="9a394-300">Assembly</span></span>                                  | <span data-ttu-id="9a394-301">CC006</span><span class="sxs-lookup"><span data-stu-id="9a394-301">CC006</span></span>                                     |                                            |

### <a name="update-the-dimension-hierarchies-that-are-used-for-reporting"></a><span data-ttu-id="9a394-302">更新用于报告的维度层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-302">Update the dimension hierarchies that are used for reporting</span></span> 

<span data-ttu-id="9a394-303">在一段时间后，必须更新在前面提及的报告工具中使用的维度层次结构。</span><span class="sxs-lookup"><span data-stu-id="9a394-303">Over time, the dimension hierarchies that are used in the previously mentioned reporting tools will have to be updated.</span></span> <span data-ttu-id="9a394-304">您可以通过刷新客户端更新维度层次结构。</span><span class="sxs-lookup"><span data-stu-id="9a394-304">You can update dimension hierarchies by refreshing the client.</span></span>

- <span data-ttu-id="9a394-305">**成本控制**工作区（客户端）</span><span class="sxs-lookup"><span data-stu-id="9a394-305">**Cost control** workspace (Client)</span></span>
- <span data-ttu-id="9a394-306">**成本控制**工作区（移动应用）</span><span class="sxs-lookup"><span data-stu-id="9a394-306">**Cost control** workspace (Mobile application)</span></span>

<span data-ttu-id="9a394-307">对维度层次结构的更新每 24 小时由预缓存作业提取。</span><span class="sxs-lookup"><span data-stu-id="9a394-307">Updates to dimension hierarchies are picked up every 24 hours by a pre-cached job.</span></span> <span data-ttu-id="9a394-308">更新导出数据后，更新的维度层次结构可用于以下工具：</span><span class="sxs-lookup"><span data-stu-id="9a394-308">After the exported data is updated, the updated dimension hierarchies are available in the following tools:</span></span>

- <span data-ttu-id="9a394-309">Excel</span><span class="sxs-lookup"><span data-stu-id="9a394-309">Excel</span></span>
- <span data-ttu-id="9a394-310">Power BI</span><span class="sxs-lookup"><span data-stu-id="9a394-310">Power BI</span></span>

> [!NOTE] 
> <span data-ttu-id="9a394-311">要手动触发维度层次结构缓存的更新，您可以为必须更新的一个或多个维度层次结构新建导出到 Excel。</span><span class="sxs-lookup"><span data-stu-id="9a394-311">To manually trigger an update of the dimension hierarchy cache, you can create a new export to Excel for the dimension hierarchy or hierarchies that must be updated.</span></span>

## <a name="define-dimension-hierarchies-for-cost-policies"></a><span data-ttu-id="9a394-312">定义用于成本策略的维度层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-312">Define dimension hierarchies for cost policies</span></span>

<span data-ttu-id="9a394-313">成本核算包括定义了详细规则的多个策略。</span><span class="sxs-lookup"><span data-stu-id="9a394-313">Cost accounting consists of multiple policies where detailed rules are defined.</span></span> <span data-ttu-id="9a394-314">您必须定义以下策略的一个或多个维度层次结构：</span><span class="sxs-lookup"><span data-stu-id="9a394-314">You must define one or more dimension hierarchies for the following policies:</span></span>

- <span data-ttu-id="9a394-315">成本行为</span><span class="sxs-lookup"><span data-stu-id="9a394-315">Cost behavior</span></span>
- <span data-ttu-id="9a394-316">成本分配</span><span class="sxs-lookup"><span data-stu-id="9a394-316">Cost distribution</span></span>
- <span data-ttu-id="9a394-317">成本分摊</span><span class="sxs-lookup"><span data-stu-id="9a394-317">Cost allocation</span></span>
- <span data-ttu-id="9a394-318">成本累积</span><span class="sxs-lookup"><span data-stu-id="9a394-318">Cost rollup</span></span>

<span data-ttu-id="9a394-319">维度层次结构将便于创建规则。</span><span class="sxs-lookup"><span data-stu-id="9a394-319">Dimension hierarchies make it easy to create rules.</span></span> <span data-ttu-id="9a394-320">若要避免必须为每个维度成员创建规则，您可以利用按维度层次结构级别提供的维度成员的合并。</span><span class="sxs-lookup"><span data-stu-id="9a394-320">To avoid having to create rules for every dimension member, you can take advantage of the aggregations of dimension members that are provided by dimension hierarchy levels.</span></span> <span data-ttu-id="9a394-321">如果您具有重叠规则，您必须定义系统在执行开销计算时将考虑的特定规则。</span><span class="sxs-lookup"><span data-stu-id="9a394-321">If you have overlapping rules, you must define specific rules that the system will consider when it does the overhead calculation.</span></span>

### <a name="example-define-a-cost-behavior-policy"></a><span data-ttu-id="9a394-322">示例：定义成本行为策略</span><span class="sxs-lookup"><span data-stu-id="9a394-322">Example: Define a cost behavior policy</span></span>

<span data-ttu-id="9a394-323">创建新的成本行为策略，且为策略分配相应的维度层次结构，如此处所示。</span><span class="sxs-lookup"><span data-stu-id="9a394-323">A new cost behavior policy is created, and appropriate dimension hierarchies are assigned to the policy, as shown here.</span></span>

<span data-ttu-id="9a394-324">**成本行为策略**</span><span class="sxs-lookup"><span data-stu-id="9a394-324">**Cost behavior policy**</span></span>

| <span data-ttu-id="9a394-325">策略名称</span><span class="sxs-lookup"><span data-stu-id="9a394-325">Policy name</span></span>   | <span data-ttu-id="9a394-326">成本元素维度层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-326">Cost element dimension hierarchy</span></span> | <span data-ttu-id="9a394-327">成本对象维度层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-327">Cost object dimension hierarchy</span></span> | <span data-ttu-id="9a394-328">记帐币种</span><span class="sxs-lookup"><span data-stu-id="9a394-328">Accounting currency</span></span> |
|---------------|----------------------------------|---------------------------------|---------------------|
| <span data-ttu-id="9a394-329">成本行为</span><span class="sxs-lookup"><span data-stu-id="9a394-329">Cost behavior</span></span> | <span data-ttu-id="9a394-330">成本行为</span><span class="sxs-lookup"><span data-stu-id="9a394-330">Cost behavior</span></span>                    | <span data-ttu-id="9a394-331">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-331">Organization</span></span>                    | <span data-ttu-id="9a394-332">美元</span><span class="sxs-lookup"><span data-stu-id="9a394-332">USD</span></span>                 |

<span data-ttu-id="9a394-333">**规则**</span><span class="sxs-lookup"><span data-stu-id="9a394-333">**Rules**</span></span>

| <span data-ttu-id="9a394-334">成本元素维度层次结构节点</span><span class="sxs-lookup"><span data-stu-id="9a394-334">Cost element dimension hierarchy node</span></span> | <span data-ttu-id="9a394-335">成本对象维度层次结构节点</span><span class="sxs-lookup"><span data-stu-id="9a394-335">Cost object dimension hierarchy node</span></span> | <span data-ttu-id="9a394-336">固定百分比</span><span class="sxs-lookup"><span data-stu-id="9a394-336">Fixed percentage</span></span> | <span data-ttu-id="9a394-337">固定金额</span><span class="sxs-lookup"><span data-stu-id="9a394-337">Fixed amount</span></span> | <span data-ttu-id="9a394-338">生效日期</span><span class="sxs-lookup"><span data-stu-id="9a394-338">Valid from</span></span> | <span data-ttu-id="9a394-339">失效日期</span><span class="sxs-lookup"><span data-stu-id="9a394-339">Valid to</span></span> |
|---------------------------------------|--------------------------------------|------------------|--------------|------------|----------|
| <span data-ttu-id="9a394-340">固定成本</span><span class="sxs-lookup"><span data-stu-id="9a394-340">Fixed cost</span></span>                            | <span data-ttu-id="9a394-341">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-341">Organization</span></span>                         | <span data-ttu-id="9a394-342">100.00</span><span class="sxs-lookup"><span data-stu-id="9a394-342">100.00</span></span>           | <span data-ttu-id="9a394-343">0.00</span><span class="sxs-lookup"><span data-stu-id="9a394-343">0.00</span></span>         | <span data-ttu-id="9a394-344">1/1/2017</span><span class="sxs-lookup"><span data-stu-id="9a394-344">1/1/2017</span></span>   | <span data-ttu-id="9a394-345">从不</span><span class="sxs-lookup"><span data-stu-id="9a394-345">Never</span></span>    |
| <span data-ttu-id="9a394-346">10001</span><span class="sxs-lookup"><span data-stu-id="9a394-346">10001</span></span>                                 | <span data-ttu-id="9a394-347">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-347">Organization</span></span>                         | <span data-ttu-id="9a394-348">0.00</span><span class="sxs-lookup"><span data-stu-id="9a394-348">0.00</span></span>             | <span data-ttu-id="9a394-349">150.00</span><span class="sxs-lookup"><span data-stu-id="9a394-349">150.00</span></span>       | <span data-ttu-id="9a394-350">1/1/2017</span><span class="sxs-lookup"><span data-stu-id="9a394-350">1/1/2017</span></span>   | <span data-ttu-id="9a394-351">从不</span><span class="sxs-lookup"><span data-stu-id="9a394-351">Never</span></span>    |
| <span data-ttu-id="9a394-352">10001（“\*”）</span><span class="sxs-lookup"><span data-stu-id="9a394-352">10001 (\*)</span></span>                             | <span data-ttu-id="9a394-353">财务</span><span class="sxs-lookup"><span data-stu-id="9a394-353">Finance</span></span>                              |                  | <span data-ttu-id="9a394-354">50.00</span><span class="sxs-lookup"><span data-stu-id="9a394-354">50.00</span></span>        | <span data-ttu-id="9a394-355">1/1/2017</span><span class="sxs-lookup"><span data-stu-id="9a394-355">1/1/2017</span></span>   | <span data-ttu-id="9a394-356">从不</span><span class="sxs-lookup"><span data-stu-id="9a394-356">Never</span></span>    |
| <span data-ttu-id="9a394-357">成本行为或可变成本 (\*\*)</span><span class="sxs-lookup"><span data-stu-id="9a394-357">Cost behavior or Variable cost (\*\*)</span></span>   | <span data-ttu-id="9a394-358">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-358">Organization</span></span>                         | <span data-ttu-id="9a394-359">0.00</span><span class="sxs-lookup"><span data-stu-id="9a394-359">0.00</span></span>             | <span data-ttu-id="9a394-360">0.00</span><span class="sxs-lookup"><span data-stu-id="9a394-360">0.00</span></span>         | <span data-ttu-id="9a394-361">1/1/2017</span><span class="sxs-lookup"><span data-stu-id="9a394-361">1/1/2017</span></span>   | <span data-ttu-id="9a394-362">从不</span><span class="sxs-lookup"><span data-stu-id="9a394-362">Never</span></span>    |

<span data-ttu-id="9a394-363">\* 不要求可变成本节点。</span><span class="sxs-lookup"><span data-stu-id="9a394-363">\* The variable cost node isn't required.</span></span> <span data-ttu-id="9a394-364">如果成本未分类为固定成本，则它必须是可变成本。</span><span class="sxs-lookup"><span data-stu-id="9a394-364">If a cost isn't classified as a fixed cost, it must be a variable cost.</span></span>

<span data-ttu-id="9a394-365">\*\* 为成本元素成员 10001 和在财务层次结构级别下合并的所有成本对象成员（CC002、CC003、CC007）的组合创建详细规则。</span><span class="sxs-lookup"><span data-stu-id="9a394-365">\*\* A detailed rule is created for the combination of cost element member 10001 and all cost object members that are aggregated under the Finance hierarchy level (CC002, CC003, CC007).</span></span>

<span data-ttu-id="9a394-366">之前的规则显示了维度层次结构提供的灵活性。</span><span class="sxs-lookup"><span data-stu-id="9a394-366">The preceding rules show the flexibility that dimension hierarchies provide.</span></span> <span data-ttu-id="9a394-367">通过定义高级别规则，您可以帮助尽量减少维护。</span><span class="sxs-lookup"><span data-stu-id="9a394-367">By defining high-level rules, you can help minimize maintenance.</span></span> <span data-ttu-id="9a394-368">然后，您可以定义详细规则以适应特定的业务目标。</span><span class="sxs-lookup"><span data-stu-id="9a394-368">You can then define detailed rules to fit into a specific business objective.</span></span>

<span data-ttu-id="9a394-369">如果在规则中使用的维度层次结构被更新，系统将自动提供更新。</span><span class="sxs-lookup"><span data-stu-id="9a394-369">If the dimension hierarchies that are used in rules are updated, the system automatically brings the updates forward.</span></span>

<span data-ttu-id="9a394-370">如果不再需要规则中的精细程度级别，可终止规则。</span><span class="sxs-lookup"><span data-stu-id="9a394-370">If a level of granularity in the rules is no longer required, the rule can be expired.</span></span>

<span data-ttu-id="9a394-371">例如，不再需要财务成本对象维度层次结构节点的特定成本行为规则。</span><span class="sxs-lookup"><span data-stu-id="9a394-371">For example, a specific cost behavior rule for the Finance cost object dimension hierarchy node is no longer required.</span></span> <span data-ttu-id="9a394-372">在这种情况下，请单击**终止规则**来终止规则。</span><span class="sxs-lookup"><span data-stu-id="9a394-372">In this case, click **Expire rule** to expire the rule.</span></span>

| <span data-ttu-id="9a394-373">成本元素维度层次结构节点</span><span class="sxs-lookup"><span data-stu-id="9a394-373">Cost element dimension hierarchy node</span></span> | <span data-ttu-id="9a394-374">成本对象维度层次结构节点</span><span class="sxs-lookup"><span data-stu-id="9a394-374">Cost object dimension hierarchy node</span></span> | <span data-ttu-id="9a394-375">固定百分比</span><span class="sxs-lookup"><span data-stu-id="9a394-375">Fixed percentage</span></span> | <span data-ttu-id="9a394-376">固定金额</span><span class="sxs-lookup"><span data-stu-id="9a394-376">Fixed amount</span></span> | <span data-ttu-id="9a394-377">生效日期</span><span class="sxs-lookup"><span data-stu-id="9a394-377">Valid from</span></span> | <span data-ttu-id="9a394-378">失效日期</span><span class="sxs-lookup"><span data-stu-id="9a394-378">Valid to</span></span>  |
|---------------------------------------|--------------------------------------|------------------|--------------|------------|-----------|
| <span data-ttu-id="9a394-379">固定成本</span><span class="sxs-lookup"><span data-stu-id="9a394-379">Fixed cost</span></span>                            | <span data-ttu-id="9a394-380">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-380">Organization</span></span>                         | <span data-ttu-id="9a394-381">100,00</span><span class="sxs-lookup"><span data-stu-id="9a394-381">100,00</span></span>           | <span data-ttu-id="9a394-382">0.00</span><span class="sxs-lookup"><span data-stu-id="9a394-382">0,00</span></span>         | <span data-ttu-id="9a394-383">1/1/2017</span><span class="sxs-lookup"><span data-stu-id="9a394-383">1/1/2017</span></span>   | <span data-ttu-id="9a394-384">从不</span><span class="sxs-lookup"><span data-stu-id="9a394-384">Never</span></span>     |
| <span data-ttu-id="9a394-385">10001</span><span class="sxs-lookup"><span data-stu-id="9a394-385">10001</span></span>                                 | <span data-ttu-id="9a394-386">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-386">Organization</span></span>                         | <span data-ttu-id="9a394-387">0.00</span><span class="sxs-lookup"><span data-stu-id="9a394-387">0,00</span></span>             | <span data-ttu-id="9a394-388">150,00</span><span class="sxs-lookup"><span data-stu-id="9a394-388">150,00</span></span>       | <span data-ttu-id="9a394-389">1/1/2017</span><span class="sxs-lookup"><span data-stu-id="9a394-389">1/1/2017</span></span>   | <span data-ttu-id="9a394-390">从不</span><span class="sxs-lookup"><span data-stu-id="9a394-390">Never</span></span>     |
| <span data-ttu-id="9a394-391">10001</span><span class="sxs-lookup"><span data-stu-id="9a394-391">10001</span></span>                                 | <span data-ttu-id="9a394-392">财务</span><span class="sxs-lookup"><span data-stu-id="9a394-392">Finance</span></span>                              |                  | <span data-ttu-id="9a394-393">50,00</span><span class="sxs-lookup"><span data-stu-id="9a394-393">50,00</span></span>        | <span data-ttu-id="9a394-394">1/1/2017</span><span class="sxs-lookup"><span data-stu-id="9a394-394">1/1/2017</span></span>   | <span data-ttu-id="9a394-395">20/1/2017</span><span class="sxs-lookup"><span data-stu-id="9a394-395">20/1/2017</span></span> |
| <span data-ttu-id="9a394-396">成本行为或可变成本</span><span class="sxs-lookup"><span data-stu-id="9a394-396">Cost behavior or Variable cost</span></span>        | <span data-ttu-id="9a394-397">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-397">Organization</span></span>                         | <span data-ttu-id="9a394-398">0.00</span><span class="sxs-lookup"><span data-stu-id="9a394-398">0,00</span></span>             | <span data-ttu-id="9a394-399">0.00</span><span class="sxs-lookup"><span data-stu-id="9a394-399">0,00</span></span>         | <span data-ttu-id="9a394-400">1/1/2017</span><span class="sxs-lookup"><span data-stu-id="9a394-400">1/1/2017</span></span>   | <span data-ttu-id="9a394-401">从不</span><span class="sxs-lookup"><span data-stu-id="9a394-401">Never</span></span>     |

<span data-ttu-id="9a394-402">在 2017 年 1 月 20 日之后运行的任何开销计算不再考虑此规则。</span><span class="sxs-lookup"><span data-stu-id="9a394-402">Any overhead calculation that is run after January 20, 2017, no longer considers this rule.</span></span>

> [!NOTE] 
> <span data-ttu-id="9a394-403">**生效日期**和**失效日期**具有日期和时间限制。</span><span class="sxs-lookup"><span data-stu-id="9a394-403">The **Valid from** and **Valid to** fields are date-effective and time-effective.</span></span> <span data-ttu-id="9a394-404">您可以在同一天终止此规则和运行新的开销计算。</span><span class="sxs-lookup"><span data-stu-id="9a394-404">You can expire the rule and run a new overhead calculation on the same day.</span></span>

## <a name="define-dimension-hierarchies-for-security-setup"></a><span data-ttu-id="9a394-405">定义用于安全设置的维度层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-405">Define dimension hierarchies for security setup</span></span>

<span data-ttu-id="9a394-406">成本核算数据应提供给负责报告单位的所有经理。</span><span class="sxs-lookup"><span data-stu-id="9a394-406">Cost accounting data should be made available to all managers who are responsible for a reporting unit.</span></span> <span data-ttu-id="9a394-407">在成本核算术语中，一个报告单位表示为一个成本对象或一组成本对象。</span><span class="sxs-lookup"><span data-stu-id="9a394-407">In Cost accounting terminology, a reporting unit is represented as a cost object or a set of cost objects.</span></span>

<span data-ttu-id="9a394-408">有可能所有经理都将能够访问高度敏感的业务数据，例如收入和毛利。</span><span class="sxs-lookup"><span data-stu-id="9a394-408">Potentially, all managers will be able to access highly sensitive business data, such revenues and margins.</span></span> <span data-ttu-id="9a394-409">因此，设置安全性十分重要，这样经理仅能看到与他们有关的数据。</span><span class="sxs-lookup"><span data-stu-id="9a394-409">Therefore, it's important that you set up security, so that managers see only the data that is relevant to them.</span></span> <span data-ttu-id="9a394-410">为了帮助控制数据安全，您定义维度层次结构。</span><span class="sxs-lookup"><span data-stu-id="9a394-410">To help control data security, you define dimension hierarchies.</span></span>

- <span data-ttu-id="9a394-411">维度层次结构的使用仅适用于在维度层次结构引用中选择的维度值为成本对象维度时。</span><span class="sxs-lookup"><span data-stu-id="9a394-411">The use of dimension hierarchies applies only when the dimension value that is selected in the dimension hierarchy reference is a cost object dimension.</span></span>
- <span data-ttu-id="9a394-412">访问列表层次结构中的每个成本对象维度仅可启用一个维度层次结构。</span><span class="sxs-lookup"><span data-stu-id="9a394-412">Only one dimension hierarchy can be enabled per cost object dimension in the access list hierarchy.</span></span>

<span data-ttu-id="9a394-413">**维度层次结构明细**</span><span class="sxs-lookup"><span data-stu-id="9a394-413">**Dimension hierarchy details**</span></span>

| <span data-ttu-id="9a394-414">维度层次结构名称</span><span class="sxs-lookup"><span data-stu-id="9a394-414">Dimension hierarchy name</span></span> | <span data-ttu-id="9a394-415">维度</span><span class="sxs-lookup"><span data-stu-id="9a394-415">Dimension</span></span>    | <span data-ttu-id="9a394-416">维度层次结构类型名称</span><span class="sxs-lookup"><span data-stu-id="9a394-416">Dimension hierarchy type name</span></span>      | <span data-ttu-id="9a394-417">访问列表层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-417">Access list hierarchy</span></span> |
|--------------------------|--------------|------------------------------------|-----------------------|
| <span data-ttu-id="9a394-418">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-418">Organization</span></span>             | <span data-ttu-id="9a394-419">成本中心</span><span class="sxs-lookup"><span data-stu-id="9a394-419">Cost centers</span></span> | <span data-ttu-id="9a394-420">维度分类层次结构</span><span class="sxs-lookup"><span data-stu-id="9a394-420">Dimension classification hierarchy</span></span> | <span data-ttu-id="9a394-421">**是**</span><span class="sxs-lookup"><span data-stu-id="9a394-421">**Yes**</span></span>               |

<span data-ttu-id="9a394-422">新**用户**快速选项卡在层次结构设计器中可用。</span><span class="sxs-lookup"><span data-stu-id="9a394-422">A new **Users** FastTab is available in the hierarchy designer.</span></span> <span data-ttu-id="9a394-423">在此处，您可以在层次结构的每个节点中插入一个或多个用户 ID。</span><span class="sxs-lookup"><span data-stu-id="9a394-423">Here, you can insert one or more user IDs at each node in the hierarchy.</span></span>

|                 | <span data-ttu-id="9a394-424">用户</span><span class="sxs-lookup"><span data-stu-id="9a394-424">Users</span></span>            | <span data-ttu-id="9a394-425">维度成员范围</span><span class="sxs-lookup"><span data-stu-id="9a394-425">Dimension member ranges</span></span>   |                         |
|-----------------|------------------|---------------------------|-------------------------|
| <span data-ttu-id="9a394-426">**节点**</span><span class="sxs-lookup"><span data-stu-id="9a394-426">**Nodes**</span></span>       | <span data-ttu-id="9a394-427">**用户 ID**</span><span class="sxs-lookup"><span data-stu-id="9a394-427">**User ID**</span></span>      | <span data-ttu-id="9a394-428">**起始维度成员**</span><span class="sxs-lookup"><span data-stu-id="9a394-428">**From dimension member**</span></span> | <span data-ttu-id="9a394-429">**截止维度成员**</span><span class="sxs-lookup"><span data-stu-id="9a394-429">**To dimension member**</span></span> |
| <span data-ttu-id="9a394-430">组织</span><span class="sxs-lookup"><span data-stu-id="9a394-430">Organization</span></span>    | <span data-ttu-id="9a394-431">本杰明，克莱尔</span><span class="sxs-lookup"><span data-stu-id="9a394-431">Benjamin, Claire</span></span> |                           |                         |
| <span data-ttu-id="9a394-432">&nbsp;&nbsp;管理</span><span class="sxs-lookup"><span data-stu-id="9a394-432">&nbsp;&nbsp;Admin</span></span>         | <span data-ttu-id="9a394-433">四月</span><span class="sxs-lookup"><span data-stu-id="9a394-433">April</span></span>            |                           |                         |
| <span data-ttu-id="9a394-434">&nbsp;&nbsp;&nbsp;&nbsp;财务</span><span class="sxs-lookup"><span data-stu-id="9a394-434">&nbsp;&nbsp;&nbsp;&nbsp;Finance</span></span>   | <span data-ttu-id="9a394-435">艾丽西亚</span><span class="sxs-lookup"><span data-stu-id="9a394-435">Alicia</span></span>           | <span data-ttu-id="9a394-436">CC002</span><span class="sxs-lookup"><span data-stu-id="9a394-436">CC002</span></span>                     | <span data-ttu-id="9a394-437">CC003</span><span class="sxs-lookup"><span data-stu-id="9a394-437">CC003</span></span>                   |
|                 |                  | <span data-ttu-id="9a394-438">CC007</span><span class="sxs-lookup"><span data-stu-id="9a394-438">CC007</span></span>                     | <span data-ttu-id="9a394-439">CC007</span><span class="sxs-lookup"><span data-stu-id="9a394-439">CC007</span></span>                   |
| <span data-ttu-id="9a394-440">&nbsp;&nbsp;&nbsp;&nbsp;HR</span><span class="sxs-lookup"><span data-stu-id="9a394-440">&nbsp;&nbsp;&nbsp;&nbsp;HR</span></span>        | <span data-ttu-id="9a394-441">尔尼</span><span class="sxs-lookup"><span data-stu-id="9a394-441">Arnie</span></span>            | <span data-ttu-id="9a394-442">CC001</span><span class="sxs-lookup"><span data-stu-id="9a394-442">CC001</span></span>                     | <span data-ttu-id="9a394-443">CC001</span><span class="sxs-lookup"><span data-stu-id="9a394-443">CC001</span></span>                   |
| <span data-ttu-id="9a394-444">&nbsp;&nbsp;生产</span><span class="sxs-lookup"><span data-stu-id="9a394-444">&nbsp;&nbsp;Production</span></span>    | <span data-ttu-id="9a394-445">大卫</span><span class="sxs-lookup"><span data-stu-id="9a394-445">David</span></span>            |                           |                         |
| <span data-ttu-id="9a394-446">&nbsp;&nbsp;&nbsp;&nbsp;包装</span><span class="sxs-lookup"><span data-stu-id="9a394-446">&nbsp;&nbsp;&nbsp;&nbsp;Packaging</span></span> | <span data-ttu-id="9a394-447">爱伦</span><span class="sxs-lookup"><span data-stu-id="9a394-447">Ellen</span></span>            | <span data-ttu-id="9a394-448">CC005</span><span class="sxs-lookup"><span data-stu-id="9a394-448">CC005</span></span>                     | <span data-ttu-id="9a394-449">CC005</span><span class="sxs-lookup"><span data-stu-id="9a394-449">CC005</span></span>                   |
| <span data-ttu-id="9a394-450">&nbsp;&nbsp;&nbsp;&nbsp;程序集</span><span class="sxs-lookup"><span data-stu-id="9a394-450">&nbsp;&nbsp;&nbsp;&nbsp;Assembly</span></span>  | <span data-ttu-id="9a394-451">克里斯</span><span class="sxs-lookup"><span data-stu-id="9a394-451">Chris</span></span>            | <span data-ttu-id="9a394-452">CC006</span><span class="sxs-lookup"><span data-stu-id="9a394-452">CC006</span></span>                     | <span data-ttu-id="9a394-453">CC006</span><span class="sxs-lookup"><span data-stu-id="9a394-453">CC006</span></span>                   |

> [!NOTE] 
> <span data-ttu-id="9a394-454">成本会计员应分配到该层次结构的顶层，以便他们可以查看成本核算中的所有条目。</span><span class="sxs-lookup"><span data-stu-id="9a394-454">Cost accountants should be assigned to the top level of the hierarchy, so that they can see all entries in Cost accounting.</span></span>

<span data-ttu-id="9a394-455">要启用访问列表层次结构及其安全设置，请转到**成本核算** > **设置** > **参数** > **常规**。</span><span class="sxs-lookup"><span data-stu-id="9a394-455">To enable the access list hierarchy and its security settings, go to **Cost accounting** > **Setup** > **Parameters** > **General**.</span></span> <span data-ttu-id="9a394-456">选择**为成本对象维度成员启用视图访问**参数。</span><span class="sxs-lookup"><span data-stu-id="9a394-456">Select the **Enable view access for cost object dimension members** parameter.</span></span>

<span data-ttu-id="9a394-457">访问列表层次结构的设置用于控制在以下区域显示的数据：</span><span class="sxs-lookup"><span data-stu-id="9a394-457">The settings for the access list hierarchy are used to control the data that is shown in the following areas:</span></span>

- <span data-ttu-id="9a394-458">**成本控制**工作区（客户端）：</span><span class="sxs-lookup"><span data-stu-id="9a394-458">**Cost control** workspace (Client):</span></span>

    - <span data-ttu-id="9a394-459">用于钻取方案的窗体中的数据。</span><span class="sxs-lookup"><span data-stu-id="9a394-459">Data in forms that are used to drill through scenarios</span></span>

- <span data-ttu-id="9a394-460">**成本控制**工作区（移动应用）：</span><span class="sxs-lookup"><span data-stu-id="9a394-460">**Cost control** workspace (Mobile application):</span></span>

    - <span data-ttu-id="9a394-461">卡内余额</span><span class="sxs-lookup"><span data-stu-id="9a394-461">Balances in cards</span></span>

- <span data-ttu-id="9a394-462">Power BI：</span><span class="sxs-lookup"><span data-stu-id="9a394-462">Power BI:</span></span>

    - <span data-ttu-id="9a394-463">Power BI 可视化项中显示的数据</span><span class="sxs-lookup"><span data-stu-id="9a394-463">Data that is shown in Power BI visualizations</span></span>
    - <span data-ttu-id="9a394-464">Microsoft Dynamics 365 for Finance and Operations 客户端中嵌入的数据 Power BI 可视化项</span><span class="sxs-lookup"><span data-stu-id="9a394-464">Data Power BI visualizations that are embedded in the Microsoft Dynamics 365 for Finance and Operations client</span></span>

> [!NOTE] 
> - <span data-ttu-id="9a394-465">在访问列表层次结构可能会影响 Power BI 中的数据前，Power BI 中的访问列表层次结构和行级别安全性必须配对。</span><span class="sxs-lookup"><span data-stu-id="9a394-465">Before the access list hierarchy can affect data in Power BI, access list hierarchy and row-level security in Power BI must be paired.</span></span> <span data-ttu-id="9a394-466">有关详细信息，请参阅 [设置成本核算内容包的安全性](../../dev-itpro/analytics/setup-security-cost-accounting-content-pack.md)。</span><span class="sxs-lookup"><span data-stu-id="9a394-466">For more information, see [Set up security for Cost accounting content pack](../../dev-itpro/analytics/setup-security-cost-accounting-content-pack.md).</span></span>
> - <span data-ttu-id="9a394-467">访问列表层次结构对将数据安全导出到 Excel 没有帮助。</span><span class="sxs-lookup"><span data-stu-id="9a394-467">The access list hierarchy doesn't help secure the export of data to Excel.</span></span> <span data-ttu-id="9a394-468">因此，该报告工具应仅由必须具有查看数据的完全访问权限的成本会计师和经理使用。</span><span class="sxs-lookup"><span data-stu-id="9a394-468">Therefore, that reporting tool should be used only by cost accountants and managers who must have full access to view the data.</span></span>