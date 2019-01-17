---
title: 运输负荷部分装运
description: 本主题说明如何部分装运装载和推迟规划装载的产能。
author: Mirzaab
manager: AnnBe
ms.date: 03/15/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WHSTransportLoad
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 1705903
ms.assetid: 427e01b3-4968-4cff-9b85-1717530f72e4
ms.search.region: Global
ms.author: mirzaab
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 8.0.0
ms.openlocfilehash: 2c6db36433a21ff5d49f44b83e9abb50a3da6b80
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55896"
---
# <a name="partial-shipment-of-a-transport-load"></a><span data-ttu-id="e7fe3-103">运输负荷部分装运</span><span class="sxs-lookup"><span data-stu-id="e7fe3-103">Partial shipment of a transport load</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="e7fe3-104">通过为装载设置部分装运，可处理其产能在所有行都添加到装载之前无法确定的装载。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-104">By setting up partial shipment of loads, you can handle loads where the capacity can't be determined until all the sales lines have been added to a load.</span></span> <span data-ttu-id="e7fe3-105">了解到精确的货盘计数时，即可完成此过程。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-105">The process can then be finalized when the exact pallet count is known.</span></span> <span data-ttu-id="e7fe3-106">因此，在货物实物从分阶段库存实际运出之前，无需确定为哪些运输分配哪些货盘。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-106">Therefore, you don't have to decide which pallets will be assigned to which transport until the moment when a transport is being physically loaded out of the staged inventory.</span></span>

<span data-ttu-id="e7fe3-107">此功能提供了备用方法来代替更严格结构的实施，在后者中，必须先确定为哪些运输分配哪些货盘，才能创建领料工作或装载工作。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-107">This feature offers an alternative to the enforcement of a more rigid structure, where you must determine which pallets will be assigned to which transport before picking work or loading work can be created.</span></span> <span data-ttu-id="e7fe3-108">相反，用户可为单个装载配置部分装运确认。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-108">Instead, users can configure individual loads for a partial shipment confirmation.</span></span> <span data-ttu-id="e7fe3-109">然后，可能会对这些装载进行运输负荷处理。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-109">The transport loading processes for those loads can then occur.</span></span> <span data-ttu-id="e7fe3-110">因此，运输规划部门在规划装载时不必考虑单次运输的产能。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-110">Therefore, the transportation planning department can plan loads without having to consider the capacity of individual transports.</span></span>

<span data-ttu-id="e7fe3-111">装载时，工作人员可定义可将货盘装载到的新运输负荷。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-111">At the time of loading, workers can define a new transport load that a pallet can be loaded to.</span></span> <span data-ttu-id="e7fe3-112">也可以识别现有运输负荷。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-112">Alternatively, they can identify an existing transport load.</span></span> <span data-ttu-id="e7fe3-113">可通过移动设备记录此数据。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-113">This data can be recorded via a mobile device.</span></span> <span data-ttu-id="e7fe3-114">因此，几位仓库工作人员可将库存从同一个负荷或不同负荷装载到同一辆卡车。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-114">Therefore, several warehouse workers can load inventory from the same loads or different loads onto the same truck.</span></span> <span data-ttu-id="e7fe3-115">然后可全部或部分装运这些负荷。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-115">The loads can then be fully or partially shipped.</span></span>

> [!NOTE] 
> <span data-ttu-id="e7fe3-116">要将库存从负荷装载到特定运输负荷，并部分装运负荷，必须通过使用工作模板中的装载类生成工作。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-116">In order to load inventory from a load to a specific transport load and partially ship the load, work must be generated by using a loading class in a work template.</span></span> <span data-ttu-id="e7fe3-117">不能将**领料**类型的普通领料工作装载到运输负荷，如卡车。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-117">Ordinary picking work of the **Picking** type can't be loaded to a transport load such as a truck.</span></span>

## <a name="set-up-transport-loads-for-partial-shipment"></a><span data-ttu-id="e7fe3-118">为部分装运设置运输负荷</span><span class="sxs-lookup"><span data-stu-id="e7fe3-118">Set up transport loads for partial shipment</span></span>

<span data-ttu-id="e7fe3-119">负荷的部分装运设置分为下面的两个步骤。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-119">The setup for partial shipment of loads consists of the following two procedures.</span></span>

### <a name="set-the-loading-strategy"></a><span data-ttu-id="e7fe3-120">设置装载策略</span><span class="sxs-lookup"><span data-stu-id="e7fe3-120">Set the loading strategy</span></span>

<span data-ttu-id="e7fe3-121">必须通过设置装载处理启用部分装载。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-121">You must enable partial loading by setting the loading strategy.</span></span> <span data-ttu-id="e7fe3-122">创建负荷后，可设置装载策略。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-122">You can set the loading strategy after you've created a load.</span></span>

1. <span data-ttu-id="e7fe3-123">选择**仓库管理** \> **负荷** \> **所有负荷**。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-123">Select **Warehouse management** \> **Loads** \> **All loads**.</span></span>
2. <span data-ttu-id="e7fe3-124">选择一个负荷，然后单击 **标题**。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-124">Select a load, and then click **Header**.</span></span>
3. <span data-ttu-id="e7fe3-125">在**装载策略**字段中，选择 **允许部分负荷装运**。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-125">In the **Loading strategy** field, select **Partial load shipping allowed**.</span></span>

### <a name="create-a-menu-item-for-loading-of-transport-loads"></a><span data-ttu-id="e7fe3-126">为装载运输装运创建一个菜单项。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-126">Create a menu item for loading of transport loads</span></span>

<span data-ttu-id="e7fe3-127">必须创建一个新的菜单项，用于启用要装载的运输负荷。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-127">You must create a new menu item that enables transport loads to be loaded.</span></span> <span data-ttu-id="e7fe3-128">可通过运输负荷为来自一个负荷或多个负荷的工作行分组。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-128">A transport load lets you group work lines from one load or multiple loads.</span></span> <span data-ttu-id="e7fe3-129">然后可通过使用移动扫描仪装运添加到运输负荷的所有物品。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-129">Everything that is added to the transport load can then be shipped by using a mobile scanner.</span></span>

1. <span data-ttu-id="e7fe3-130">选择**仓库管理** \> **设置** \> **移动设备** \> **移动设备菜单项**。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-130">Select **Warehouse management** \> **Setup** \> **Mobile device** \> **Mobile device menu items**.</span></span>
2. <span data-ttu-id="e7fe3-131">选择**新建**，然后在**模式**字段中选择**工作**。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-131">Select **New**, and then, in the **Mode** field, select **Work**.</span></span>
3. <span data-ttu-id="e7fe3-132">将**使用现有工作**选项设置为**是**。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-132">Set the **Use existing work** option to **Yes**.</span></span>
4. <span data-ttu-id="e7fe3-133">在**常规**选项卡中，在**主管**字段内选择**运输装载**。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-133">On the **General** tab, in the **Directed by** field, select **Transport loading**.</span></span>
5. <span data-ttu-id="e7fe3-134">若要在移动扫描仪上启用装运确认，请在**允许的装运确认类型**字段中选择**运输负荷**。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-134">To enable shipment confirmation on a mobile scanner, in the **Allowed ship confirmation type** field, select **Transport load**.</span></span>

## <a name="confirm-shipment-of-a-transport-load-from-the-client"></a><span data-ttu-id="e7fe3-135">从客户端确认运输负荷的装运</span><span class="sxs-lookup"><span data-stu-id="e7fe3-135">Confirm shipment of a transport load from the client</span></span>

<span data-ttu-id="e7fe3-136">可通过此设置确认包含要装运的完全符合或部分装载符合的运输负荷。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-136">This setup lets you confirm a transport load that includes a full load or a partially loaded load to be shipped.</span></span>

1. <span data-ttu-id="e7fe3-137">选择**仓库管理** \> **负荷** \> **运输负荷**。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-137">Select **Warehouse management** \> **Loads** \> **Transport loads**.</span></span>
2. <span data-ttu-id="e7fe3-138">在操作窗格上**装运和接收**选项卡上**确认**组中，选择**运输**。</span><span class="sxs-lookup"><span data-stu-id="e7fe3-138">On the Action Pane, on the **Ship and receive** tab, in the **Confirm** group, select **Transport**.</span></span>