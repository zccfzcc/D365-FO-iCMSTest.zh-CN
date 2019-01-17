---
title: 销售点 (POS) 的屏幕布局
description: 此主题提供有关 Microsoft Dynamics 365 for Retail 销售点 (POS) 体验的屏幕布局的信息。
author: jblucher
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
ms.search.form: RetailTillLayout
audience: Application user
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 90573
ms.assetid: a6868f93-02ed-4928-9f6a-3b7383e7e399
ms.search.region: global
ms.search.industry: Retail
ms.author: jeffbl
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Retail July 2017 update
ms.openlocfilehash: fa7023c1ec9a77b0793ed63abfb712e7148143eb
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56248"
---
# <a name="screen-layouts-for-the-point-of-sale-pos"></a><span data-ttu-id="0924b-103">销售点 (POS) 的屏幕布局</span><span class="sxs-lookup"><span data-stu-id="0924b-103">Screen layouts for the point of sale (POS)</span></span>

[!include [banner](includes/banner.md)]

<span data-ttu-id="0924b-104">此主题提供有关 Microsoft Dynamics 365 for Retail 销售点 (POS) 体验的屏幕布局的信息。</span><span class="sxs-lookup"><span data-stu-id="0924b-104">This topic provides information about screen layouts for Microsoft Dynamics 365 for Retail point of sale (POS) experiences.</span></span>

<span data-ttu-id="0924b-105">可使用为商店、收银机和/或用户分配的视觉配置文件和屏幕布局，配置 Retail POS 用户界面 (UI)。</span><span class="sxs-lookup"><span data-stu-id="0924b-105">The Retail POS user interface (UI) can be configured by using a combination of visual profiles and screen layouts that are assigned to stores, registers, and/or users.</span></span>

<span data-ttu-id="0924b-106">下图显示构成 POS UI 可配置项的各实体之间的关系。</span><span class="sxs-lookup"><span data-stu-id="0924b-106">The following illustration shows the relationships among the various entities that make up the configurable aspects of the POS UI.</span></span>

![POS 屏幕布局实体](../retail/media/POS-layout-configuration-entities-diagram.png)

## <a name="visual-profile"></a><span data-ttu-id="0924b-108">可视化配置文件</span><span class="sxs-lookup"><span data-stu-id="0924b-108">Visual profile</span></span>
<span data-ttu-id="0924b-109">视觉配置文件分配给收银机，用于指定收银机特定且在用户中共享的视觉元素。</span><span class="sxs-lookup"><span data-stu-id="0924b-109">Visual profiles are assigned to registers, and they specify the visual elements that are register-specific and shared across users.</span></span> <span data-ttu-id="0924b-110">每位登录收银机的用户都将看到相同的主题、颜色和图像。</span><span class="sxs-lookup"><span data-stu-id="0924b-110">Every user who signs in to the register sees the same theme, colors, and images.</span></span>

![采用浅色主题的 POS 欢迎使用屏幕](../retail/media/POS-Welcome-Screen-with-Light-theme.png)

![采用深色主题的 POS 交易记录屏幕](../retail/media/POS-Transaction-Screen-with-Dark-theme.png)

- <span data-ttu-id="0924b-113">**配置文件编号** – 配置文件编号是可视化配置文件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0924b-113">**Profile number** – The profile number is the unique identifier of the visual profile.</span></span>
- <span data-ttu-id="0924b-114">**描述** - 您可以指定有意义的名称，帮助确定适合您的情况的配置文件。</span><span class="sxs-lookup"><span data-stu-id="0924b-114">**Description** – You can specify a meaningful name that will help identify the correct profile for your situation.</span></span>
- <span data-ttu-id="0924b-115">**主题** – 您可以在“浅色”和“深色”两种应用程序主题之间选择。</span><span class="sxs-lookup"><span data-stu-id="0924b-115">**Theme** – You can select between the Light and Dark application themes.</span></span> <span data-ttu-id="0924b-116">主题影响整个应用程序中的字体和背景色。</span><span class="sxs-lookup"><span data-stu-id="0924b-116">The theme affects the font and background colors throughout the application.</span></span>
- <span data-ttu-id="0924b-117">**个性色** – 个性色在整个 POS 中用于区分或突出显示特定视觉元素，如标题、命令按钮和超链接。</span><span class="sxs-lookup"><span data-stu-id="0924b-117">**Accent color** – The accent color is used throughout the POS to differentiate or highlight specific visual elements, such as tiles, command buttons, and hyperlinks.</span></span> <span data-ttu-id="0924b-118">这些元素通常可操作。</span><span class="sxs-lookup"><span data-stu-id="0924b-118">Typically, these elements are actionable.</span></span>
- <span data-ttu-id="0924b-119">**标题颜色** – 您可以配置页标题的颜色，以便满足零售商的品牌需要。</span><span class="sxs-lookup"><span data-stu-id="0924b-119">**Header color** – You can configure the color of the page header to meet the retailer's branding requirements.</span></span> <span data-ttu-id="0924b-120">只有 Microsoft Dynamics 365 for Retail 版本 1611 中才有此功能。</span><span class="sxs-lookup"><span data-stu-id="0924b-120">This feature is available only in Microsoft Dynamics 365 for Retail version 1611.</span></span>
- <span data-ttu-id="0924b-121">**登录背景** – 您可以为登录屏幕指定背景图像。</span><span class="sxs-lookup"><span data-stu-id="0924b-121">**Login backgrounds** – You can specify a background image for the sign-in screen.</span></span> <span data-ttu-id="0924b-122">背景图像的文件大小应尽量小，因为存储和加载大型文件可能影响应用程序的行为和性能。</span><span class="sxs-lookup"><span data-stu-id="0924b-122">The file size of background images should be kept as small as possible, because storing and loading large files can affect application behavior and performance.</span></span>
- <span data-ttu-id="0924b-123">**应用程序背景** – 您可以指定整个应用程序中使用的背景图像来代替纯色主题色。</span><span class="sxs-lookup"><span data-stu-id="0924b-123">**Application background** – You can specify a background image that is used instead of the solid theme color throughout the application.</span></span> <span data-ttu-id="0924b-124">至于登录背景，文件大小应该尽量小。</span><span class="sxs-lookup"><span data-stu-id="0924b-124">As for login backgrounds, the file size should be kept as small as possible.</span></span>

## <a name="screen-layouts"></a><span data-ttu-id="0924b-125">屏幕布局</span><span class="sxs-lookup"><span data-stu-id="0924b-125">Screen layouts</span></span>
<span data-ttu-id="0924b-126">屏幕布局配置决定 POS 欢迎屏幕和**交易记录**屏幕中的 UI 控件的操作、内容和位置。</span><span class="sxs-lookup"><span data-stu-id="0924b-126">Screen layout configurations determine the actions, content, and placement of UI controls on the POS welcome screen and **Transaction** screen.</span></span>

![POS 屏幕布局视图](../retail/media/POS-Screen-Layout-View.png)

- <span data-ttu-id="0924b-128">**欢迎屏幕** – 在大多数情况下，欢迎屏幕是用户首次登录 POS 时看到的页面。</span><span class="sxs-lookup"><span data-stu-id="0924b-128">**Welcome screen** – In most cases, the welcome screen is the page that users see when they first sign in to the POS.</span></span> <span data-ttu-id="0924b-129">欢迎屏幕中可以包含品牌图像和用于访问 POS 操作的按钮网格。</span><span class="sxs-lookup"><span data-stu-id="0924b-129">The welcome screen can consist of a branding image and button grids that provide access to POS operations.</span></span> <span data-ttu-id="0924b-130">此屏幕通常放置不特定于当前交易记录的操作。</span><span class="sxs-lookup"><span data-stu-id="0924b-130">Typically, operations that aren't specific to the current transaction are put on this screen.</span></span>

    ![POS 欢迎屏幕](../retail/media/POS-Welcome-Screen.png)

- <span data-ttu-id="0924b-132">**交易记录屏幕** – **交易记录**屏幕是 POS 中用于处理销售交易记录和订单的主屏幕。</span><span class="sxs-lookup"><span data-stu-id="0924b-132">**Transaction screen** – The **Transaction** screen is the main screen in the POS for processing sales transactions and orders.</span></span> <span data-ttu-id="0924b-133">内容和布局使用屏幕布局设计器配置。</span><span class="sxs-lookup"><span data-stu-id="0924b-133">The content and layout are configured by using the screen layout designer.</span></span>

    ![POS 交易记录屏幕](../retail/media/POS-Transaction-Screen.png)

- <span data-ttu-id="0924b-135">**默认开始屏幕** – 有些零售商倾向于收银员在登录后直接进入**交易记录**屏幕。</span><span class="sxs-lookup"><span data-stu-id="0924b-135">**Default start screen** – Some retailers prefer that cashiers go directly to the **Transaction** screen after sign-in.</span></span> <span data-ttu-id="0924b-136">**默认启动屏幕**设置用于指定登录后每个屏幕布局显示的默认屏幕。</span><span class="sxs-lookup"><span data-stu-id="0924b-136">The **Default start screen** setting lets you specify the default screen that appears after sign-in for each screen layout.</span></span>

### <a name="assignment"></a><span data-ttu-id="0924b-137">赋值</span><span class="sxs-lookup"><span data-stu-id="0924b-137">Assignment</span></span>

<span data-ttu-id="0924b-138">可在商店、收银机或用户级别分配屏幕布局。</span><span class="sxs-lookup"><span data-stu-id="0924b-138">Screen layouts can be assigned at the store, register, or user level.</span></span> <span data-ttu-id="0924b-139">用户的分配将覆盖收银机和商店的分配，而收银机分配则覆盖商店分配。</span><span class="sxs-lookup"><span data-stu-id="0924b-139">The user assignment overrides the register and store assignments, and the register assignment overrides the store assignment.</span></span> <span data-ttu-id="0924b-140">在简单方案中（即无论任何收银机或角色，所有用户都使用相同布局），只能在商店级别设计屏幕布局。</span><span class="sxs-lookup"><span data-stu-id="0924b-140">In a simple scenario where all users use the same layout, regardless of register or role, the screen layout can be set only at the store level.</span></span> <span data-ttu-id="0924b-141">如果特定收银机或用户需要定制布局，可以为其分配这些布局。</span><span class="sxs-lookup"><span data-stu-id="0924b-141">In scenarios where specific registers or users require specialized layouts, those layouts can be assigned.</span></span>

### <a name="layout-sizes"></a><span data-ttu-id="0924b-142">布局大小</span><span class="sxs-lookup"><span data-stu-id="0924b-142">Layout sizes</span></span>

<span data-ttu-id="0924b-143">大多数 POS UI 可响应，而布局则会根据屏幕尺寸和方向自动调整大小和方向。</span><span class="sxs-lookup"><span data-stu-id="0924b-143">Most aspects of the POS UI are responsive, and the layout is automatically resized and adjusted based on the screen size and orientation.</span></span> <span data-ttu-id="0924b-144">但是，必须为 POS **交易记录**屏幕配置预期将使用的每种屏幕分辨率。</span><span class="sxs-lookup"><span data-stu-id="0924b-144">However, the POS **Transaction** screen must be configured for every screen resolution that is expected.</span></span>

<span data-ttu-id="0924b-145">启动时，POS 应用程序将自动选择为设备配置的最接近的布局尺寸。</span><span class="sxs-lookup"><span data-stu-id="0924b-145">At startup, the POS application automatically selects the closest layout size that is configured for the device.</span></span> <span data-ttu-id="0924b-146">屏幕布局中也可以包含横向和纵向模式的配置，以及全尺寸设备和精简型设备的配置。</span><span class="sxs-lookup"><span data-stu-id="0924b-146">A screen layout can also contain configurations for both landscape and portrait modes, and for both full-size and compact devices.</span></span> <span data-ttu-id="0924b-147">因此，可以为用户分配一个屏幕布局，而该屏幕布局支持商店内的多种尺寸和外形。</span><span class="sxs-lookup"><span data-stu-id="0924b-147">Therefore, users can be assigned to a single screen layout that works across various sizes and form factors that are used in the store.</span></span>

![POS 布局尺寸](../retail/media/POS-Screen-Layout-Sizes.png)

- <span data-ttu-id="0924b-149">**名称** – 您可以输入有意义的名称来标识屏幕大小。</span><span class="sxs-lookup"><span data-stu-id="0924b-149">**Name** – You can enter a meaningful name to identify the screen size.</span></span>
- <span data-ttu-id="0924b-150">**布局类型** – POS 应用程序可以以各种模式显示其 UI，以便在给定设备上提供最佳用户体验。</span><span class="sxs-lookup"><span data-stu-id="0924b-150">**Layout type** – The POS application can show its UI in various modes to provide the best user experience on a given device.</span></span>

    - <span data-ttu-id="0924b-151">**现代 POS – 完整型** – 完整型布局通常最适合较大显示器，如台式机显示器或平板电脑。</span><span class="sxs-lookup"><span data-stu-id="0924b-151">**Modern POS – Full** – Full layouts are typically best for larger displays, such as desktop monitors and tablets.</span></span> <span data-ttu-id="0924b-152">您可以可以选择要包含的 UI 元素，指定这些元素的尺寸和位置，并配置它们的详细属性。</span><span class="sxs-lookup"><span data-stu-id="0924b-152">You can select the UI elements to include, specify the size and placement of those elements, and configure their detailed properties.</span></span> <span data-ttu-id="0924b-153">完整型布局同时支持垂直配置和水平配置。</span><span class="sxs-lookup"><span data-stu-id="0924b-153">Full layouts support both portrait and landscape configurations.</span></span>
    - <span data-ttu-id="0924b-154">**现代 POS – 紧凑型** – 紧凑型布局通常最适合手机和小平板电脑。</span><span class="sxs-lookup"><span data-stu-id="0924b-154">**Modern POS – Compact** – Compact layouts are typically best for phones and small tablets.</span></span> <span data-ttu-id="0924b-155">对于紧凑型设备，设计功能受到限制。</span><span class="sxs-lookup"><span data-stu-id="0924b-155">The design possibilities for compact devices are limited.</span></span> <span data-ttu-id="0924b-156">您可以为收据和总计窗格配置列和字段。</span><span class="sxs-lookup"><span data-stu-id="0924b-156">You can configure the columns and fields for the receipt and totals panels.</span></span>

- <span data-ttu-id="0924b-157">**宽度/高度** –这些值以像素为单位表示布局应采用的有效屏幕尺寸。</span><span class="sxs-lookup"><span data-stu-id="0924b-157">**Width/Height** – These values represent the effective screen size, in pixels, that is expected for the layout.</span></span> <span data-ttu-id="0924b-158">请注意，某些操作系统对高分辨率显示器使用缩放功能。</span><span class="sxs-lookup"><span data-stu-id="0924b-158">Remember that some operating systems use scaling for high-resolution displays.</span></span>

> [!TIP]
> <span data-ttu-id="0924b-159">可以通过在应用程序中查看分辨率了解 POS 需要的布局尺寸。</span><span class="sxs-lookup"><span data-stu-id="0924b-159">You can learn the layout size that is required for a POS screen by viewing the resolution in the app.</span></span> <span data-ttu-id="0924b-160">启动 POS，然后转至**设置 \> 会话信息**。</span><span class="sxs-lookup"><span data-stu-id="0924b-160">Start the POS, and go to **Settings \> Session information**.</span></span> <span data-ttu-id="0924b-161">POS 显示当前加载的屏幕布局，布局尺寸和应用程序窗口的分辨率。</span><span class="sxs-lookup"><span data-stu-id="0924b-161">POS shows the screen layout that is currently loaded, the layout size, and the resolution of the app window.</span></span>

![POS 布局尺寸](../retail/media/POS-Session-Information.png)

### <a name="button-grids"></a><span data-ttu-id="0924b-163">按钮网格</span><span class="sxs-lookup"><span data-stu-id="0924b-163">Button grids</span></span>
<span data-ttu-id="0924b-164">对于屏幕布局的各布局尺寸，可以为 POS 欢迎屏幕和**交易记录**屏幕配置和分配按钮网格。</span><span class="sxs-lookup"><span data-stu-id="0924b-164">For each layout size in a screen layout, you can configure and assign button grids for the POS welcome screen and **Transaction** screen.</span></span> <span data-ttu-id="0924b-165">欢迎屏幕的按钮网格自动从左到右，从最小编号（欢迎屏幕 1）到最大编号分布。</span><span class="sxs-lookup"><span data-stu-id="0924b-165">Button grids for the welcome screen are automatically laid out from left to right, from the lowest number (Welcome screen 1) to the highest number.</span></span>

<span data-ttu-id="0924b-166">在完整型 POS 布局中，按钮网格的放置在屏幕布局设计器中指定。</span><span class="sxs-lookup"><span data-stu-id="0924b-166">In Full POS layouts, the placement of button grids is specified in the screen layout designer.</span></span>

<span data-ttu-id="0924b-167">在精简型 POS 布局中，按钮网格自动从上到下，从最小编号（“交易记录”屏幕 1）到最大编号分布。</span><span class="sxs-lookup"><span data-stu-id="0924b-167">In Compact POS layouts, the button grids are automatically laid out from top to bottom, from the lowest number (Transaction screen 1) to the highest number.</span></span> <span data-ttu-id="0924b-168">可以在**操作**菜单中访问这些按钮网格。</span><span class="sxs-lookup"><span data-stu-id="0924b-168">They can be accessed on the **Actions** menu.</span></span>

![精简型布局按钮网格](../retail/media/Compact-View-Button-Grids.png)

### <a name="images"></a><span data-ttu-id="0924b-170">图像</span><span class="sxs-lookup"><span data-stu-id="0924b-170">Images</span></span>
<span data-ttu-id="0924b-171">对于屏幕布局中的每种布局尺寸，您可以指定 POS UI 中要包含的图像。</span><span class="sxs-lookup"><span data-stu-id="0924b-171">For each layout size in a screen layout, you can specify images to include in the POS UI.</span></span> <span data-ttu-id="0924b-172">对于完整型 POS 布局，只能为欢迎屏幕指定一个图像。</span><span class="sxs-lookup"><span data-stu-id="0924b-172">For Full POS layouts, a single image can be specified for the welcome screen.</span></span> <span data-ttu-id="0924b-173">此图像显示为左侧的第一个 UI 元素。</span><span class="sxs-lookup"><span data-stu-id="0924b-173">This image appears as the first UI element on the left.</span></span> <span data-ttu-id="0924b-174">在**交易记录**屏幕上，可以将图像用作标签图像或徽标。</span><span class="sxs-lookup"><span data-stu-id="0924b-174">On the **Transaction** screen, images can be used as tab images or as a logo.</span></span> <span data-ttu-id="0924b-175">精简型 POS 布局不使用这些图像。</span><span class="sxs-lookup"><span data-stu-id="0924b-175">Compact POS layouts don't use these images.</span></span>

### <a name="screen-layout-designer"></a><span data-ttu-id="0924b-176">屏幕布局设计器</span><span class="sxs-lookup"><span data-stu-id="0924b-176">Screen layout designer</span></span>

<span data-ttu-id="0924b-177">可使用屏幕布局设计器为纵向和横向模式下的各布局尺寸配置 POS **交易记录**屏幕的各设置，也可以同时为完整型和精简型布局配置。</span><span class="sxs-lookup"><span data-stu-id="0924b-177">The screen layout designer lets you configure various aspects of the POS **Transaction** screen for each layout size, in both portrait and landscape modes, and for both Full and Compact layouts.</span></span> <span data-ttu-id="0924b-178">只要用户访问应用程序，屏幕布局设计器都将使用 ClickOnce 部署技术下载、安装和启动应用程序的最新版本。</span><span class="sxs-lookup"><span data-stu-id="0924b-178">The screen layout designer uses the ClickOnce deployment technology to download, install, and start the latest version of the application every time that users access it.</span></span> <span data-ttu-id="0924b-179">请确保检查 ClickOnce 的浏览器要求。</span><span class="sxs-lookup"><span data-stu-id="0924b-179">Be sure to check the browser requirements for ClickOnce.</span></span> <span data-ttu-id="0924b-180">某些浏览器（如 Google Chrome）需要扩展。</span><span class="sxs-lookup"><span data-stu-id="0924b-180">Some browsers, such as Google Chrome, require extensions.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="0924b-181">必须为定义供 POS 使用的每个布局尺寸配置一个屏幕布局。</span><span class="sxs-lookup"><span data-stu-id="0924b-181">You must configure a screen layout for each layout size that is defined and that is used by the POS.</span></span>

### <a name="full-layout-designer"></a><span data-ttu-id="0924b-182">完整型布局设计器</span><span class="sxs-lookup"><span data-stu-id="0924b-182">Full layout designer</span></span>

<span data-ttu-id="0924b-183">用户可使用完整型布局设计器将 UI 控件拖到 POS **交易记录**屏幕上和配置这些控件的设置。</span><span class="sxs-lookup"><span data-stu-id="0924b-183">The Full layout designer lets users drag UI controls onto the POS **Transaction** screen and configure the settings of those controls.</span></span>

![POS 完整型布局设计器（横向）](../retail/media/POS-Full-Layout-Designer-Landscape.png)

- <span data-ttu-id="0924b-185">**导入布局/导出布局** – 可将将 POS 屏幕布局设计作为 XML 文件导出和导入，以便轻松重复使用和在环境之间共享。</span><span class="sxs-lookup"><span data-stu-id="0924b-185">**Import layout/Export layout** – You can export and import POS screen layout designs as XML files, so that you can easily reuse and share them across environments.</span></span> <span data-ttu-id="0924b-186">请务必导入正确布局尺寸的布局设计。</span><span class="sxs-lookup"><span data-stu-id="0924b-186">It's important that you import layout designs for the correct layout sizes.</span></span> <span data-ttu-id="0924b-187">否则，UI 元素可能不能正确适应屏幕。</span><span class="sxs-lookup"><span data-stu-id="0924b-187">Otherwise, UI elements might not fit correctly on the screen.</span></span>
- <span data-ttu-id="0924b-188">**横向/纵向** – 如果 POS 设备允许用户在横向和纵向模式之间切换，则您必须为各模式定义屏幕布局。</span><span class="sxs-lookup"><span data-stu-id="0924b-188">**Landscape/Portrait** – If the POS device lets users switch between landscape and portrait modes, you must define a screen layout for each mode.</span></span> <span data-ttu-id="0924b-189">POS 将自动检测屏幕旋转方向并显示正确的布局。</span><span class="sxs-lookup"><span data-stu-id="0924b-189">The POS automatically detects screen rotation and shows the correct layout.</span></span>
- <span data-ttu-id="0924b-190">**布局网格** – POS 布局设计器使用 4 像素网格。</span><span class="sxs-lookup"><span data-stu-id="0924b-190">**Layout grid** – The POS layout designer uses a 4-pixel grid.</span></span> <span data-ttu-id="0924b-191">UI 控件“”与网格啮合，帮助您正确对齐内容。</span><span class="sxs-lookup"><span data-stu-id="0924b-191">UI controls "snap" to the grid to help you correctly align the content.</span></span>
- <span data-ttu-id="0924b-192">**设计器缩放** – 可以缩放设计器视图，以便更好查看 POS 屏幕上的内容。</span><span class="sxs-lookup"><span data-stu-id="0924b-192">**Designer zoom** – You can zoom the designer view in and out to better view the content on the POS screen.</span></span> <span data-ttu-id="0924b-193">POS 上的屏幕分辨率与设计器中使用的屏幕分辨率差别很大时，此功能非常有用。</span><span class="sxs-lookup"><span data-stu-id="0924b-193">This feature is useful when the screen resolution on the POS differs greatly from the resolution of the screen that is used in the designer.</span></span>
- <span data-ttu-id="0924b-194">**显示/隐藏导航栏** – 对于完整型 POS 布局，您可以选择**交易记录**屏幕中是否显示左侧导航栏。</span><span class="sxs-lookup"><span data-stu-id="0924b-194">**Show/hide navigation bar** – For Full POS layouts, you can select whether the left navigation bar is visible on the **Transaction** screen.</span></span> <span data-ttu-id="0924b-195">此功能对分辨率较低的显示器很有用。</span><span class="sxs-lookup"><span data-stu-id="0924b-195">This feature is helpful for displays that have a lower resolution.</span></span> <span data-ttu-id="0924b-196">若要设置可见性，请在设计器中右键单击导航栏，然后选中或清除**始终显示**复选框。</span><span class="sxs-lookup"><span data-stu-id="0924b-196">To set the visibility, right-click the navigation bar in the designer, and select or clear the **Always visible** check box.</span></span> <span data-ttu-id="0924b-197">如果导航栏已隐藏，POS 用户仍然可以使用左上角的菜单访问。</span><span class="sxs-lookup"><span data-stu-id="0924b-197">If the navigation bar is hidden, POS users can still access it by using the menu in the upper left.</span></span>

    ![显示/隐藏导航栏](../retail/media/Navigation-Bar.PNG)

- <span data-ttu-id="0924b-199">**POS 控件** – POS 布局设计器支持以下控件。</span><span class="sxs-lookup"><span data-stu-id="0924b-199">**POS controls** – The POS layout designer supports the following controls.</span></span> <span data-ttu-id="0924b-200">可通过右键单击和使用快捷菜单配置大量控件。</span><span class="sxs-lookup"><span data-stu-id="0924b-200">You can configure many controls by right-clicking and using the shortcut menu.</span></span>

    ![POS UI 控件](../retail/media/POS-UI-Controls.png)

    - <span data-ttu-id="0924b-202">**数字键盘** - 数字键盘是 POS **交易记录**屏幕中的主要用户输入机制。</span><span class="sxs-lookup"><span data-stu-id="0924b-202">**Number pad** – The number pad is the main mechanism for user input on the POS **Transaction** screen.</span></span> <span data-ttu-id="0924b-203">您可以配置控件，以便显示完整型的数字键盘。</span><span class="sxs-lookup"><span data-stu-id="0924b-203">You can configure the control so that the full number pad is shown.</span></span> <span data-ttu-id="0924b-204">此选项是触控屏设备的理想选择。</span><span class="sxs-lookup"><span data-stu-id="0924b-204">This option is ideal for touchscreen devices.</span></span> <span data-ttu-id="0924b-205">您也可以将其配置为仅显示输入字段。</span><span class="sxs-lookup"><span data-stu-id="0924b-205">Alternatively, you can configure it so that only the input field is shown.</span></span> <span data-ttu-id="0924b-206">在这种情况下，使用物理键盘进行输入。</span><span class="sxs-lookup"><span data-stu-id="0924b-206">In this case, a physical keyboard is used for input.</span></span> <span data-ttu-id="0924b-207">只有完整型布局中才有数字键盘设置。</span><span class="sxs-lookup"><span data-stu-id="0924b-207">The number pad settings are available only for Full layouts.</span></span> <span data-ttu-id="0924b-208">对于精简型布局，**交易记录**屏幕上始终显示完整型的数字键盘。</span><span class="sxs-lookup"><span data-stu-id="0924b-208">For Compact layouts, the full number pad is always shown on the **Transaction** screen.</span></span>
    - <span data-ttu-id="0924b-209">**总计面板** - 您可以将总计面板配置为一列或两列，以显示值，如行计数、折扣金额、费用、小计和税。</span><span class="sxs-lookup"><span data-stu-id="0924b-209">**Totals panel** – You can configure the totals panel in either one column or two columns, to show values such as the line count, discount amount, charges, subtotal, and tax.</span></span> <span data-ttu-id="0924b-210">精简型布局仅支持一列。</span><span class="sxs-lookup"><span data-stu-id="0924b-210">Compact layouts support only a single column.</span></span>
    - <span data-ttu-id="0924b-211">**收据面板** – 收据面板中包含 POS 中处理的产品和服务的销售行、付款行和交货信息。</span><span class="sxs-lookup"><span data-stu-id="0924b-211">**Receipt panel** – The receipt panel contains the sales lines, payment lines, and delivery information for the products and services that are processed in the POS.</span></span> <span data-ttu-id="0924b-212">您可以指定列、宽度和位置。</span><span class="sxs-lookup"><span data-stu-id="0924b-212">You can specify columns, widths, and placement.</span></span> <span data-ttu-id="0924b-213">在精简型布局中，也可以配置在主行下的行中显示的更多信息。</span><span class="sxs-lookup"><span data-stu-id="0924b-213">In Compact layouts, you can also configure additional information that appears in the row under the main line.</span></span>
    - <span data-ttu-id="0924b-214">**客户卡** – 客户卡显示有关与当前交易关联的客户的信息。</span><span class="sxs-lookup"><span data-stu-id="0924b-214">**Customer card** – The customer card shows information about the customer who is associated with the current transaction.</span></span> <span data-ttu-id="0924b-215">您可以将客户卡配置为隐藏或显示更多信息。</span><span class="sxs-lookup"><span data-stu-id="0924b-215">You can configure the customer card to hide or show additional information.</span></span>
    - <span data-ttu-id="0924b-216">**选项卡控件** – 您可以向屏幕布局添加选项卡控件，然后在其中放置其他控件（如数字键盘、客户卡或按钮窗格）。</span><span class="sxs-lookup"><span data-stu-id="0924b-216">**Tab control** – You can add the tab control to a screen layout, and then put other controls, such as the number pad, customer card, or button grids, in it.</span></span> <span data-ttu-id="0924b-217">选项卡控件是帮助您在屏幕中放置更多内容的容器。</span><span class="sxs-lookup"><span data-stu-id="0924b-217">The tab control is a container that helps you fit more content on the screen.</span></span> <span data-ttu-id="0924b-218">选项卡控件仅可用于完整型布局。</span><span class="sxs-lookup"><span data-stu-id="0924b-218">The tab control is available only for Full layouts.</span></span>
    - <span data-ttu-id="0924b-219">**图像** -您可以使用 图像控件在**交易记录**屏幕中显示商店徽标或其他品牌图像。</span><span class="sxs-lookup"><span data-stu-id="0924b-219">**Image** – You can use the image control to show the store's logo or another branding image on the **Transaction** screen.</span></span> <span data-ttu-id="0924b-220">图像控件仅可用于完整型布局。</span><span class="sxs-lookup"><span data-stu-id="0924b-220">The image control is available only for Full layouts.</span></span>
    - <span data-ttu-id="0924b-221">**推荐产品** – 如果为环境配置了推荐产品控件，则将根据机器学习显示产品建议。</span><span class="sxs-lookup"><span data-stu-id="0924b-221">**Recommended products** – If the recommended products control is configured for the environment, it shows product suggestions, based on machine learning.</span></span>
    - <span data-ttu-id="0924b-222">**自定义控件** – 自定义控件充当屏幕布局内的占位符，用于为自定义内容预留空间。</span><span class="sxs-lookup"><span data-stu-id="0924b-222">**Custom control** – The custom control acts as a placeholder in the screen layout and lets you reserve space for custom content.</span></span> <span data-ttu-id="0924b-223">自定义控件仅可用于完整型布局。</span><span class="sxs-lookup"><span data-stu-id="0924b-223">The custom control is available only for Full layouts.</span></span>

### <a name="compact-layout-designer"></a><span data-ttu-id="0924b-224">精简型布局设计器</span><span class="sxs-lookup"><span data-stu-id="0924b-224">Compact layout designer</span></span>
<span data-ttu-id="0924b-225">和完整型布局设计器一样，精简型布局设计器可用于针对手机和小型平板电脑配置 POS 屏幕布局。</span><span class="sxs-lookup"><span data-stu-id="0924b-225">Like the Full layout designer, the Compact layout designer lets you configure the POS screen layout for phones and small tablets.</span></span> <span data-ttu-id="0924b-226">但是，在这种情况下，布局本身是固定的。</span><span class="sxs-lookup"><span data-stu-id="0924b-226">However, in this case, the layout itself is fixed.</span></span> <span data-ttu-id="0924b-227">可通过右键单击和使用快捷菜单在布局中配置控件。</span><span class="sxs-lookup"><span data-stu-id="0924b-227">You can configure the controls in the layout by right-clicking and using the shortcut menu.</span></span> <span data-ttu-id="0924b-228">但是，您不能为其他内容使用拖放操作。</span><span class="sxs-lookup"><span data-stu-id="0924b-228">However, you can't use drag-and-drop operations for additional content.</span></span>

![精简型布局设计器](../retail/media/Compact-Layout-Designer.png)

### <a name="button-grid-designer"></a><span data-ttu-id="0924b-230">按钮网格设计器</span><span class="sxs-lookup"><span data-stu-id="0924b-230">Button grid designer</span></span>
<span data-ttu-id="0924b-231">可通过按钮网格设计器为完整型布局和精简型布局配置 POS 欢迎屏幕和**交易记录**屏幕上可使用的按钮网格。</span><span class="sxs-lookup"><span data-stu-id="0924b-231">The button grid designer lets you configure button grids that can be used on the POS welcome screen and **Transaction** screen for both Full and Compact layouts.</span></span> <span data-ttu-id="0924b-232">可跨布局和布局类型使用同一个按钮网格。</span><span class="sxs-lookup"><span data-stu-id="0924b-232">The same button grid can be used across layouts and layout types.</span></span> <span data-ttu-id="0924b-233">和屏幕布局设计器一样，只要用户访问应用程序，按钮网格设计器都将使用 ClickOnce 部署技术下载、安装和启动应用程序的最新版本。</span><span class="sxs-lookup"><span data-stu-id="0924b-233">Like the screen layout designer, the button grid designer uses the ClickOnce deployment technology to download, install, and start the latest version of the application every time that users access it.</span></span> <span data-ttu-id="0924b-234">请确保检查 ClickOnce 的浏览器要求。</span><span class="sxs-lookup"><span data-stu-id="0924b-234">Be sure to check the browser requirements for ClickOnce.</span></span> <span data-ttu-id="0924b-235">某些浏览器（如 Google Chrome）需要扩展。</span><span class="sxs-lookup"><span data-stu-id="0924b-235">Some browsers, such as Google Chrome, require extensions.</span></span>

![按钮网格设计器](../retail/media/Button-Grid-Designer.png)

- <span data-ttu-id="0924b-237">**新按钮** – 单击以向按钮网格添加新按钮。</span><span class="sxs-lookup"><span data-stu-id="0924b-237">**New button** – Click to add a new button to the button grid.</span></span> <span data-ttu-id="0924b-238">默认情况下，新按钮在网格左上角显示。</span><span class="sxs-lookup"><span data-stu-id="0924b-238">By default, new buttons appear in the upper-left corner of the grid.</span></span> <span data-ttu-id="0924b-239">但是，您可以通过在布局中拖放来重新安排按钮。</span><span class="sxs-lookup"><span data-stu-id="0924b-239">However, you can arrange buttons by dragging them in the layout.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="0924b-240">按钮网格的内容可能重叠。</span><span class="sxs-lookup"><span data-stu-id="0924b-240">The contents of the button grid can overlap.</span></span> <span data-ttu-id="0924b-241">安排按钮时，请确保按钮不会彼此遮挡。</span><span class="sxs-lookup"><span data-stu-id="0924b-241">When you arrange buttons, make sure that they don't hide other buttons.</span></span>

- <span data-ttu-id="0924b-242">**新设计** – 单击以通过指定每行和每列的按钮数来自动设置按钮网格布局。</span><span class="sxs-lookup"><span data-stu-id="0924b-242">**New design** – Click to automatically set up a button grid layout by specifying the number of buttons per row and column.</span></span>
- <span data-ttu-id="0924b-243">**按钮属性** – 您可以通过右键单击按钮和使用快捷菜单配置按钮属性。</span><span class="sxs-lookup"><span data-stu-id="0924b-243">**Button properties** – You can configure button properties by right-clicking the button and using the shortcut menu.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="0924b-244">某些按钮网格设置仅适用于 Enterprise POS，不适用于 Retail Modern POS 或 Cloud POS。</span><span class="sxs-lookup"><span data-stu-id="0924b-244">Some button grid settings apply only to Enterprise POS, not to Retail Modern POS or Cloud POS.</span></span>

    ![按钮网格按钮属性](../retail/media/Button-grid-button-properties.png)

    - <span data-ttu-id="0924b-246">**操作** – 在适用 POS 操作列表中，选择在 POS 中单击按钮时调用的操作。</span><span class="sxs-lookup"><span data-stu-id="0924b-246">**Action** – In the list of applicable POS operations, select the operation that is invoked when the button is clicked in the POS.</span></span>

        <span data-ttu-id="0924b-247">有关支持的 POS 操作的列表，请参阅 [POS 操作、联机和脱机](pos-operations.md)。</span><span class="sxs-lookup"><span data-stu-id="0924b-247">For the list of supported POS operations, see [POS operations, online and offline](pos-operations.md).</span></span>

    - <span data-ttu-id="0924b-248">**操作参数** – 某些 POS 操作在调用时使用更多参数。</span><span class="sxs-lookup"><span data-stu-id="0924b-248">**Action parameters** – Some POS operations use additional parameters when they are invoked.</span></span> <span data-ttu-id="0924b-249">例如，对于“添加产品”操作，用户可以指定要添加的产品。</span><span class="sxs-lookup"><span data-stu-id="0924b-249">For example, for the Add product operation, users can specify the product to add.</span></span>
    - <span data-ttu-id="0924b-250">**按钮稳步** – 指定 POS 中的按钮上显示的文本。</span><span class="sxs-lookup"><span data-stu-id="0924b-250">**Button text** – Specify the text that appears on the button in the POS.</span></span>
    - <span data-ttu-id="0924b-251">**隐藏按钮文本** – 此复选框用于隐藏或显示按钮文本。</span><span class="sxs-lookup"><span data-stu-id="0924b-251">**Hide button text** – Use this check box to hide or show the button text.</span></span> <span data-ttu-id="0924b-252">仅显示一个按钮的小型按钮通常会显示按钮文本。</span><span class="sxs-lookup"><span data-stu-id="0924b-252">Button text is often hidden for small buttons that show only an icon.</span></span>
    - <span data-ttu-id="0924b-253">**工具提示** – 指定用户将鼠标光标悬停在按钮上方时显示的更多帮助文本。</span><span class="sxs-lookup"><span data-stu-id="0924b-253">**Tooltip** – Specify additional Help text that appears when users mouse over the button.</span></span>
    - <span data-ttu-id="0924b-254">**以列为单位的大小/以行为单位的大小** – 您可以指定按钮的高度和宽度。</span><span class="sxs-lookup"><span data-stu-id="0924b-254">**Size in columns/Size in rows** – You can specify how tall and wide the button is.</span></span>

        ![以行和列为单位的 POS 按钮大小](../retail/media/POS-Button-Sizes-In-Rows-And-Columns.png)

    - <span data-ttu-id="0924b-256">**自定义字体** – 如果选中**启用 POS 的自定义字体**复选框，则可为 POS 指定非系统默认字体。</span><span class="sxs-lookup"><span data-stu-id="0924b-256">**Custom font** – When you select the **Enable custom font for POS** check box, you can specify a font other than the default system font for the POS.</span></span>
    - <span data-ttu-id="0924b-257">**自定义主题** – 默认情况下，POS 按钮使用可视化配置文件中的主题颜色。</span><span class="sxs-lookup"><span data-stu-id="0924b-257">**Custom theme** – By default, POS buttons use the accent color from the visual profile.</span></span> <span data-ttu-id="0924b-258">如果选中**使用自定义主题**复选框，则可指定更多颜色。</span><span class="sxs-lookup"><span data-stu-id="0924b-258">When you select the **Use custom theme** check box, you can specify additional colors.</span></span>

        > [!NOTE]
        > <span data-ttu-id="0924b-259">Retail Modern POS 和 Cloud POS 仅适用于**背景色**和**字体颜色**值。</span><span class="sxs-lookup"><span data-stu-id="0924b-259">Retail Modern POS and Cloud POS use only the **Back color** and **Font color** values.</span></span>

    - <span data-ttu-id="0924b-260">–**按钮图像** – 按钮中可以包含图像或图标。</span><span class="sxs-lookup"><span data-stu-id="0924b-260">**Button image** – Buttons can include images or icons.</span></span> <span data-ttu-id="0924b-261">可以在**零售 \> 渠道设置 \> POS 设置 \> POS \> 图像**中指定的可用图像内进行选择。</span><span class="sxs-lookup"><span data-stu-id="0924b-261">Select among the available images that are specified at **Retail \> Channel setup \> POS setup \> POS \> Images**.</span></span>

![POS 中的示例按钮网格](../retail/media/Example-Button-Grid-In-POS.png)

## <a name="additional-resources"></a><span data-ttu-id="0924b-263">其他资源</span><span class="sxs-lookup"><span data-stu-id="0924b-263">Additional resources</span></span>

[<span data-ttu-id="0924b-264">安装 Retail POS 布局设计器</span><span class="sxs-lookup"><span data-stu-id="0924b-264">Install the Retail POS Layout designer</span></span>](install-pos-layout-designer.md)