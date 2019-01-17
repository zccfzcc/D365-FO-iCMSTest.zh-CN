---
title: 配置工作人员
description: 此过程演示如何将零售工作人员配置为有资格享受 POS 中的销售佣金的销售代表。
author: jblucher
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CommissionSalesGroup, CommissionSalesMember, DirPartyLookup, HcmWorker
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Retail
ms.author: jeffbl
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: c3c70a3980addab82744351e819aaba69a3792c0
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54233"
---
# <a name="configure-a-worker"></a><span data-ttu-id="03cc2-103">配置工作人员</span><span class="sxs-lookup"><span data-stu-id="03cc2-103">Configure a worker</span></span>

[!include[task guide banner](../includes/task-guide-banner.md)]

<span data-ttu-id="03cc2-104">此过程演示如何将零售工作人员配置为有资格享受 POS 中的销售佣金的销售代表。</span><span class="sxs-lookup"><span data-stu-id="03cc2-104">This procedure demonstrates how to configure a retail worker as a sales representative who is eligible for commission on sales in POS.</span></span> <span data-ttu-id="03cc2-105">此程序使用 USRT 演示数据公司。</span><span class="sxs-lookup"><span data-stu-id="03cc2-105">This procedure uses the USRT demo data company.</span></span>


## <a name="create-a-commission-sales-group-for-the-worker"></a><span data-ttu-id="03cc2-106">为工作人员创建佣金销售组</span><span class="sxs-lookup"><span data-stu-id="03cc2-106">Create a commission sales group for the worker</span></span>
1. <span data-ttu-id="03cc2-107">转到“销售和市场营销”>“佣金”>“销售组”。</span><span class="sxs-lookup"><span data-stu-id="03cc2-107">Go to Sales and marketing > Commissions > Sales groups.</span></span>
    * <span data-ttu-id="03cc2-108">可以将工作人员分配给一个或多个销售组。</span><span class="sxs-lookup"><span data-stu-id="03cc2-108">Workers can be assigned to one or more sales groups.</span></span> <span data-ttu-id="03cc2-109">在 POS 中，可以从商店通讯簿中选择包含工作人员的任何销售组。</span><span class="sxs-lookup"><span data-stu-id="03cc2-109">In POS, you can choose any sales group that contains workers from the store's address book.</span></span>  
2. <span data-ttu-id="03cc2-110">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="03cc2-110">Click New.</span></span>
3. <span data-ttu-id="03cc2-111">在“组”字段中，输入一个值。</span><span class="sxs-lookup"><span data-stu-id="03cc2-111">In the Group field, type a value.</span></span>
4. <span data-ttu-id="03cc2-112">在“名称”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="03cc2-112">In the Name field, type a value.</span></span>
5. <span data-ttu-id="03cc2-113">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="03cc2-113">Click Save.</span></span>
6. <span data-ttu-id="03cc2-114">在操作窗格上，单击“常规”。</span><span class="sxs-lookup"><span data-stu-id="03cc2-114">On the Action Pane, click General.</span></span>
7. <span data-ttu-id="03cc2-115">单击“销售代表”。</span><span class="sxs-lookup"><span data-stu-id="03cc2-115">Click Sales rep.</span></span>
    * <span data-ttu-id="03cc2-116">一个销售组可以包含多个工作人员。</span><span class="sxs-lookup"><span data-stu-id="03cc2-116">A sales group can contain more than one worker.</span></span> <span data-ttu-id="03cc2-117">可以根据定义的佣金份额在工作人员之间分佣金。</span><span class="sxs-lookup"><span data-stu-id="03cc2-117">Commissions can be split between workers based on how you define the commission share.</span></span>  
8. <span data-ttu-id="03cc2-118">在“名称”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="03cc2-118">In the Name field, enter or select a value.</span></span>
9. <span data-ttu-id="03cc2-119">在“佣金份额”字段中，输入一个数字。</span><span class="sxs-lookup"><span data-stu-id="03cc2-119">In the Commission share field, enter a number.</span></span>
10. <span data-ttu-id="03cc2-120">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="03cc2-120">Click Save.</span></span>
11. <span data-ttu-id="03cc2-121">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="03cc2-121">Close the page.</span></span>
12. <span data-ttu-id="03cc2-122">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="03cc2-122">Close the page.</span></span>

## <a name="assign-the-workers-default-sales-group"></a><span data-ttu-id="03cc2-123">为工作人员分配默认销售组</span><span class="sxs-lookup"><span data-stu-id="03cc2-123">Assign the workers default sales group</span></span>
1. <span data-ttu-id="03cc2-124">转至“零售和商业”>“员工”>“工作人员”。</span><span class="sxs-lookup"><span data-stu-id="03cc2-124">Go to Retail and commerce > Employees > Workers.</span></span>
2. <span data-ttu-id="03cc2-125">在列表中，找到并选择所需记录。</span><span class="sxs-lookup"><span data-stu-id="03cc2-125">In the list, find and select the desired record.</span></span>
3. <span data-ttu-id="03cc2-126">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="03cc2-126">In the list, click the link in the selected row.</span></span>
4. <span data-ttu-id="03cc2-127">单击“零售”选项卡。</span><span class="sxs-lookup"><span data-stu-id="03cc2-127">Click the Retail tab.</span></span>
    * <span data-ttu-id="03cc2-128">可以将工作人员分配给默认销售组。</span><span class="sxs-lookup"><span data-stu-id="03cc2-128">A worker can be assigned to a default sales group.</span></span> <span data-ttu-id="03cc2-129">如果商店的功能模板中启用了此选项，将把默认销售组自动添加到 POS 中的销售行。</span><span class="sxs-lookup"><span data-stu-id="03cc2-129">The default sales group will be automatically added to sales lines in POS if the option is enabled in the functionality profile for the store.</span></span>  
5. <span data-ttu-id="03cc2-130">单击“编辑”。</span><span class="sxs-lookup"><span data-stu-id="03cc2-130">Click Edit.</span></span>
6. <span data-ttu-id="03cc2-131">在“默认组”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="03cc2-131">In the Default group field, enter or select a value.</span></span>
7. <span data-ttu-id="03cc2-132">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="03cc2-132">Click Save.</span></span>

