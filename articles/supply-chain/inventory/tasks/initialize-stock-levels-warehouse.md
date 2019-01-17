---
title: 初始化仓库中的库存级别
description: 该过程说明如何利用“库存移动日记帐”手动更新现有库存。
author: perlynne
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: InventJournalMovement, InventJournalCreate, InventItemIdLookupSimple, InventLocationIdLookup, WMSLocationIdLookup
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Distribution
ms.author: perlynne
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: e36709a049084588e2e851ed2895529a676d55d9
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55966"
---
# <a name="initialize-stock-levels-in-the-warehouse"></a><span data-ttu-id="088f5-103">初始化仓库中的库存级别</span><span class="sxs-lookup"><span data-stu-id="088f5-103">Initialize stock levels in the warehouse</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="088f5-104">该过程说明如何利用“库存移动日记帐”手动更新现有库存。</span><span class="sxs-lookup"><span data-stu-id="088f5-104">This procedure shows you how to get the on-hand inventory updated manually using an Inventory movement journal.</span></span> <span data-ttu-id="088f5-105">（也可根据导入交易的数据实体更新现有库存。）您可以通过演示数据公司 USMF 运行此指南，通过它可以获得所有的必要条件，如日记帐名称、项目设置、过帐文件以及帐号。</span><span class="sxs-lookup"><span data-stu-id="088f5-105">(It’s also possible to update on-hand inventory by importing transactions in data entities.) You can run this guide in demo data company USMF where all the prerequisites like journal name, item setup, posting profiles, and accounts are available.</span></span> <span data-ttu-id="088f5-106">该指南显示了所使用的物料和维度的特定值。</span><span class="sxs-lookup"><span data-stu-id="088f5-106">The guide suggests specific values for the item and dimensions that are used.</span></span> <span data-ttu-id="088f5-107">如果选择不同的项目，则需要输入不同的维度值。</span><span class="sxs-lookup"><span data-stu-id="088f5-107">If you choose a different item, you may need to enter values for different dimensions.</span></span>

1. <span data-ttu-id="088f5-108">转到“库存管理”>“日记帐条目”>“物料”>“移动”。</span><span class="sxs-lookup"><span data-stu-id="088f5-108">Go to Inventory management > Journal entries > Items > Movement.</span></span>
2. <span data-ttu-id="088f5-109">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="088f5-109">Click New.</span></span>
3. <span data-ttu-id="088f5-110">在“名称”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="088f5-110">In the Name field, click the drop-down button to open the lookup.</span></span>
4. <span data-ttu-id="088f5-111">选择“IMov”。</span><span class="sxs-lookup"><span data-stu-id="088f5-111">Select IMov.</span></span>
    * <span data-ttu-id="088f5-112">根据不同的业务用途使用不同的日记帐名称模板是一个很好的实践。</span><span class="sxs-lookup"><span data-stu-id="088f5-112">It’s a good practise to use different journal name templates for the different business purposes.</span></span>  
5. <span data-ttu-id="088f5-113">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="088f5-113">In the list, click the link in the selected row.</span></span>
6. <span data-ttu-id="088f5-114">在“抵消帐户”字段中，设定值“140200”。</span><span class="sxs-lookup"><span data-stu-id="088f5-114">In the Offset account field, specify the values '140200'.</span></span>
    * <span data-ttu-id="088f5-115">该抵消帐户将默认为日记帐行的帐户。</span><span class="sxs-lookup"><span data-stu-id="088f5-115">This is the offset account that will be the default account on the journal lines.</span></span> <span data-ttu-id="088f5-116">给抵消帐户每一行分配不同的名称可以覆盖默认帐户名称。</span><span class="sxs-lookup"><span data-stu-id="088f5-116">It’s possible to override the default to assign different offset accounts per line.</span></span>  
7. <span data-ttu-id="088f5-117">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="088f5-117">Click OK.</span></span>
8. <span data-ttu-id="088f5-118">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="088f5-118">Click New.</span></span>
9. <span data-ttu-id="088f5-119">在“物料编号”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="088f5-119">In the Item number field, click the drop-down button to open the lookup.</span></span>
10. <span data-ttu-id="088f5-120">选择物料 A0001。</span><span class="sxs-lookup"><span data-stu-id="088f5-120">Select item A0001.</span></span>
11. <span data-ttu-id="088f5-121">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="088f5-121">In the list, click the link in the selected row.</span></span>
12. <span data-ttu-id="088f5-122">单击“库存维度”选项卡。</span><span class="sxs-lookup"><span data-stu-id="088f5-122">Click the Inventory dimensions tab.</span></span>
13. <span data-ttu-id="088f5-123">在“位置”字段中，单击下拉按钮打开查询。</span><span class="sxs-lookup"><span data-stu-id="088f5-123">In the Site field, click the drop-down button to open the lookup.</span></span>
14. <span data-ttu-id="088f5-124">选择“站点 1”。</span><span class="sxs-lookup"><span data-stu-id="088f5-124">Select site 1.</span></span>
15. <span data-ttu-id="088f5-125">在“仓库”字段，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="088f5-125">In the Warehouse field, click the drop-down button to open the lookup.</span></span>
16. <span data-ttu-id="088f5-126">选择“仓库 13”。</span><span class="sxs-lookup"><span data-stu-id="088f5-126">Select warehouse 13.</span></span>
17. <span data-ttu-id="088f5-127">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="088f5-127">In the list, click the link in the selected row.</span></span>
18. <span data-ttu-id="088f5-128">在“地点”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="088f5-128">In the Location field, click the drop-down button to open the lookup.</span></span>
19. <span data-ttu-id="088f5-129">选择“库位 13”。</span><span class="sxs-lookup"><span data-stu-id="088f5-129">Select location 13.</span></span>
20. <span data-ttu-id="088f5-130">在“数量”字段中，输入一个数字。</span><span class="sxs-lookup"><span data-stu-id="088f5-130">In the Quantity field, enter a number.</span></span>
21. <span data-ttu-id="088f5-131">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="088f5-131">Click Save.</span></span>
22. <span data-ttu-id="088f5-132">单击“过帐”。</span><span class="sxs-lookup"><span data-stu-id="088f5-132">Click Post.</span></span>
23. <span data-ttu-id="088f5-133">选中或取消选中“将所有错误过帐至一个新日记帐”的复选框。</span><span class="sxs-lookup"><span data-stu-id="088f5-133">Check or uncheck the Transfer all posting errors to a new journal check box.</span></span>
    * <span data-ttu-id="088f5-134">如果您选取该选项，任意行过帐失败都将被复制到一个新的日记帐中。</span><span class="sxs-lookup"><span data-stu-id="088f5-134">If you enable this option, any lines that fail to post will be copied to a new journal.</span></span> <span data-ttu-id="088f5-135">您可以利用原信息更正该问题，然后再过帐该行。</span><span class="sxs-lookup"><span data-stu-id="088f5-135">You can use the information in the log to correct the issues and then re-post the lines.</span></span>  
24. <span data-ttu-id="088f5-136">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="088f5-136">Click OK.</span></span>
25. <span data-ttu-id="088f5-137">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="088f5-137">Close the page.</span></span>
26. <span data-ttu-id="088f5-138">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="088f5-138">Close the page.</span></span>
