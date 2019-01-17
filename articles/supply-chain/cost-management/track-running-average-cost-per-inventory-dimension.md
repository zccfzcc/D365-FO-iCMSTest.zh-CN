---
title: 按库存维度跟踪移动平均成本
description: 库存维度组附加到每个库存物料。 因此，基于选择的在财务上正跟踪的库存维度，计算某一物料的经常性平均成本价。
author: AndersGirke
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: InventOnhandItem
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 75053
ms.assetid: 68cc00f4-0f7a-4a7d-be90-8f2e0d0563d3
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: mguada
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 3c8c8eb5d053c4b5ea70a222d06ba8f025a95460
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56401"
---
# <a name="track-running-average-cost-per-inventory-dimension"></a><span data-ttu-id="ae406-104">按库存维度跟踪移动平均成本</span><span class="sxs-lookup"><span data-stu-id="ae406-104">Track running average cost per inventory dimension</span></span>

[!include [banner](../includes/banner.md)]

[!include [retail name](../includes/retail-name.md)]

<span data-ttu-id="ae406-105">库存维度组附加到每个库存物料。</span><span class="sxs-lookup"><span data-stu-id="ae406-105">An inventory dimension group is attached to every inventory item.</span></span> <span data-ttu-id="ae406-106">因此，基于选择的在财务上正跟踪的库存维度，计算某一物料的经常性平均成本价。</span><span class="sxs-lookup"><span data-stu-id="ae406-106">Therefore, the running average cost price of an item is calculated based on the selected inventory dimensions that are being tracked financially.</span></span>

<span data-ttu-id="ae406-107">库存维度有三种类型：产品，存储区和跟踪。</span><span class="sxs-lookup"><span data-stu-id="ae406-107">There are three types of inventory dimensions: product, storage, and tracking.</span></span> <span data-ttu-id="ae406-108">产品维度包括配置、大小和颜色。</span><span class="sxs-lookup"><span data-stu-id="ae406-108">Product dimensions include configuration, size, and color.</span></span> <span data-ttu-id="ae406-109">产品维度始终在财务上跟踪。</span><span class="sxs-lookup"><span data-stu-id="ae406-109">Product dimensions are always tracked financially.</span></span> <span data-ttu-id="ae406-110">存储和跟踪维度包括站点、仓库、库位、库存状态、牌照、批处理号和序列号。</span><span class="sxs-lookup"><span data-stu-id="ae406-110">Storage and tracking dimensions include site, warehouse, location, inventory status, license plate, batch number, and serial number.</span></span> <span data-ttu-id="ae406-111">您可以决定在财务上跟踪哪一存储和跟踪维度。</span><span class="sxs-lookup"><span data-stu-id="ae406-111">You can decide which storage and tracking dimensions are tracked financially.</span></span> 

<span data-ttu-id="ae406-112">**示例 1**</span><span class="sxs-lookup"><span data-stu-id="ae406-112">**Example 1**</span></span> 

<span data-ttu-id="ae406-113">如果按仓库从财务上跟踪附加到物料的存储维度组，则将为每个仓库都计算移动平均成本价。</span><span class="sxs-lookup"><span data-stu-id="ae406-113">If the storage dimension group that is attached to the item is financially tracked by warehouse, the running average cost price is calculated per warehouse.</span></span> <span data-ttu-id="ae406-114">以下采购订单已开票：</span><span class="sxs-lookup"><span data-stu-id="ae406-114">The following purchase orders have been invoiced:</span></span>

-   <span data-ttu-id="ae406-115">数量为 2 且成本价为 USD 10.00 的采购订单已为仓库 GW 开票。</span><span class="sxs-lookup"><span data-stu-id="ae406-115">A purchase order for a quantity of 2 at a cost price of USD 10.00 has been invoiced for warehouse GW.</span></span>
-   <span data-ttu-id="ae406-116">数量为 3 且成本价为 USD 12.00 的采购订单已为仓库 GW 开票。</span><span class="sxs-lookup"><span data-stu-id="ae406-116">A purchase order for a quantity of 3 at a cost price of USD 12.00 has been invoiced for warehouse GW.</span></span>
-   <span data-ttu-id="ae406-117">数量为 5 且成本价为 USD 15.00 的采购订单已为仓库 MW 开票。</span><span class="sxs-lookup"><span data-stu-id="ae406-117">A purchase order for a quantity of 5 at a cost price of USD 15.00 has been invoiced for warehouse MW.</span></span>

<span data-ttu-id="ae406-118">仓库 GW 的移动平均成本价为 USD 11.20，并且，仓库 MW 的移动平均成本价为 USD 15.00。</span><span class="sxs-lookup"><span data-stu-id="ae406-118">The running average cost price for warehouse GW is USD 11.20, and the running average cost price for warehouse MW is USD 15.00.</span></span> <span data-ttu-id="ae406-119">为仓库 GW 过帐销售订单发票。</span><span class="sxs-lookup"><span data-stu-id="ae406-119">A sales order invoice is posted for warehouse GW.</span></span> <span data-ttu-id="ae406-120">库存和所售货物成本的价值（在执行库存结转前并且未标记）将是 USD 11.20。</span><span class="sxs-lookup"><span data-stu-id="ae406-120">The value of the inventory and the cost of goods sold (before inventory close is run and without marking) is USD 11.20.</span></span> <span data-ttu-id="ae406-121">为仓库 MW 过帐另一个销售订单。</span><span class="sxs-lookup"><span data-stu-id="ae406-121">Another sales order is posted for warehouse MW.</span></span> <span data-ttu-id="ae406-122">库存和所售货物成本的价值（在执行库存结转前并且未标记）将是 USD 15.00。</span><span class="sxs-lookup"><span data-stu-id="ae406-122">The value of the inventory and the cost of goods sold (before inventory close is run and without marking) is USD 15.00.</span></span> 

<span data-ttu-id="ae406-123">**示例 2**如果附加到物料的存储维度组按仓库从财务上跟踪，并按批号从财务上跟踪跟踪维度组，则为每个批次计算移动平均成本价。</span><span class="sxs-lookup"><span data-stu-id="ae406-123">**Example 2** If the storage dimension group that is attached to the item is financially tracked by warehouse, and the tracking dimension group is financially tracked by batch number, the running average cost price is calculated for each batch.</span></span> 

<span data-ttu-id="ae406-124">**注意：** 我们建议您始终查看正在跟踪的所有财务维度的成本价。</span><span class="sxs-lookup"><span data-stu-id="ae406-124">**Note:** We recommend that you always view the cost price for all financial dimensions that are being tracked.</span></span> <span data-ttu-id="ae406-125">以下采购订单已开票：</span><span class="sxs-lookup"><span data-stu-id="ae406-125">The following purchase orders have been invoiced:</span></span>

-   <span data-ttu-id="ae406-126">数量为 2 且成本价为 USD 10.00 的采购订单已为仓库 GW 和批处理 AAA 开票。</span><span class="sxs-lookup"><span data-stu-id="ae406-126">A purchase order for a quantity of 2 at a cost price of USD 10.00 has been invoiced for warehouse GW and batch AAA.</span></span>
-   <span data-ttu-id="ae406-127">数量为 3 且成本价为 USD 12.00 的采购订单已为仓库 GW 和批处理 AAA 开票。</span><span class="sxs-lookup"><span data-stu-id="ae406-127">A purchase order for a quantity of 3 at a cost price of USD 12.00 has been invoiced for warehouse GW and batch AAA.</span></span>
-   <span data-ttu-id="ae406-128">数量为 2 且成本价为 USD 15.00 的采购订单已为仓库 GW 和批处理 BBB 开票。</span><span class="sxs-lookup"><span data-stu-id="ae406-128">A purchase order for a quantity of 2 at a cost price of USD 15.00 has been invoiced for warehouse GW and batch BBB.</span></span>

<span data-ttu-id="ae406-129">仓库 GW 和批处理 AAA 的移动平均成本价为 USD 11.20，并且，仓库 GW 和批处理 BBB 的移动平均成本价为 USD 15.00。</span><span class="sxs-lookup"><span data-stu-id="ae406-129">The running average cost price for warehouse GW and batch AAA is USD 11.20, and the running average cost price for warehouse GW and batch BBB is USD 15.00.</span></span>



