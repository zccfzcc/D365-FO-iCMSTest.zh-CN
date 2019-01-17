---
title: 在 Retail Modern POS (MPOS) 和 Cloud POS 之间选择
description: 本主题说明 Retail Modern POS 和 Cloud POS 之间的主要差别。 它还描述实现 Microsoft Dynamics 365 for Retail 的零售商应考虑的以帮助他们作出满足自己要求的最佳选择的各个因素。
author: jblucher
manager: AnnBe
ms.date: 10/12/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: ''
ms.assetid: ''
ms.search.region: global
ms.search.industry: Retail
ms.author: jeffbl
ms.search.validFrom: 2017-10-12
ms.dyn365.ops.version: AX 7.0.0, Retail July 2017 update
ms.openlocfilehash: a6e3be5116b3cf0ccda5193b8bcc5a575a1df0bc
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56133"
---
# <a name="choose-between-retail-modern-pos-mpos-and-cloud-pos"></a><span data-ttu-id="db5a8-104">在 Retail Modern POS (MPOS) 和 Cloud POS 之间选择</span><span class="sxs-lookup"><span data-stu-id="db5a8-104">Choose between Retail Modern POS (MPOS) and Cloud POS</span></span>

[!include [banner](includes/banner.md)]

<span data-ttu-id="db5a8-105">此主题为实施人员提供在部署 Microsoft Dynamics 365 for Retail 时应该考虑的因素的其他背景、建议和指南。</span><span class="sxs-lookup"><span data-stu-id="db5a8-105">This topic gives implementers additional background, tips, and guidance for factors that they should consider when they deploy Microsoft Dynamics 365 for Retail.</span></span> <span data-ttu-id="db5a8-106">通过查看并在部署过程中遵循此指导，实施人员可以避免可能会影响用户满意度或性能的问题。</span><span class="sxs-lookup"><span data-stu-id="db5a8-106">By reviewing and following this guidance as part of the deployment process, implementers can avoid issues that might affect user satisfaction or performance.</span></span>

## <a name="insights"></a><span data-ttu-id="db5a8-107">洞察力</span><span class="sxs-lookup"><span data-stu-id="db5a8-107">Insights</span></span>
<span data-ttu-id="db5a8-108">Retail 提供多种部署和拓扑选项。</span><span class="sxs-lookup"><span data-stu-id="db5a8-108">Retail provides a wide range of deployment and topology options.</span></span> <span data-ttu-id="db5a8-109">因此，零售商可以选择最满足其业务和技术要求的组件和配置。</span><span class="sxs-lookup"><span data-stu-id="db5a8-109">Therefore, retailers can choose the components and configuration that best meet their business and technology requirements.</span></span> <span data-ttu-id="db5a8-110">需要仔细考虑的一个实现方面是平台的选择和销售点 (POS) 组件的窗体因子。</span><span class="sxs-lookup"><span data-stu-id="db5a8-110">One aspect of implementation that requires careful consideration is the choice of a platform and form factor for the point of sale (POS) component.</span></span>

### <a name="pos-platform-and-form-factor-considerations"></a><span data-ttu-id="db5a8-111">POS 平台和窗体因子考虑事项</span><span class="sxs-lookup"><span data-stu-id="db5a8-111">POS platform and form factor considerations</span></span>
<span data-ttu-id="db5a8-112">Retail 支持以下 POS 选项：</span><span class="sxs-lookup"><span data-stu-id="db5a8-112">Retail supports the following POS options:</span></span>

- <span data-ttu-id="db5a8-113">适用于 Microsoft Windows 的 Retail Modern POS (MPOS)</span><span class="sxs-lookup"><span data-stu-id="db5a8-113">Retail Modern POS (MPOS) for Microsoft Windows</span></span>
- <span data-ttu-id="db5a8-114">适用于 Microsoft Windows Phone 的 MPOS</span><span class="sxs-lookup"><span data-stu-id="db5a8-114">MPOS for Microsoft Windows Phone</span></span>
- <span data-ttu-id="db5a8-115">适用于 Apple iPad 或 Google Android 平板电脑的 MPOS</span><span class="sxs-lookup"><span data-stu-id="db5a8-115">MPOS for Apple iPad or Google Android tablet</span></span>
- <span data-ttu-id="db5a8-116">Cloud POS (CPOS) 支持 Microsoft Edge、Internet Explorer 和 Google Chrome 浏览器</span><span class="sxs-lookup"><span data-stu-id="db5a8-116">Cloud POS (CPOS), which supports the Microsoft Edge, Internet Explorer, and Google Chrome browsers</span></span>

<span data-ttu-id="db5a8-117">在任何情况下，POS（MPOS 和 CPOS）都共享同一个核心应用程序代码。</span><span class="sxs-lookup"><span data-stu-id="db5a8-117">In all cases, the POS (MPOS and CPOS) shares the same core application code.</span></span> <span data-ttu-id="db5a8-118">由于以下原因这一点很重要：</span><span class="sxs-lookup"><span data-stu-id="db5a8-118">This point is important for the following reasons:</span></span>

- <span data-ttu-id="db5a8-119">用户界面 (UI) 是一致的，不管平台或窗体因子如何。</span><span class="sxs-lookup"><span data-stu-id="db5a8-119">The user interface (UI) is consistent, regardless of the platform or form factor.</span></span>
- <span data-ttu-id="db5a8-120">大多数功能能力是相同的，无论平台或窗体因子如何。</span><span class="sxs-lookup"><span data-stu-id="db5a8-120">Most of the functional capabilities are the same, regardless of the platform or form factor.</span></span> <span data-ttu-id="db5a8-121">不过，也存在某些重要差异。</span><span class="sxs-lookup"><span data-stu-id="db5a8-121">However, there are some important differences.</span></span> <span data-ttu-id="db5a8-122">这些差异在本主题中有说明。</span><span class="sxs-lookup"><span data-stu-id="db5a8-122">These differences are noted in this topic.</span></span>
- <span data-ttu-id="db5a8-123">在指定商店中，POS 差异可以合并，并可以同时运行。</span><span class="sxs-lookup"><span data-stu-id="db5a8-123">In a given store, the POS variations can be combined and can run concurrently.</span></span> <span data-ttu-id="db5a8-124">例如，对于其主要收银机，零售商可以在运行 Windows 的计算机上使用 MPOS。</span><span class="sxs-lookup"><span data-stu-id="db5a8-124">For example, for its main registers, a retailer can use MPOS on computers that run Windows.</span></span> <span data-ttu-id="db5a8-125">但是，零售商可以使用基于浏览器的终端或移动设备补充这些收银机。</span><span class="sxs-lookup"><span data-stu-id="db5a8-125">However, the retailer can supplement those registers with browser-based terminals or mobile devices.</span></span>
- <span data-ttu-id="db5a8-126">自定义和扩展可以跨平台和窗体因子轻松使用。</span><span class="sxs-lookup"><span data-stu-id="db5a8-126">Customizations and extensions can easily be used across platforms and form factors.</span></span> <span data-ttu-id="db5a8-127">由于核心应用程序代码被共享，大多数自定义可以实施一次，而不是多次。</span><span class="sxs-lookup"><span data-stu-id="db5a8-127">Because the core application code is shared, most customizations can be implemented one time instead of multiple times.</span></span>

### <a name="mpos-vs-cpos"></a><span data-ttu-id="db5a8-128">MPOS 与 CPOS</span><span class="sxs-lookup"><span data-stu-id="db5a8-128">MPOS vs. CPOS</span></span>
<span data-ttu-id="db5a8-129">尽管 MPOS 和 CPOS 大部分是相同的，但您必须了解某些重要的差异。</span><span class="sxs-lookup"><span data-stu-id="db5a8-129">Although MPOS and CPOS are largely the same, there are some important differences that you must understand.</span></span>

#### <a name="mpos"></a><span data-ttu-id="db5a8-130">MPOS</span><span class="sxs-lookup"><span data-stu-id="db5a8-130">MPOS</span></span>

<span data-ttu-id="db5a8-131">Windows、iOS 或 Android 设备上的 MPOS 是在该设备上打包、安装和服务的应用程序。</span><span class="sxs-lookup"><span data-stu-id="db5a8-131">MPOS on a Windows, iOS, or Android device is an application that is packaged, installed, and serviced on that device.</span></span>

- <span data-ttu-id="db5a8-132">**Windows** – Windows 应用程序的 MPOS 包含所有应用程序代码和嵌入的 Commerce Runtime (CRT)。</span><span class="sxs-lookup"><span data-stu-id="db5a8-132">**Windows** – The MPOS for Windows application contains all the application code and the embedded commerce runtime (CRT).</span></span> 
- <span data-ttu-id="db5a8-133">**iOS/Android** – 在这些平台上，此应用程序充当 CPOS 应用程序代码的主机。</span><span class="sxs-lookup"><span data-stu-id="db5a8-133">**iOS/Android** – On these platforms, the application acts as a host for the CPOS application code.</span></span> <span data-ttu-id="db5a8-134">换言之，应用程序代码来自 Microsoft Azure 或零售商店扩展单位 (RSSU) 上的 CPOS 服务器。</span><span class="sxs-lookup"><span data-stu-id="db5a8-134">In other words, the application code comes from the CPOS server on Microsoft Azure or the Retail Store Scale Unit (RSSU).</span></span> <span data-ttu-id="db5a8-135">有关详细信息，请参阅[零售商店扩展单位概览](https://docs.microsoft.com/en-us/dynamics365/unified-operations/retail/dev-itpro/retail-store-system-begin)。</span><span class="sxs-lookup"><span data-stu-id="db5a8-135">For more information, see [Retail Store Scale Unit overview](https://docs.microsoft.com/en-us/dynamics365/unified-operations/retail/dev-itpro/retail-store-system-begin).</span></span>

#### <a name="cpos"></a><span data-ttu-id="db5a8-136">CPOS</span><span class="sxs-lookup"><span data-stu-id="db5a8-136">CPOS</span></span>

<span data-ttu-id="db5a8-137">由于 CPOS 在浏览器中运行，应用程序不在设备上安装。</span><span class="sxs-lookup"><span data-stu-id="db5a8-137">Because CPOS runs in a browser, the application isn't installed on the device.</span></span> <span data-ttu-id="db5a8-138">浏览器改从 CPOS 服务器访问应用程序代码。</span><span class="sxs-lookup"><span data-stu-id="db5a8-138">Instead, the browser accesses the application code from the CPOS server.</span></span> <span data-ttu-id="db5a8-139">因此，CPOS 不能直接访问 POS 硬件或在脱机状态下工作。</span><span class="sxs-lookup"><span data-stu-id="db5a8-139">Therefore, CPOS can't directly access POS hardware or work in an offline state.</span></span>

### <a name="store-deployment-considerations"></a><span data-ttu-id="db5a8-140">商店部署注意事项</span><span class="sxs-lookup"><span data-stu-id="db5a8-140">Store deployment considerations</span></span>
<span data-ttu-id="db5a8-141">除了平台和窗体因子外，零售商还必须在商店选择部署选项。</span><span class="sxs-lookup"><span data-stu-id="db5a8-141">In addition to a platform and form factor, retailers must also choose a deployment option at the store.</span></span> <span data-ttu-id="db5a8-142">下表显示每个 POS 选项可用的配置。</span><span class="sxs-lookup"><span data-stu-id="db5a8-142">The following table shows the configurations that are available for each POS option.</span></span>

| <span data-ttu-id="db5a8-143">POS 应用程序</span><span class="sxs-lookup"><span data-stu-id="db5a8-143">POS application</span></span>         | <span data-ttu-id="db5a8-144">Retail Server</span><span class="sxs-lookup"><span data-stu-id="db5a8-144">Retail server</span></span> | <span data-ttu-id="db5a8-145">脱机可用</span><span class="sxs-lookup"><span data-stu-id="db5a8-145">Available offline</span></span> |
|-------------------------|---------------|-------------------|
| <span data-ttu-id="db5a8-146">适用于 Windows 的 MPOS</span><span class="sxs-lookup"><span data-stu-id="db5a8-146">MPOS for Windows</span></span>        | <span data-ttu-id="db5a8-147">云或 RSSU</span><span class="sxs-lookup"><span data-stu-id="db5a8-147">Cloud or RSSU</span></span> | <span data-ttu-id="db5a8-148">是</span><span class="sxs-lookup"><span data-stu-id="db5a8-148">Yes</span></span>               |
| <span data-ttu-id="db5a8-149">适用于 iOS 或 Android 的 MPOS</span><span class="sxs-lookup"><span data-stu-id="db5a8-149">MPOS for iOS or Android</span></span> | <span data-ttu-id="db5a8-150">云或 RSSU</span><span class="sxs-lookup"><span data-stu-id="db5a8-150">Cloud or RSSU</span></span> | <span data-ttu-id="db5a8-151">无</span><span class="sxs-lookup"><span data-stu-id="db5a8-151">No</span></span>                |
| <span data-ttu-id="db5a8-152">云 POS</span><span class="sxs-lookup"><span data-stu-id="db5a8-152">Cloud POS</span></span>               | <span data-ttu-id="db5a8-153">云或 RSSU</span><span class="sxs-lookup"><span data-stu-id="db5a8-153">Cloud or RSSU</span></span> | <span data-ttu-id="db5a8-154">无</span><span class="sxs-lookup"><span data-stu-id="db5a8-154">No</span></span>                |

#### <a name="retail-server"></a><span data-ttu-id="db5a8-155">Retail Server</span><span class="sxs-lookup"><span data-stu-id="db5a8-155">Retail server</span></span>

<span data-ttu-id="db5a8-156">Retail 服务器是承载 CRT 的组件。</span><span class="sxs-lookup"><span data-stu-id="db5a8-156">The Retail server is a component that hosts the CRT.</span></span> <span data-ttu-id="db5a8-157">CRT 包含 POS 使用的所有业务逻辑，并提供对渠道数据库的访问。</span><span class="sxs-lookup"><span data-stu-id="db5a8-157">The CRT contains all the business logic that the POS uses, and it provides access to the channel database.</span></span> <span data-ttu-id="db5a8-158">当在线时，商店中的所有 POS 客户端均使用 Retail 服务器。</span><span class="sxs-lookup"><span data-stu-id="db5a8-158">While they are online, all POS clients in the store use the Retail server.</span></span> <span data-ttu-id="db5a8-159">Retail 服务器可以在云或商店 (RSSU) 中部署。</span><span class="sxs-lookup"><span data-stu-id="db5a8-159">The Retail server can be deployed either in the cloud or in the store (RSSU).</span></span>

#### <a name="offline-mode"></a><span data-ttu-id="db5a8-160">脱机模式</span><span class="sxs-lookup"><span data-stu-id="db5a8-160">Offline mode</span></span>

<span data-ttu-id="db5a8-161">适用于 Windows 的 MPOS 支持脱机模式。</span><span class="sxs-lookup"><span data-stu-id="db5a8-161">MPOS for Windows supports offline mode.</span></span> <span data-ttu-id="db5a8-162">在脱机模式下，POS 可以继续处理销售，即使它从 Retail 服务器断开。</span><span class="sxs-lookup"><span data-stu-id="db5a8-162">In offline mode, the POS can continue to process sales even if it's disconnected from the Retail server.</span></span> <span data-ttu-id="db5a8-163">在恢复连接时，它可以与渠道数据库同步。</span><span class="sxs-lookup"><span data-stu-id="db5a8-163">It can then be synchronized with the channel database when connectivity is restored.</span></span> <span data-ttu-id="db5a8-164">MPOS 使用其自己的嵌入 CRT 实例，并暂时使用其自己的本地数据源（脱机 SQL Server 数据库）。</span><span class="sxs-lookup"><span data-stu-id="db5a8-164">MPOS uses its own embedded instance of the CRT and temporarily uses its own local data source (offline SQL Server database).</span></span> <span data-ttu-id="db5a8-165">有关脱机功能的详细信息，请参阅 [POS 脱机功能](https://docs.microsoft.com/en-us/dynamics365/unified-operations/retail/pos-offline-functionality)。</span><span class="sxs-lookup"><span data-stu-id="db5a8-165">For more information about offline functionality, see [POS offline functionality](https://docs.microsoft.com/en-us/dynamics365/unified-operations/retail/pos-offline-functionality).</span></span>

### <a name="pos-peripheralhardware-considerations"></a><span data-ttu-id="db5a8-166">POS 外设/硬件注意事项</span><span class="sxs-lookup"><span data-stu-id="db5a8-166">POS peripheral/hardware considerations</span></span>
<span data-ttu-id="db5a8-167">零售商还必须考虑 POS 如何访问打印机、银箱和付款终端等设备和外设。</span><span class="sxs-lookup"><span data-stu-id="db5a8-167">Retailers must also consider how the POS will access devices and peripherals such as printers, cash drawers, and payment terminals.</span></span> <span data-ttu-id="db5a8-168">仅适用于 Windows 的 MPOS 支持与这些设备的直接通信。</span><span class="sxs-lookup"><span data-stu-id="db5a8-168">Only MPOS for Windows supports direct communication with these devices.</span></span> <span data-ttu-id="db5a8-169">适用于 Windows Phone、iOS 或 Android 的 MPOS 和 Cloud POS 需要硬件工作站来访问这些设备。</span><span class="sxs-lookup"><span data-stu-id="db5a8-169">MPOS for Windows Phone, iOS, or Android, and Cloud POS require a hardware station in order to access these devices.</span></span> <span data-ttu-id="db5a8-170">硬件工作站可专用于 POS 收银机或在商店中的收银机之间共用。</span><span class="sxs-lookup"><span data-stu-id="db5a8-170">Hardware stations can be dedicated to a POS register or shared among the registers in a store.</span></span> <span data-ttu-id="db5a8-171">有关硬件工作站的详细信息，请参阅[配置和安装 Retail 硬件工作站](https://docs.microsoft.com/en-us/dynamics365/unified-operations/retail/retail-hardware-station-configuration-installation)。</span><span class="sxs-lookup"><span data-stu-id="db5a8-171">For more information about hardware stations, see [Configure and install Retail hardware station](https://docs.microsoft.com/en-us/dynamics365/unified-operations/retail/retail-hardware-station-configuration-installation).</span></span>

## <a name="implementation-considerations"></a><span data-ttu-id="db5a8-172">实施注意事项</span><span class="sxs-lookup"><span data-stu-id="db5a8-172">Implementation considerations</span></span>
<span data-ttu-id="db5a8-173">在您规划零售店的 POS 实现时请考虑以下信息：</span><span class="sxs-lookup"><span data-stu-id="db5a8-173">Consider the following information as you plan your POS implementation in your retail stores:</span></span>

- <span data-ttu-id="db5a8-174">**功能要求** – 核心业务流程和功能是相同的，不论平台、窗体因子或部署拓扑如何。</span><span class="sxs-lookup"><span data-stu-id="db5a8-174">**Functional requirements** – The core business processes and capabilities are the same, regardless of the platform, form factor, or deployment topology.</span></span> <span data-ttu-id="db5a8-175">因此，大多数零售商在规划其实现时不必考虑功能要求。</span><span class="sxs-lookup"><span data-stu-id="db5a8-175">Therefore, most retailers don't have to consider functional requirements when they plan their implementation.</span></span>
- <span data-ttu-id="db5a8-176">**连接** - 网络可用性（广域网 \[WAN\] 和局域网 \[LAN\]）是需要仔细考虑的一个主要因素。</span><span class="sxs-lookup"><span data-stu-id="db5a8-176">**Connectivity** - Network availability (wide area network \[WAN\] and local area network \[LAN\]) is a major factor that requires careful consideration.</span></span> <span data-ttu-id="db5a8-177">如果系统不可用于业务关键型流程，那么零占地的云托管解决方案在成本和简化方面带来的任何优势都将消失。</span><span class="sxs-lookup"><span data-stu-id="db5a8-177">Any benefits that a zero-footprint, cloud-hosted solution brings in terms of cost and simplicity are lost if the system isn't available for business-critical processes.</span></span>

    <span data-ttu-id="db5a8-178">除非特定设备的连接非常可靠和灵活，或者零售商可以接受一定的停机时间，否则我们建议以下选项之一：</span><span class="sxs-lookup"><span data-stu-id="db5a8-178">Unless the connectivity for a given device is very dependable and resilient, or unless a certain amount of downtime is acceptable to the retailer, we recommend one of the following options:</span></span>

  - <span data-ttu-id="db5a8-179">在 Windows 中使用 MPOS，并启用脱机模式。</span><span class="sxs-lookup"><span data-stu-id="db5a8-179">Use MPOS in Windows, and enable offline mode.</span></span>
  - <span data-ttu-id="db5a8-180">部署本地 RSSU。</span><span class="sxs-lookup"><span data-stu-id="db5a8-180">Deploy an on-premises RSSU.</span></span>

    <span data-ttu-id="db5a8-181">这两个选项不彼此排斥。</span><span class="sxs-lookup"><span data-stu-id="db5a8-181">These two options aren't mutually exclusive.</span></span> <span data-ttu-id="db5a8-182">对于最可靠的拓扑，零售商可以部署本地 RSSU 以减少对互联网连接与 Azure 可用性的依赖，如果本地服务器或网络有问题，他们还可以部署启用脱机模式的 POS 收银机。</span><span class="sxs-lookup"><span data-stu-id="db5a8-182">For the most reliable topology, retailers can deploy a local RSSU to reduce the dependency on internet connectivity or Azure availability, and they can also deploy POS registers where offline mode is enabled if there is an issue with the local server or network.</span></span>

- <span data-ttu-id="db5a8-183">**硬件设备/外设** – Retail POS 系统的一个重要方面是它能够使用 POS 外设，如打印机、银箱和付款终端。</span><span class="sxs-lookup"><span data-stu-id="db5a8-183">**Hardware devices/peripherals** – One important aspect of a Retail POS system is its ability to use POS peripherals such as printers, cash drawers, and payment terminals.</span></span> <span data-ttu-id="db5a8-184">虽然所有可用 POS 选项均可以使用外设，但只有适用于 Windows 的 MPOS 直接支持它们。</span><span class="sxs-lookup"><span data-stu-id="db5a8-184">Although all the available POS options can use peripheral devices, only MPOS for Windows supports them directly.</span></span> <span data-ttu-id="db5a8-185">对于所有其他应用程序，均需要一个或多个硬件工作站。</span><span class="sxs-lookup"><span data-stu-id="db5a8-185">For all other applications, one or more hardware stations are required.</span></span> <span data-ttu-id="db5a8-186">虽然此方法增加了灵活性，但必须部署、配置和服务其他组件。</span><span class="sxs-lookup"><span data-stu-id="db5a8-186">Although this approach adds flexibility, additional components must be deployed, configured, and serviced.</span></span>
- <span data-ttu-id="db5a8-187">**系统要求** – POS 应用程序的系统要求会发生变化。</span><span class="sxs-lookup"><span data-stu-id="db5a8-187">**System requirements** – The system requirements for the POS application vary.</span></span> <span data-ttu-id="db5a8-188">在您进行选择前，请确保检查最新信息。</span><span class="sxs-lookup"><span data-stu-id="db5a8-188">Be sure to check the latest information before you make your choice.</span></span> <span data-ttu-id="db5a8-189">例如，因为 CPOS 在浏览器中运行，它支持各种操作系统。</span><span class="sxs-lookup"><span data-stu-id="db5a8-189">For example, because CPOS runs in a browser, it supports a wider range of operating systems.</span></span> <span data-ttu-id="db5a8-190">有关系统要求的详细信息，请参阅[云部署的系统要求](https://docs.microsoft.com/en-us/dynamics365/unified-operations/fin-and-ops/get-started/system-requirements)。</span><span class="sxs-lookup"><span data-stu-id="db5a8-190">For more information about system requirements, see [System requirements for cloud deployments](https://docs.microsoft.com/en-us/dynamics365/unified-operations/fin-and-ops/get-started/system-requirements).</span></span>
- <span data-ttu-id="db5a8-191">**部署和服务** – 部署和服务要求的复杂程度可能因应用程序和部署选择的更改而改变。</span><span class="sxs-lookup"><span data-stu-id="db5a8-191">**Deployment and servicing** – The complexity of the deployment and servicing requirements can vary, depending on the application and deployment choices.</span></span> <span data-ttu-id="db5a8-192">例如，对于云托管的 CPOS 部署，您不必在每台设备上安装和更新。</span><span class="sxs-lookup"><span data-stu-id="db5a8-192">For example, for a cloud-hosted CPOS deployment, you don't have to install and update on every device.</span></span> <span data-ttu-id="db5a8-193">因此，此方法将极大地减少复杂性和成本。</span><span class="sxs-lookup"><span data-stu-id="db5a8-193">Therefore, this approach greatly reduces complexity and cost.</span></span> <span data-ttu-id="db5a8-194">但是，如果您在每个收银机上部署 MPOS 并启用脱机模式，而且您还部署了共享的硬件工作站，这会大大增加必须管理的终结点数量。</span><span class="sxs-lookup"><span data-stu-id="db5a8-194">However, if you deploy MPOS on every register and enable offline mode, and you also deploy shared hardware stations, you greatly increase the number of endpoints that must be managed.</span></span>