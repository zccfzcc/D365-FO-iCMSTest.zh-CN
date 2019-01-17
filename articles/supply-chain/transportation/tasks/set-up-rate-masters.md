---
title: 设置费率主数据
description: 此过程显示如何设置费率主数据。
author: ShylaThompson
manager: AnnBe
ms.date: 11/11/2016
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Operations
ms.search.region: Global
ms.search.industry: Distribution
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: e059cd8e1228748ac247931b6af5b87368a20fc1
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55989"
---
# <a name="set-up-rate-masters"></a><span data-ttu-id="c2bf0-103">设置费率主数据</span><span class="sxs-lookup"><span data-stu-id="c2bf0-103">Set up rate masters</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="c2bf0-104">此过程显示如何设置费率主数据。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-104">This procedure shows you how to set up a rate master.</span></span> <span data-ttu-id="c2bf0-105">物流经理通常根据与承运人签订的合同设置费率主数据。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-105">The logistic manager usually sets up rate masters, depending on the contracts signed with the carriers.</span></span> <span data-ttu-id="c2bf0-106">在此场景中，您将设置航空承运人的费率主数据。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-106">In this scenario you will set up a rate master for an air carrier.</span></span> <span data-ttu-id="c2bf0-107">创建此程序的演示数据公司是 USMF。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-107">The demo data company used to create this procedure is USMF.</span></span>


## <a name="set-up-rate-master"></a><span data-ttu-id="c2bf0-108">设置费率主数据</span><span class="sxs-lookup"><span data-stu-id="c2bf0-108">Set up rate master</span></span>
1. <span data-ttu-id="c2bf0-109">转到“运输管理”>“设置”>“评级”>“费率主数据”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-109">Go to Transportation management > Setup > Rating > Rate master.</span></span>
2. <span data-ttu-id="c2bf0-110">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-110">Click New.</span></span>
3. <span data-ttu-id="c2bf0-111">在“费率主数据”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-111">In the Rate master field, type a value.</span></span>
4. <span data-ttu-id="c2bf0-112">在“名称”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-112">In the Name field, type a value.</span></span>
5. <span data-ttu-id="c2bf0-113">在“评级元数据 ID”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-113">In the Rating metadata ID field, click the drop-down button to open the lookup.</span></span>
    * <span data-ttu-id="c2bf0-114">评级元数据 ID 将确定费率主数据所需的数据，因为其定义使用此费率主数据的 TMS 引擎预期的主数据。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-114">The rating metadata ID will determine the data needed for the rate master, as it defines the metadata expected by the TMS engine using this rate master.</span></span>  
6. <span data-ttu-id="c2bf0-115">在本示例中，选择 P2P 选项</span><span class="sxs-lookup"><span data-stu-id="c2bf0-115">For this example, select the P2P option</span></span>
7. <span data-ttu-id="c2bf0-116">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-116">In the list, click the link in the selected row.</span></span>
8. <span data-ttu-id="c2bf0-117">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-117">Click Save.</span></span>

## <a name="set-up-rate-base"></a><span data-ttu-id="c2bf0-118">设置基本费率</span><span class="sxs-lookup"><span data-stu-id="c2bf0-118">Set up rate base</span></span>
1. <span data-ttu-id="c2bf0-119">单击“基本费率”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-119">Click Rate base.</span></span>
    * <span data-ttu-id="c2bf0-120">基本费率确定承运人的费率，并且可用于设置关税结构，因为其构成分解主数据中定义的中断点的费率。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-120">The rate base determines the rate of the carrier, and can be used to set up a tariff structure as it structures the rates in the breakpoints defined in the break master.</span></span>  
2. <span data-ttu-id="c2bf0-121">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-121">Click New.</span></span>
3. <span data-ttu-id="c2bf0-122">在“基本费率”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-122">In the Rate base field, type a value.</span></span>
4. <span data-ttu-id="c2bf0-123">在“名称”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-123">In the Name field, type a value.</span></span>
5. <span data-ttu-id="c2bf0-124">在“分解主数据”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-124">In the Break master field, click the drop-down button to open the lookup.</span></span>
    * <span data-ttu-id="c2bf0-125">分解主数据用于定义价格结构及其中断点。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-125">Break masters are used to define the pricing structure and its breakpoints.</span></span> <span data-ttu-id="c2bf0-126">价格结构使用基于物理维度的分层定价方式。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-126">The pricing structure uses tiered pricing that is based on physical dimensions.</span></span>  
6. <span data-ttu-id="c2bf0-127">在本示例中，使用重量</span><span class="sxs-lookup"><span data-stu-id="c2bf0-127">For this example, use weight</span></span>
7. <span data-ttu-id="c2bf0-128">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-128">In the list, click the link in the selected row.</span></span>
8. <span data-ttu-id="c2bf0-129">切换“详细信息”部分的展开项。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-129">Toggle the expansion of the Details section.</span></span>
9. <span data-ttu-id="c2bf0-130">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-130">Click New.</span></span>
10. <span data-ttu-id="c2bf0-131">在“卸货地邮政编码起始编号”字段中，键入“30301”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-131">In the Drop-off Postal Code From field, type '30301'.</span></span>
11. <span data-ttu-id="c2bf0-132">在“卸货地邮政编码结束编号”字段中，键入“30318”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-132">In the Drop-off Postal Code To field, type '30318'.</span></span>
12. <span data-ttu-id="c2bf0-133">在“卸货国家/地区”字段中，键入“美国”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-133">In the Drop-off Country Region field, type 'USA'.</span></span>
13. <span data-ttu-id="c2bf0-134">在“<1.00 磅”字段中，键入 '100'。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-134">In the <1.00 Lbs field, type '100'.</span></span>
    * <span data-ttu-id="c2bf0-135">如果负荷的总重量少于 1 磅，插入每磅费率。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-135">Insert the rate per lbs if the total weight of the load is less than 1 pound.</span></span>  
14. <span data-ttu-id="c2bf0-136">在“< 5.00 磅”字段中，键入“300”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-136">In the <5.00 Lbs field, type '300'.</span></span>
    * <span data-ttu-id="c2bf0-137">如果负荷的总重量少于 5 磅，插入每磅费率。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-137">Insert the rate per lbs if the total weight of the load is less than 5 pounds.</span></span>  
15. <span data-ttu-id="c2bf0-138">在“< 20.00 磅”字段中，键入“500”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-138">In the <20.00 Lbs field, type '500'.</span></span>
    * <span data-ttu-id="c2bf0-139">如果负荷的总重量少于 20 磅，插入每磅费率。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-139">Insert the rate per lbs if the total weight of the load is less than 20 pounds.</span></span>  
16. <span data-ttu-id="c2bf0-140">在“< 100.00 磅”字段中，键入“1000”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-140">In the <100.00 Lbs field, type '1000'.</span></span>
    * <span data-ttu-id="c2bf0-141">如果负荷的总重量少于 100 磅，插入每磅费率。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-141">Insert the rate per lbs if the total weight of the load is less than 100 pounds.</span></span>  
17. <span data-ttu-id="c2bf0-142">在“< 1,000.00 磅”字段中，键入“3000”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-142">In the <1,000.00 Lbs field, type '3000'.</span></span>
    * <span data-ttu-id="c2bf0-143">如果负荷的总重量少于 1000 磅，插入每磅费率。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-143">Insert the rate per lbs if the total weight of the load is less than 1000 pounds.</span></span>  
18. <span data-ttu-id="c2bf0-144">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-144">Click Save.</span></span>
19. <span data-ttu-id="c2bf0-145">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-145">Close the page.</span></span>

## <a name="assign-rate-base"></a><span data-ttu-id="c2bf0-146">分配基本费率</span><span class="sxs-lookup"><span data-stu-id="c2bf0-146">Assign rate base</span></span>
1. <span data-ttu-id="c2bf0-147">切换“基本费率分配”部分的展开项。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-147">Toggle the expansion of the Rate base assignments section.</span></span>
2. <span data-ttu-id="c2bf0-148">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-148">Click New.</span></span>
    * <span data-ttu-id="c2bf0-149">对于每个费率主数据，您可以有几个基本费率分配。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-149">You can have several rate base assignments for each rate master.</span></span> <span data-ttu-id="c2bf0-150">这使得可能根据目的地、服务或不同的基本费率，为每个承运人创建多个不同的价格点。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-150">This makes it possible to create several different price points for each carrier depending on destinations, services, or different rate bases.</span></span> <span data-ttu-id="c2bf0-151">在此过程将只创建基本费率分配。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-151">In this procedure you will only create one rate base assignment.</span></span>  
3. <span data-ttu-id="c2bf0-152">在“名称”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-152">In the Name field, type a value.</span></span>
4. <span data-ttu-id="c2bf0-153">在“基本费率”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-153">In the Rate base field, click the drop-down button to open the lookup.</span></span>
5. <span data-ttu-id="c2bf0-154">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-154">In the list, click the link in the selected row.</span></span>
6. <span data-ttu-id="c2bf0-155">在“服务”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-155">In the Service field, click the drop-down button to open the lookup.</span></span>
7. <span data-ttu-id="c2bf0-156">在列表中，找到并选择所需记录。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-156">In the list, find and select the desired record.</span></span>
8. <span data-ttu-id="c2bf0-157">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-157">In the list, click the link in the selected row.</span></span>
9. <span data-ttu-id="c2bf0-158">在“提货邮政编码”字段中，键入“98052”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-158">In the Pick-up Postal Code field, type '98052'.</span></span>
    * <span data-ttu-id="c2bf0-159">指定哪些邮政编码对于此基本费率分配是有效的。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-159">Specify which postal code this rate base assignment should be valid from.</span></span>    
10. <span data-ttu-id="c2bf0-160">在“提货国家/地区”字段中，键入“美国”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-160">In the Pick-up Country Region field, type 'USA'.</span></span>
11. <span data-ttu-id="c2bf0-161">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="c2bf0-161">Click Save.</span></span>
