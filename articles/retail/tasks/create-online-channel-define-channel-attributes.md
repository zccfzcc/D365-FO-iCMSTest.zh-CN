---
title: 创建在线渠道和定义渠道属性
description: 此程序会逐步演示如何创建新的在线渠道，然后将其添加到组织层次结构。
author: jashanno
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: RetailSPOnlineStoreDetailPage, SysLookupMultiSelectGrid, DimensionLookup, OMHierarchyManager, HierarchyDesigner, OMNodeSelection, HierarchyPublishAndCloseForm
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Retail
ms.author: jashanno
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 967048ef90072c3ee9aafe1fc657a6aa32550a3e
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56077"
---
# <a name="create-online-channel-and-define-channel-attributes"></a><span data-ttu-id="aae9b-103">创建在线渠道和定义渠道属性</span><span class="sxs-lookup"><span data-stu-id="aae9b-103">Create online channel and define channel attributes</span></span>

[!include[task guide banner](../includes/task-guide-banner.md)]

<span data-ttu-id="aae9b-104">此程序会逐步演示如何创建新的在线渠道，然后将其添加到组织层次结构。</span><span class="sxs-lookup"><span data-stu-id="aae9b-104">This procedure walks through creating a new online channel and adding it to the organization hierarchy.</span></span> <span data-ttu-id="aae9b-105">在创建新的在线渠道之前，您必须创建组织层次结构。</span><span class="sxs-lookup"><span data-stu-id="aae9b-105">You must create the organization hierarchy before you can create a new online channel.</span></span> <span data-ttu-id="aae9b-106">此程序使用 USRT 演示数据公司。</span><span class="sxs-lookup"><span data-stu-id="aae9b-106">This procedure uses the USRT demo data company.</span></span>


## <a name="create-a-new-online-channel"></a><span data-ttu-id="aae9b-107">创建新的在线渠道</span><span class="sxs-lookup"><span data-stu-id="aae9b-107">Create a new online channel</span></span>
1. <span data-ttu-id="aae9b-108">转至“零售和商业”>“渠道”>“在线商店”。</span><span class="sxs-lookup"><span data-stu-id="aae9b-108">Go to Retail and commerce > Channels > Online stores.</span></span>
2. <span data-ttu-id="aae9b-109">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="aae9b-109">Click New.</span></span>
3. <span data-ttu-id="aae9b-110">在“名称”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="aae9b-110">In the Name field, type a value.</span></span>
4. <span data-ttu-id="aae9b-111">在“仓库”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="aae9b-111">In the Warehouse field, enter or select a value.</span></span>
5. <span data-ttu-id="aae9b-112">在“商店时区”字段中，选择一个选项。</span><span class="sxs-lookup"><span data-stu-id="aae9b-112">In the Store time zone field, select an option.</span></span>
6. <span data-ttu-id="aae9b-113">在“默认客户”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="aae9b-113">In the Default customer field, enter or select a value.</span></span>
7. <span data-ttu-id="aae9b-114">在“客户通讯簿”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="aae9b-114">In the Customer address book field, enter or select a value.</span></span>
8. <span data-ttu-id="aae9b-115">在“付款条款”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="aae9b-115">In the Terms of payment field, enter or select a value.</span></span>
9. <span data-ttu-id="aae9b-116">在“付款方式”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="aae9b-116">In the Method of payment field, enter or select a value.</span></span>
10. <span data-ttu-id="aae9b-117">在“电子邮件通知配置文件”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="aae9b-117">In the Email notification profile field, enter or select a value.</span></span>
11. <span data-ttu-id="aae9b-118">扩展财务维度区段。</span><span class="sxs-lookup"><span data-stu-id="aae9b-118">Expand the Financial dimensions section.</span></span>
12. <span data-ttu-id="aae9b-119">在“业务单位”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="aae9b-119">In the BusinessUnit field, enter or select a value.</span></span>
    * <span data-ttu-id="aae9b-120">同样设置所有其他默认维度的值。</span><span class="sxs-lookup"><span data-stu-id="aae9b-120">Similarly set the value for all the other default dimensions.</span></span>  
13. <span data-ttu-id="aae9b-121">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="aae9b-121">Click Save.</span></span>

## <a name="add-the-online-channel-to-organization-hierarchy"></a><span data-ttu-id="aae9b-122">将在线渠道添加到组织层次结构</span><span class="sxs-lookup"><span data-stu-id="aae9b-122">Add the online channel to organization hierarchy</span></span>
1. <span data-ttu-id="aae9b-123">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="aae9b-123">Close the page.</span></span>
2. <span data-ttu-id="aae9b-124">转到“组织管理”>“组织”>“组织层次结构”。</span><span class="sxs-lookup"><span data-stu-id="aae9b-124">Go to Organization administration > Organizations > Organization hierarchies.</span></span>
3. <span data-ttu-id="aae9b-125">在列表中，找到并选择所需记录。</span><span class="sxs-lookup"><span data-stu-id="aae9b-125">In the list, find and select the desired record.</span></span>
4. <span data-ttu-id="aae9b-126">单击“查看”。</span><span class="sxs-lookup"><span data-stu-id="aae9b-126">Click View.</span></span>
5. <span data-ttu-id="aae9b-127">单击“编辑”。</span><span class="sxs-lookup"><span data-stu-id="aae9b-127">Click Edit.</span></span>
    * <span data-ttu-id="aae9b-128">您可以选择您想要在其项下插入新渠道的任何层次结构节点。</span><span class="sxs-lookup"><span data-stu-id="aae9b-128">You can select any hierarchy node under which you want to insert the new channel.</span></span>  
6. <span data-ttu-id="aae9b-129">单击“插入”。</span><span class="sxs-lookup"><span data-stu-id="aae9b-129">Click Insert.</span></span>
7. <span data-ttu-id="aae9b-130">单击“零售渠道”。</span><span class="sxs-lookup"><span data-stu-id="aae9b-130">Click Retail channel.</span></span>
8. <span data-ttu-id="aae9b-131">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="aae9b-131">Click OK.</span></span>
9. <span data-ttu-id="aae9b-132">单击“发布”以打开下拉对话框。</span><span class="sxs-lookup"><span data-stu-id="aae9b-132">Click Publish to open the drop dialog.</span></span>
10. <span data-ttu-id="aae9b-133">在“有效日期”字段中输入日期和时间。</span><span class="sxs-lookup"><span data-stu-id="aae9b-133">In the Effective date field, enter a date and time.</span></span>
11. <span data-ttu-id="aae9b-134">单击“发布”。</span><span class="sxs-lookup"><span data-stu-id="aae9b-134">Click Publish.</span></span>
