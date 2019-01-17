---
title: 设置领料短缺的物料重新分配
description: 此过程显示如何启用仓库工作人员，以便在为其指示的库位的库存不足时，快速找到备用库位。
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WHSWorkException, WHSWorker
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Distribution
ms.author: mirzaab
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: b24d9622d0756811e08d8ae93eb97b9039bac3c8
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56165"
---
# <a name="set-up-short-picking-item-reallocation"></a><span data-ttu-id="2ecb3-103">设置领料短缺的物料重新分配</span><span class="sxs-lookup"><span data-stu-id="2ecb3-103">Set up short picking item reallocation</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="2ecb3-104">此过程显示如何启用仓库工作人员，以便在为其指示的库位的库存不足时，快速找到备用库位。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-104">This procedure shows you how to enable warehouse workers to quickly find alternative locations if there isn’t sufficient inventory at the location they’ve been directed to.</span></span> <span data-ttu-id="2ecb3-105">可以使用自动重新分配流程，该流程使用库位指令检索货物，前提是这些货物在另一个库位可用。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-105">It’s possible to use an automatic re-allocation process, which uses location directives to retrieve the goods if they’re available at another location.</span></span> <span data-ttu-id="2ecb3-106">此外，如果使用手动重新分配，则移动设备上将显示库位列表和可用数量，供仓库工作人员选择使用哪个库位的库存。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-106">Alternatively, when manual re-allocation is used, a list of the locations with the available quantity is shown on the mobile device, allowing the warehouse worker to choose which location to use inventory from.</span></span> <span data-ttu-id="2ecb3-107">您可以在演示数据公司 USMF 中使用此过程。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-107">You can use this procedure in demo data company USMF.</span></span> <span data-ttu-id="2ecb3-108">此过程针对 Dynamics 365 for Operations 版本 1611 中增加的一项功能。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-108">This procedure is for a feature that was added in Dynamics 365 for Operations version 1611.</span></span>


## <a name="set-up-work-exceptions"></a><span data-ttu-id="2ecb3-109">设置工作异常</span><span class="sxs-lookup"><span data-stu-id="2ecb3-109">Set up work exceptions</span></span>
1. <span data-ttu-id="2ecb3-110">转到“仓库管理”>“设置”>“工作”>“工作异常”。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-110">Go to Warehouse management > Setup > Work > Work exceptions.</span></span>
2. <span data-ttu-id="2ecb3-111">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-111">Click New.</span></span>
    * <span data-ttu-id="2ecb3-112">可以使用不同物料重新分配策略定义多个工作异常，以便让仓库工作人员可以根据处理的装运需求选择一个。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-112">It’s possible to define several work exceptions with different item reallocation policies to enable the warehouse worker to choose one based on the needs of the shipment that they are processing.</span></span>  
3. <span data-ttu-id="2ecb3-113">在”工作异常代码“字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-113">In the Work exception code field, type a value.</span></span>
    * <span data-ttu-id="2ecb3-114">为工作异常分配标题以指示其用途。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-114">Give the work exception a title to indicate what it’s used for.</span></span> <span data-ttu-id="2ecb3-115">例如，“手动领料短缺”。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-115">For example, Short picking manual.</span></span>  
4. <span data-ttu-id="2ecb3-116">在“描述”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-116">In the Description field, type a value.</span></span>
5. <span data-ttu-id="2ecb3-117">在“异常类型”字段中，选择“领料短缺”。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-117">In the Exception type field, select 'Short pick'.</span></span>
6. <span data-ttu-id="2ecb3-118">选中“调整库存”复选框。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-118">Select the Adjust inventory check box.</span></span>
    * <span data-ttu-id="2ecb3-119">此选项意味着领料短缺库位自动将库存调整为 0。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-119">This option means that inventory will automatically be adjusted to 0 at the short picked location.</span></span>  
7. <span data-ttu-id="2ecb3-120">在“默认调整类型代码”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-120">In the Default adjustment type code field, enter or select a value.</span></span>
    * <span data-ttu-id="2ecb3-121">例如，在 USMF 中，可以选择“删除 Res Adj Out”。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-121">For example, in USMF you can select 'Remove Res Adj Out'.</span></span>  
8. <span data-ttu-id="2ecb3-122">在“物料重新分配”字段中，选择“手动”。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-122">In the Item reallocation field, select 'Manual'.</span></span>
    * <span data-ttu-id="2ecb3-123">如果选择“手动”或“自动和手动”，需要启用仓库工作人员才能使用手动重新分配。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-123">If you select Manual, or Automatic and Manual, the warehouse worker needs to be enabled to use manual reallocation.</span></span>  

## <a name="set-up-a-worker-to-use-manual-item-reallocation"></a><span data-ttu-id="2ecb3-124">设置工作人员以使用物料手动重新分配</span><span class="sxs-lookup"><span data-stu-id="2ecb3-124">Set up a worker to use manual item reallocation</span></span>
1. <span data-ttu-id="2ecb3-125">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-125">Close the page.</span></span>
2. <span data-ttu-id="2ecb3-126">转到“仓库管理”>“设置”>“工作人员”。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-126">Go to Warehouse management > Setup > Worker.</span></span>
3. <span data-ttu-id="2ecb3-127">单击“编辑”。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-127">Click Edit.</span></span>
4. <span data-ttu-id="2ecb3-128">在列表中，选择工作人员 24。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-128">In the list, select worker 24.</span></span>
5. <span data-ttu-id="2ecb3-129">展开“工作”部分。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-129">Expand the Work section.</span></span>
6. <span data-ttu-id="2ecb3-130">在“允许手动重新分配物料”字段中选择“是”。</span><span class="sxs-lookup"><span data-stu-id="2ecb3-130">Select Yes in the Allow manual item reallocation field.</span></span>
