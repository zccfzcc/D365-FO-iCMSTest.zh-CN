---
title: 成本条目
description: 本文提供有关成本条目及其何时创建的信息。 成本条目是登记指定事件的数量和成本的记录。
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
ms.custom: 19131
ms.assetid: dd2663d8-bcc0-47b1-b36d-57433143487c
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 447b994892e0e71437fbd6c7b8f25bd8fb297728
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56503"
---
# <a name="cost-entries"></a><span data-ttu-id="2a310-104">成本条目</span><span class="sxs-lookup"><span data-stu-id="2a310-104">Cost entries</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="2a310-105">本文提供有关成本条目及其何时创建的信息。</span><span class="sxs-lookup"><span data-stu-id="2a310-105">This article provides information about cost entries and when they are created.</span></span> <span data-ttu-id="2a310-106">成本条目是登记指定事件的数量和成本的记录。</span><span class="sxs-lookup"><span data-stu-id="2a310-106">A cost entry is a record that registers the quantity and cost of a given event.</span></span>

<span data-ttu-id="2a310-107">成本条目是在活动财务库存维度上记录的库存交易记录的合并。</span><span class="sxs-lookup"><span data-stu-id="2a310-107">Cost entries are aggregations of inventory transactions that are recorded on active financial inventory dimensions.</span></span>

## <a name="examples"></a><span data-ttu-id="2a310-108">示例</span><span class="sxs-lookup"><span data-stu-id="2a310-108">Examples</span></span>
### <a name="example-1-no-cost-entries-are-created"></a><span data-ttu-id="2a310-109">示例 1：未创建任何成本条目</span><span class="sxs-lookup"><span data-stu-id="2a310-109">Example 1: No cost entries are created</span></span>

<span data-ttu-id="2a310-110">登记转移日记帐事件。</span><span class="sxs-lookup"><span data-stu-id="2a310-110">A transfer journal event is registered.</span></span> <span data-ttu-id="2a310-111">该事件将一件物料 A 从库位 A 转移到库位 B。Location 库存维度不被视为成本对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="2a310-111">The event transfers one piece of item A from location A to location B. The Location inventory dimension isn't considered part of the cost object.</span></span> <span data-ttu-id="2a310-112">因此，该事件将创建两个库存交易记录，但不创建成本条目。</span><span class="sxs-lookup"><span data-stu-id="2a310-112">Therefore, the event creates two inventory transactions and no cost entries.</span></span>

### <a name="example-2-cost-entries-are-created"></a><span data-ttu-id="2a310-113">示例 2：创建成本条目</span><span class="sxs-lookup"><span data-stu-id="2a310-113">Example 2: Cost entries are created</span></span>

<span data-ttu-id="2a310-114">登记转移日记帐事件。</span><span class="sxs-lookup"><span data-stu-id="2a310-114">A transfer journal event is registered.</span></span> <span data-ttu-id="2a310-115">该事件将一件物料 A 从站点 1 转移到站点 2。</span><span class="sxs-lookup"><span data-stu-id="2a310-115">The event transfers one piece of item A from site 1 to site 2.</span></span> <span data-ttu-id="2a310-116">Site 库存维度被视为成本对象的一部分。</span><span class="sxs-lookup"><span data-stu-id="2a310-116">The Site inventory dimension is considered part of the cost object.</span></span> <span data-ttu-id="2a310-117">因此，该事件将创建两个库存交易记录和两个成本条目。</span><span class="sxs-lookup"><span data-stu-id="2a310-117">Therefore, the event creates two inventory transactions and two cost entries.</span></span>

### <a name="example-3-one-cost-entry-is-created"></a><span data-ttu-id="2a310-118">示例 3：创建一个成本条目</span><span class="sxs-lookup"><span data-stu-id="2a310-118">Example 3: One cost entry is created</span></span>

<span data-ttu-id="2a310-119">登记采购订单的产品收据事件。</span><span class="sxs-lookup"><span data-stu-id="2a310-119">A product receipt event is registered for a purchase order.</span></span> <span data-ttu-id="2a310-120">该事件登记 100 件物料 A（单位成本为 10.00 美元 (USD)）。</span><span class="sxs-lookup"><span data-stu-id="2a310-120">The event registers 100 pieces of item A at a unit cost of 10.00 U.S. dollars (USD).</span></span> <span data-ttu-id="2a310-121">由于物料 A 使用序列号跟踪库存管理的目的，因此将为接收的每个物料创建一个唯一的序列号。</span><span class="sxs-lookup"><span data-stu-id="2a310-121">Because item A uses a serial number to track the purpose of inventory management, a unique serial number is created for each item that is received.</span></span> <span data-ttu-id="2a310-122">因此，该事件将创建 100 个库存交易记录和一个成本条目。</span><span class="sxs-lookup"><span data-stu-id="2a310-122">Therefore, the event creates 100 inventory transactions and one cost entry.</span></span>

## <a name="cost-entries-page"></a><span data-ttu-id="2a310-123">成本条目页面</span><span class="sxs-lookup"><span data-stu-id="2a310-123">Cost entries page</span></span>
<span data-ttu-id="2a310-124">利用新的**成本条目**页面，可以查看和控制数量和成本的登记。</span><span class="sxs-lookup"><span data-stu-id="2a310-124">The new **Cost entries** page lets you view and control registrations of quantities and costs.</span></span> <span data-ttu-id="2a310-125">此页面对**库存交易记录**和**库存结算**页面进行了补充。</span><span class="sxs-lookup"><span data-stu-id="2a310-125">This page complements the **Inventory transaction** and **Inventory settlement** pages.</span></span> <span data-ttu-id="2a310-126">按时间顺序登记事件的记录。</span><span class="sxs-lookup"><span data-stu-id="2a310-126">Records are registered in chronological order for an event.</span></span> <span data-ttu-id="2a310-127">因此，您可以快速查找和控制与文档相关的一个特定事件或所有事件的累计成本。</span><span class="sxs-lookup"><span data-stu-id="2a310-127">Therefore, you can quickly find and control the accumulated costs of a specific event or all events that are related to a document.</span></span> <span data-ttu-id="2a310-128">以下是一个示例：</span><span class="sxs-lookup"><span data-stu-id="2a310-128">Here is an example:</span></span>

-   <span data-ttu-id="2a310-129">为物料 A 登记产品收据事件。以单位成本 10.00 美元接收 100 件物料。</span><span class="sxs-lookup"><span data-stu-id="2a310-129">A product receipt event is registered for item A. One hundred pieces are received at a unit cost of 10.00 USD.</span></span>
-   <span data-ttu-id="2a310-130">在登记发票事件几天后，单位成本增加到 11.00 美元。</span><span class="sxs-lookup"><span data-stu-id="2a310-130">A few days after the invoice event is registered, the cost increases to 11.00 USD.</span></span> <span data-ttu-id="2a310-131">因此，总金额为 1,100 美元。</span><span class="sxs-lookup"><span data-stu-id="2a310-131">Therefore, the total amount is 1,100 USD.</span></span> <span data-ttu-id="2a310-132">创建另一个凭证来说明 100 美元的差额。</span><span class="sxs-lookup"><span data-stu-id="2a310-132">A second voucher is created to account for the difference of 100 USD.</span></span>
-   <span data-ttu-id="2a310-133">几天后，将在采购订单上登记 15.00 美元的杂费（含运输成本）。</span><span class="sxs-lookup"><span data-stu-id="2a310-133">A few days later, a miscellaneous charge of 15.00 USD to cover the transportation cost is registered on the purchase order.</span></span>

| <span data-ttu-id="2a310-134">凭证</span><span class="sxs-lookup"><span data-stu-id="2a310-134">Voucher</span></span> | <span data-ttu-id="2a310-135">日期</span><span class="sxs-lookup"><span data-stu-id="2a310-135">Date</span></span>       | <span data-ttu-id="2a310-136">参考</span><span class="sxs-lookup"><span data-stu-id="2a310-136">Reference</span></span>      | <span data-ttu-id="2a310-137">数字</span><span class="sxs-lookup"><span data-stu-id="2a310-137">Number</span></span> | <span data-ttu-id="2a310-138">批次 ID</span><span class="sxs-lookup"><span data-stu-id="2a310-138">Lot ID</span></span>  | <span data-ttu-id="2a310-139">数量</span><span class="sxs-lookup"><span data-stu-id="2a310-139">Quantity</span></span> | <span data-ttu-id="2a310-140">本币金额</span><span class="sxs-lookup"><span data-stu-id="2a310-140">Amount</span></span>  |
|---------|------------|----------------|--------|---------|---------------|----|
| <span data-ttu-id="2a310-141">00001</span><span class="sxs-lookup"><span data-stu-id="2a310-141">00001</span></span>   | <span data-ttu-id="2a310-142">01-01-2015</span><span class="sxs-lookup"><span data-stu-id="2a310-142">01-01-2015</span></span> | <span data-ttu-id="2a310-143">采购订单</span><span class="sxs-lookup"><span data-stu-id="2a310-143">Purchase order</span></span> | <span data-ttu-id="2a310-144">100001</span><span class="sxs-lookup"><span data-stu-id="2a310-144">100001</span></span> | <span data-ttu-id="2a310-145">0000101</span><span class="sxs-lookup"><span data-stu-id="2a310-145">0000101</span></span> | <span data-ttu-id="2a310-146">100.00</span><span class="sxs-lookup"><span data-stu-id="2a310-146">100.00</span></span>   | <span data-ttu-id="2a310-147">1000.00</span><span class="sxs-lookup"><span data-stu-id="2a310-147">1000.00</span></span> |
| <span data-ttu-id="2a310-148">00002</span><span class="sxs-lookup"><span data-stu-id="2a310-148">00002</span></span>   | <span data-ttu-id="2a310-149">20-01-2015</span><span class="sxs-lookup"><span data-stu-id="2a310-149">20-01-2015</span></span> | <span data-ttu-id="2a310-150">采购订单</span><span class="sxs-lookup"><span data-stu-id="2a310-150">Purchase order</span></span> | <span data-ttu-id="2a310-151">100001</span><span class="sxs-lookup"><span data-stu-id="2a310-151">100001</span></span> | <span data-ttu-id="2a310-152">0000101</span><span class="sxs-lookup"><span data-stu-id="2a310-152">0000101</span></span> |          | <span data-ttu-id="2a310-153">100.00</span><span class="sxs-lookup"><span data-stu-id="2a310-153">100.00</span></span>  |
| <span data-ttu-id="2a310-154">00003</span><span class="sxs-lookup"><span data-stu-id="2a310-154">00003</span></span>   | <span data-ttu-id="2a310-155">31-01-2015</span><span class="sxs-lookup"><span data-stu-id="2a310-155">31-01-2015</span></span> | <span data-ttu-id="2a310-156">调整</span><span class="sxs-lookup"><span data-stu-id="2a310-156">Adjustment</span></span>     | <span data-ttu-id="2a310-157">100001</span><span class="sxs-lookup"><span data-stu-id="2a310-157">100001</span></span> | <span data-ttu-id="2a310-158">0000101</span><span class="sxs-lookup"><span data-stu-id="2a310-158">0000101</span></span> |          | <span data-ttu-id="2a310-159">15.00</span><span class="sxs-lookup"><span data-stu-id="2a310-159">15.00</span></span>   |

<span data-ttu-id="2a310-160">**成本条目**页面支持按文档 ID 和文档日期进行筛选。</span><span class="sxs-lookup"><span data-stu-id="2a310-160">The **Cost entries** page enables filtering by document ID and document date.</span></span> 

> [!NOTE]
> <span data-ttu-id="2a310-161">成本条目仅适用于[成本对象](cost-object.md)或已发布的产品。</span><span class="sxs-lookup"><span data-stu-id="2a310-161">Cost entries are available only for [cost objects](cost-object.md) or released products.</span></span>

<a name="additional-resources"></a><span data-ttu-id="2a310-162">其他资源</span><span class="sxs-lookup"><span data-stu-id="2a310-162">Additional resources</span></span>
--------

[<span data-ttu-id="2a310-163">成本对象</span><span class="sxs-lookup"><span data-stu-id="2a310-163">Cost objects</span></span>](cost-object.md)


