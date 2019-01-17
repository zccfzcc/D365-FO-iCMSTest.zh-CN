---
title: 成本对象
description: 本文提供有关成本对象的信息，并说明如何累计成本和数量。 成本对象是为其累计成本和数量的实体。 成本对象实体可以是产品或产品变型，例如样式和颜色的变型。
author: AndersGirke
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: InventCostOnhandItem
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 19451
ms.assetid: ec776b98-813a-490d-848f-468452d98fac
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 79aeda518b900629761825476954130fb3fa0838
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "53795"
---
# <a name="cost-objects"></a><span data-ttu-id="c7e3b-105">成本对象</span><span class="sxs-lookup"><span data-stu-id="c7e3b-105">Cost objects</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="c7e3b-106">本文提供有关成本对象的信息，并说明如何累计成本和数量。</span><span class="sxs-lookup"><span data-stu-id="c7e3b-106">This article provides information about costs objects, and explains how costs and quantities are accumulated.</span></span> <span data-ttu-id="c7e3b-107">成本对象是为其累计成本和数量的实体。</span><span class="sxs-lookup"><span data-stu-id="c7e3b-107">A cost object is an entity that costs and quantities are accumulated for.</span></span> <span data-ttu-id="c7e3b-108">成本对象实体可以是产品或产品变型，例如样式和颜色的变型。</span><span class="sxs-lookup"><span data-stu-id="c7e3b-108">A cost object entity can be either a product or product variants, such as variants for style and color.</span></span>  

## <a name="cost-objects"></a><span data-ttu-id="c7e3b-109">成本对象</span><span class="sxs-lookup"><span data-stu-id="c7e3b-109">Cost objects</span></span>

<span data-ttu-id="c7e3b-110">**成本对象**页面列出在某个产品上登记的所有成本对象。</span><span class="sxs-lookup"><span data-stu-id="c7e3b-110">The **Cost objects** page lists all cost objects that are registered on a product.</span></span> <span data-ttu-id="c7e3b-111">成本对象由来自以下源的数据定义：</span><span class="sxs-lookup"><span data-stu-id="c7e3b-111">The cost objects are defined by data from the following sources:</span></span>

-   <span data-ttu-id="c7e3b-112">产品</span><span class="sxs-lookup"><span data-stu-id="c7e3b-112">Product</span></span>
-   <span data-ttu-id="c7e3b-113">产品维度组</span><span class="sxs-lookup"><span data-stu-id="c7e3b-113">Product dimension group</span></span>
-   <span data-ttu-id="c7e3b-114">存储维度组</span><span class="sxs-lookup"><span data-stu-id="c7e3b-114">Storage dimension group</span></span>
-   <span data-ttu-id="c7e3b-115">跟踪维度组</span><span class="sxs-lookup"><span data-stu-id="c7e3b-115">Tracking dimension group</span></span>

<span data-ttu-id="c7e3b-116">**注意：** 成本对象仅表示**直接材料**类型的成本元素。</span><span class="sxs-lookup"><span data-stu-id="c7e3b-116">**Note:** A cost object represents a cost element of the **Direct material** type only.</span></span> <span data-ttu-id="c7e3b-117">成本对象和库存对象在为财务库存所选的库存维度定义成本对象的方式上存在差异。</span><span class="sxs-lookup"><span data-stu-id="c7e3b-117">A cost object and an inventory object differ in the way that a cost object is defined by the inventory dimensions that are selected for financial inventory.</span></span> <span data-ttu-id="c7e3b-118">例如，某个物料具有以下配置：</span><span class="sxs-lookup"><span data-stu-id="c7e3b-118">For example, an item has the following configuration:</span></span>

-   <span data-ttu-id="c7e3b-119">**站点：** Physical inventory = Yes, Financial inventory = Yes</span><span class="sxs-lookup"><span data-stu-id="c7e3b-119">**Site:** Physical inventory = Yes, Financial inventory = Yes</span></span>
-   <span data-ttu-id="c7e3b-120">**仓库：** Physical inventory = Yes, Financial inventory = No</span><span class="sxs-lookup"><span data-stu-id="c7e3b-120">**Warehouse:** Physical inventory = Yes, Financial inventory = No</span></span>
-   <span data-ttu-id="c7e3b-121">**批号：** Physical inventory = Yes, Financial inventory = No</span><span class="sxs-lookup"><span data-stu-id="c7e3b-121">**Batch No.:** Physical inventory = Yes, Financial inventory = No</span></span>

<span data-ttu-id="c7e3b-122">下表显示了成本对象和库存对象的定义。</span><span class="sxs-lookup"><span data-stu-id="c7e3b-122">The following table shows what is a cost object and what is an inventory object.</span></span>

| <span data-ttu-id="c7e3b-123">对象类型</span><span class="sxs-lookup"><span data-stu-id="c7e3b-123">Object type</span></span>      | <span data-ttu-id="c7e3b-124">物料编号</span><span class="sxs-lookup"><span data-stu-id="c7e3b-124">Item number</span></span> | <span data-ttu-id="c7e3b-125">站点</span><span class="sxs-lookup"><span data-stu-id="c7e3b-125">Site</span></span> | <span data-ttu-id="c7e3b-126">仓库</span><span class="sxs-lookup"><span data-stu-id="c7e3b-126">Warehouse</span></span> | <span data-ttu-id="c7e3b-127">批号</span><span class="sxs-lookup"><span data-stu-id="c7e3b-127">Batch No.</span></span> |
|------------------|-------------|------|-----------|-----------|
| <span data-ttu-id="c7e3b-128">成本对象</span><span class="sxs-lookup"><span data-stu-id="c7e3b-128">Cost object</span></span>      | <span data-ttu-id="c7e3b-129"> x</span><span class="sxs-lookup"><span data-stu-id="c7e3b-129">x</span></span>           | <span data-ttu-id="c7e3b-130"> x</span><span class="sxs-lookup"><span data-stu-id="c7e3b-130">x</span></span>    |           |           |
| <span data-ttu-id="c7e3b-131">库存对象</span><span class="sxs-lookup"><span data-stu-id="c7e3b-131">Inventory object</span></span> | <span data-ttu-id="c7e3b-132"> x</span><span class="sxs-lookup"><span data-stu-id="c7e3b-132">x</span></span>           | <span data-ttu-id="c7e3b-133"> x</span><span class="sxs-lookup"><span data-stu-id="c7e3b-133">x</span></span>    |  <span data-ttu-id="c7e3b-134"> x</span><span class="sxs-lookup"><span data-stu-id="c7e3b-134">x</span></span>        | <span data-ttu-id="c7e3b-135"> x</span><span class="sxs-lookup"><span data-stu-id="c7e3b-135">x</span></span>         |

## <a name="accumulation-of-costs-and-quantities"></a><span data-ttu-id="c7e3b-136">成本和数量的累计</span><span class="sxs-lookup"><span data-stu-id="c7e3b-136">Accumulation of costs and quantities</span></span>
-   <span data-ttu-id="c7e3b-137">**值**字段中的值为以下值的和：</span><span class="sxs-lookup"><span data-stu-id="c7e3b-137">The value in the **Value** fieldis a sum of the following values:</span></span>
    -   <span data-ttu-id="c7e3b-138">实际成本额</span><span class="sxs-lookup"><span data-stu-id="c7e3b-138">Physical cost amount</span></span>
    -   <span data-ttu-id="c7e3b-139">财务成本额</span><span class="sxs-lookup"><span data-stu-id="c7e3b-139">Financial cost amount</span></span>
    -   <span data-ttu-id="c7e3b-140">调整</span><span class="sxs-lookup"><span data-stu-id="c7e3b-140">Adjustments</span></span>
-   <span data-ttu-id="c7e3b-141">**数量**字段中的值为以下值的和：</span><span class="sxs-lookup"><span data-stu-id="c7e3b-141">The value in the **Quantity** field is a sum of the following values:</span></span>
    -   <span data-ttu-id="c7e3b-142">已接收</span><span class="sxs-lookup"><span data-stu-id="c7e3b-142">Received</span></span>
    -   <span data-ttu-id="c7e3b-143">已扣除</span><span class="sxs-lookup"><span data-stu-id="c7e3b-143">Deducted</span></span>
    -   <span data-ttu-id="c7e3b-144">已过帐的数量</span><span class="sxs-lookup"><span data-stu-id="c7e3b-144">Posted quantity</span></span>
-   <span data-ttu-id="c7e3b-145">**平均单位成本**字段为计算字段。</span><span class="sxs-lookup"><span data-stu-id="c7e3b-145">The **Average unit cost** field is a calculated field.</span></span> <span data-ttu-id="c7e3b-146">该值通过用**值**值除以**数量**值得出。</span><span class="sxs-lookup"><span data-stu-id="c7e3b-146">The value is calculated by dividing the **Value** value by the **Quantity** value.</span></span>

<span data-ttu-id="c7e3b-147">**注意：** **包括实际成本** 参数不影响之前的计算。</span><span class="sxs-lookup"><span data-stu-id="c7e3b-147">**Note:** The \*\*Include physical value \*\*parameter has no effect on the preceding calculations.</span></span>

<a name="additional-resources"></a><span data-ttu-id="c7e3b-148">其他资源</span><span class="sxs-lookup"><span data-stu-id="c7e3b-148">Additional resources</span></span>
--------

[<span data-ttu-id="c7e3b-149">产品维度组</span><span class="sxs-lookup"><span data-stu-id="c7e3b-149">Product dimension group</span></span>](https://technet.microsoft.com/en-us/library/aa499382.aspx)

[<span data-ttu-id="c7e3b-150">存储维度组</span><span class="sxs-lookup"><span data-stu-id="c7e3b-150">Storage dimension group</span></span>](https://technet.microsoft.com/en-us/library/hh209317.aspx)

[<span data-ttu-id="c7e3b-151">跟踪维度组</span><span class="sxs-lookup"><span data-stu-id="c7e3b-151">Tracking dimension group</span></span>](https://technet.microsoft.com/en-us/library/hh209465.aspx)

[<span data-ttu-id="c7e3b-152">新增功能或更改的功能</span><span class="sxs-lookup"><span data-stu-id="c7e3b-152">What's new or changed</span></span>](../../fin-and-ops/get-started/whats-new-changed.md)

[<span data-ttu-id="c7e3b-153">成本条目</span><span class="sxs-lookup"><span data-stu-id="c7e3b-153">Cost entries</span></span>](cost-entries.md)



