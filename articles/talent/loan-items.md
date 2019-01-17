---
title: 管理借给工作人员的物品
description: 借出物品是帮助经理跟踪您的公司借出给工作人员的实际物品。
author: kherr75
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-talent
ms.technology: ''
ms.search.form: HcmLoanItem, HcmLoanType, HcmPersonLoan
audience: Application User
ms.reviewer: rschloma
ms.search.scope: Core, Operations, Talent
ms.custom: 3581
ms.assetid: b14bdddb-f10e-4619-9f91-8c88439da862
ms.search.region: Global
ms.author: kherr
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Talent July 2017 update
ms.openlocfilehash: ae4c9a14a09602cc18d465bd4eded9bd11fc0205
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "60300"
---
# <a name="manage-items-that-are-lent-to-workers"></a><span data-ttu-id="d1d05-103">管理借给工作人员的物品</span><span class="sxs-lookup"><span data-stu-id="d1d05-103">Manage items that are lent to workers</span></span>

[!include [banner](includes/banner.md)]

<span data-ttu-id="d1d05-104">借出物品是帮助经理跟踪您的公司借出给工作人员的实际物品。</span><span class="sxs-lookup"><span data-stu-id="d1d05-104">Loan items are records that help managers track the physical items that your company lends to its workers.</span></span> 

<span data-ttu-id="d1d05-105">以下各点列出公司可能借出给工作人员的物品的示例：</span><span class="sxs-lookup"><span data-stu-id="d1d05-105">The following points list examples of items that a company might lend to workers:</span></span>
-   <span data-ttu-id="d1d05-106">手机</span><span class="sxs-lookup"><span data-stu-id="d1d05-106">Mobile telephones</span></span>
-   <span data-ttu-id="d1d05-107">汽车</span><span class="sxs-lookup"><span data-stu-id="d1d05-107">Automobiles</span></span>
-   <span data-ttu-id="d1d05-108">计算机设备</span><span class="sxs-lookup"><span data-stu-id="d1d05-108">Computer equipment</span></span>

<span data-ttu-id="d1d05-109">每个实际物品都必须具有相应的借出物品。</span><span class="sxs-lookup"><span data-stu-id="d1d05-109">Each physical item must have a corresponding loan item.</span></span> <span data-ttu-id="d1d05-110">每个借出物品记录都应描述所借物品，负责借出的员工和物品可以借出给工作人员的天数。</span><span class="sxs-lookup"><span data-stu-id="d1d05-110">Each loan item record should describe what is being loaned, who is responsible for the loan, and the number of days the item can loaned to a worker.</span></span> <span data-ttu-id="d1d05-111">您可以同时创建多个借出物品，例如钥匙、门卡或制服等。</span><span class="sxs-lookup"><span data-stu-id="d1d05-111">You can create multiple loan items, for items such as keys, access cards or uniforms, at the same time.</span></span> 

<span data-ttu-id="d1d05-112">借出物品时，应输入物品的借出日期和预定归还日期。</span><span class="sxs-lookup"><span data-stu-id="d1d05-112">When loaning an item, enter the date that the item was loaned, and the planned return date.</span></span> <span data-ttu-id="d1d05-113">当归还物品时，应输入实际的归还日期。</span><span class="sxs-lookup"><span data-stu-id="d1d05-113">When the item is returned, enter the actual return date.</span></span>

<span data-ttu-id="d1d05-114">员工可以使用员工自助服务工作区查看借出给他们的物品的记录。</span><span class="sxs-lookup"><span data-stu-id="d1d05-114">Employees can view the records of the items that have been loaned to them using the Employee self-service workspace.</span></span> <span data-ttu-id="d1d05-115">如果他们收到额外的实际物品，则他们还可以编辑现有记录或输入新借出物品。</span><span class="sxs-lookup"><span data-stu-id="d1d05-115">They can also edit the existing records or enter new loan items, if they've received additional physical items.</span></span>  <span data-ttu-id="d1d05-116">工作流可以设置为通过审核流程将更改传输到新的或现有的借出物品。</span><span class="sxs-lookup"><span data-stu-id="d1d05-116">Workflow can be set up to route changes to new or existing loan items through an approval process.</span></span> 

<span data-ttu-id="d1d05-117">经理可以查看借出给其直接下属的物品。</span><span class="sxs-lookup"><span data-stu-id="d1d05-117">Managers can view loaned items for their direct reports.</span></span> <span data-ttu-id="d1d05-118">他们还可以被授予权限来代表其新员工添加新借出物品。</span><span class="sxs-lookup"><span data-stu-id="d1d05-118">They can also be granted permission to add new loan items on behalf of their employees.</span></span>

 <a name="account-for-lost-or-misplaced-loan-items"></a><span data-ttu-id="d1d05-119">丢失或放错地方的借出物品的科目</span><span class="sxs-lookup"><span data-stu-id="d1d05-119">Account for lost or misplaced loan items</span></span>
-----------------------------------------

<span data-ttu-id="d1d05-120">如果物品被损坏或放错了地方，应输入虚拟的归还记录。</span><span class="sxs-lookup"><span data-stu-id="d1d05-120">If an item becomes damaged or misplaced, enter a fictitious return record.</span></span> <span data-ttu-id="d1d05-121">然后删除该物品或将其保留在概览中，并更改描述以指出该物品不可用。</span><span class="sxs-lookup"><span data-stu-id="d1d05-121">Then either delete the item or keep it in the overview and change the description to indicate that the item is not available.</span></span>


<a name="additional-resources"></a><span data-ttu-id="d1d05-122">其他资源</span><span class="sxs-lookup"><span data-stu-id="d1d05-122">Additional resources</span></span>
--------

[<span data-ttu-id="d1d05-123">人力资源</span><span class="sxs-lookup"><span data-stu-id="d1d05-123">Human resources</span></span>](index.md)


