---
title: 创建借出物品
description: 借出物品是帮助您跟踪您的公司借出给工作人员的实际物品（如手机或电脑）的记录。
author: kherr75
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: HcmLoanType, DefaultDashboard, HcmLoanItem, HcmWorkerLookUp
audience: Application User
ms.reviewer: rschloma
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: kherr
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 173f77c689e45760ced7f290c8ec2fb07477180d
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55904"
---
# <a name="create-loan-items"></a><span data-ttu-id="fc31f-103">创建借出物品</span><span class="sxs-lookup"><span data-stu-id="fc31f-103">Create loan items</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="fc31f-104">借出物品是帮助您跟踪您的公司借出给工作人员的实际物品（如手机或电脑）的记录。</span><span class="sxs-lookup"><span data-stu-id="fc31f-104">Loan items are records that help you track physical items, such as phones or computers, that your company lends to workers.</span></span> <span data-ttu-id="fc31f-105">每个实际物品都必须具有相应的借出物品。</span><span class="sxs-lookup"><span data-stu-id="fc31f-105">Each physical item must have a corresponding loan item.</span></span> <span data-ttu-id="fc31f-106">每个借出物品记录都应描述所借物品，负责借出的员工和物品可以借出的天数。</span><span class="sxs-lookup"><span data-stu-id="fc31f-106">Each loan item record should describe what is being loaned, who is responsible for the loan, and the number of days the item can be on loan.</span></span> <span data-ttu-id="fc31f-107">您可以同时创建多个借出物品，例如钥匙、门卡或制服等。</span><span class="sxs-lookup"><span data-stu-id="fc31f-107">You can create multiple loan items, such as keys, access cards, or uniforms, at the same time.</span></span> <span data-ttu-id="fc31f-108">创建此程序的演示数据公司是 USMF。</span><span class="sxs-lookup"><span data-stu-id="fc31f-108">The demo data company used to create this procedure is USMF.</span></span>


## <a name="create-loan-types"></a><span data-ttu-id="fc31f-109">创建“借出类型”</span><span class="sxs-lookup"><span data-stu-id="fc31f-109">Create Loan types</span></span>
1. <span data-ttu-id="fc31f-110">转到“人力资源”>“工作人员”>“借出物品”>“借出类型”。</span><span class="sxs-lookup"><span data-stu-id="fc31f-110">Go to Human resources > Workers > Loan items > Loan types.</span></span>
2. <span data-ttu-id="fc31f-111">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="fc31f-111">Click New.</span></span>
3. <span data-ttu-id="fc31f-112">在“借出类型”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="fc31f-112">In the Loan type field, type a value.</span></span>
4. <span data-ttu-id="fc31f-113">在“描述”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="fc31f-113">In the Description field, type a value.</span></span>
5. <span data-ttu-id="fc31f-114">输入指派给此借出类型的物品可逾期返还的天数。</span><span class="sxs-lookup"><span data-stu-id="fc31f-114">Enter the number of days that items assigned to this loan type can be overdue.</span></span> 
6. <span data-ttu-id="fc31f-115">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="fc31f-115">Click Save.</span></span>
7. <span data-ttu-id="fc31f-116">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="fc31f-116">Close the page.</span></span>
8. <span data-ttu-id="fc31f-117">刷新该页面。</span><span class="sxs-lookup"><span data-stu-id="fc31f-117">Refresh the page.</span></span>

## <a name="create-loan-items"></a><span data-ttu-id="fc31f-118">创建“借出物品”</span><span class="sxs-lookup"><span data-stu-id="fc31f-118">Create Loan items</span></span>
1. <span data-ttu-id="fc31f-119">转到“人力资源”>“工作人员”>“借出物品”>“借出物品”。</span><span class="sxs-lookup"><span data-stu-id="fc31f-119">Go to Human resources > Workers > Loan items > Loan items.</span></span>
2. <span data-ttu-id="fc31f-120">单击“创建借出物品”。</span><span class="sxs-lookup"><span data-stu-id="fc31f-120">Click Create loan items.</span></span>
3. <span data-ttu-id="fc31f-121">在“数量” 字段中，输入一个数字。</span><span class="sxs-lookup"><span data-stu-id="fc31f-121">In the Qty. field, enter a number.</span></span>
4. <span data-ttu-id="fc31f-122">在“描述”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="fc31f-122">In the Description field, type a value.</span></span>
5. <span data-ttu-id="fc31f-123">在“借出类型”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="fc31f-123">In the Loan type field, click the drop-down button to open the lookup.</span></span>
6. <span data-ttu-id="fc31f-124">在列表中，找到并选择所需记录。</span><span class="sxs-lookup"><span data-stu-id="fc31f-124">In the list, find and select the desired record.</span></span>
7. <span data-ttu-id="fc31f-125">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="fc31f-125">In the list, click the link in the selected row.</span></span>
8. <span data-ttu-id="fc31f-126">输入允许物品借出的天数。</span><span class="sxs-lookup"><span data-stu-id="fc31f-126">Enter the number of days the item can be on loan.</span></span>
    * <span data-ttu-id="fc31f-127">借出设备的“预定归还日期”字段的默认值计算为当前日期加上此数字。</span><span class="sxs-lookup"><span data-stu-id="fc31f-127">The default value for the Planned return field on the Loaned equipment page is calculated as the current date plus this number.</span></span>  
9. <span data-ttu-id="fc31f-128">在“负责人”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="fc31f-128">In the Person in charge field, click the drop-down button to open the lookup.</span></span>
10. <span data-ttu-id="fc31f-129">单击“选择”。</span><span class="sxs-lookup"><span data-stu-id="fc31f-129">Click Select.</span></span>
11. <span data-ttu-id="fc31f-130">在“起始值”字段中，输入一个数字。</span><span class="sxs-lookup"><span data-stu-id="fc31f-130">In the Starting value field, enter a number.</span></span>
12. <span data-ttu-id="fc31f-131">在“间隔”字段中，输入一个数字。</span><span class="sxs-lookup"><span data-stu-id="fc31f-131">In the Interval field, enter a number.</span></span>
13. <span data-ttu-id="fc31f-132">在“格式”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="fc31f-132">In the Format field, type a value.</span></span>
    * <span data-ttu-id="fc31f-133">例如，借出物品的起始编号为 10，则在“格式”字段中输入两个数字符号。</span><span class="sxs-lookup"><span data-stu-id="fc31f-133">For example, if the starting number for a loan item is 10, enter two number symbols symbols in the Format field.</span></span>  
14. <span data-ttu-id="fc31f-134">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="fc31f-134">Click OK.</span></span>
15. <span data-ttu-id="fc31f-135">刷新该页面。</span><span class="sxs-lookup"><span data-stu-id="fc31f-135">Refresh the page.</span></span>
