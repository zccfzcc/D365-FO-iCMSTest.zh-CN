---
title: 创建成本元素
description: 可通过几种方法在成本核算中创建成本要素。
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CAMDimension, CAMAXMainAccountDimensionMemberProviderConfiguration, CAMDimensionMember
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 25d0613a72badf83da470c840a17c5d33908ad3f
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "53462"
---
# <a name="create-cost-elements"></a><span data-ttu-id="990c6-103">创建成本元素</span><span class="sxs-lookup"><span data-stu-id="990c6-103">Create cost elements</span></span> 

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="990c6-104">可通过几种方法在成本核算中创建成本要素。</span><span class="sxs-lookup"><span data-stu-id="990c6-104">There are several ways to create cost elements in Cost accounting.</span></span> <span data-ttu-id="990c6-105">此过程显示如何通过数据连接器导入主科目来创建成本要素。</span><span class="sxs-lookup"><span data-stu-id="990c6-105">This procedure shows how to create cost elements by importing main accounts via a data connector.</span></span> <span data-ttu-id="990c6-106">用于创建该过程的是演示公司 USMF。</span><span class="sxs-lookup"><span data-stu-id="990c6-106">The USMF demo company was used to create this procedure.</span></span> <span data-ttu-id="990c6-107">此过程针对 Microsoft Dynamics 365 for Operations 版本 1611 中增加的成本核算功能。</span><span class="sxs-lookup"><span data-stu-id="990c6-107">This procedure is for a Cost accounting feature that was added in Dynamics 365 for Operations, version 1611.</span></span>


## <a name="create-new-cost-elements"></a><span data-ttu-id="990c6-108">新建成本要素</span><span class="sxs-lookup"><span data-stu-id="990c6-108">Create new cost elements</span></span>
1. <span data-ttu-id="990c6-109">转到“成本核算”>“维度”>“成本要素维度”。</span><span class="sxs-lookup"><span data-stu-id="990c6-109">Go to Cost accounting > Dimensions > Cost element dimensions.</span></span>
2. <span data-ttu-id="990c6-110">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="990c6-110">Click New.</span></span>
3. <span data-ttu-id="990c6-111">在“名称”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="990c6-111">In the Name field, type a value.</span></span>
4. <span data-ttu-id="990c6-112">在“维度成员的数据连接器”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="990c6-112">In the Data connector for dimension members field, enter or select a value.</span></span>
5. <span data-ttu-id="990c6-113">在“描述”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="990c6-113">In the Description field, type a value.</span></span>
6. <span data-ttu-id="990c6-114">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="990c6-114">Click Save.</span></span>

## <a name="configure-the-data-connector"></a><span data-ttu-id="990c6-115">配置数据连接器</span><span class="sxs-lookup"><span data-stu-id="990c6-115">Configure the data connector</span></span>
1. <span data-ttu-id="990c6-116">单击“配置维度成员提供方”。</span><span class="sxs-lookup"><span data-stu-id="990c6-116">Click Configure dimension member provider.</span></span>
2. <span data-ttu-id="990c6-117">在“会计科目表”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="990c6-117">In the Chart of accounts field, enter or select a value.</span></span>
    * <span data-ttu-id="990c6-118">选择“共享”以使用共享的会计科目表。</span><span class="sxs-lookup"><span data-stu-id="990c6-118">Select Shared to use the shared chart of accounts.</span></span>  
3. <span data-ttu-id="990c6-119">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="990c6-119">Click New.</span></span>
4. <span data-ttu-id="990c6-120">在列表中，标记所选的行。</span><span class="sxs-lookup"><span data-stu-id="990c6-120">In the list, mark the selected row.</span></span>
    * <span data-ttu-id="990c6-121">可以为科目应用筛选器以满足条件。</span><span class="sxs-lookup"><span data-stu-id="990c6-121">You can apply filters to accounts to meet your criteria.</span></span>  
5. <span data-ttu-id="990c6-122">在“源主科目”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="990c6-122">In the From main account field, enter or select a value.</span></span>
6. <span data-ttu-id="990c6-123">在“目标主科目”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="990c6-123">In the To main account field, enter or select a value.</span></span>
7. <span data-ttu-id="990c6-124">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="990c6-124">Click OK.</span></span>

## <a name="import-main-accounts"></a><span data-ttu-id="990c6-125">导入主科目</span><span class="sxs-lookup"><span data-stu-id="990c6-125">Import main accounts</span></span>
1. <span data-ttu-id="990c6-126">单击“导入维度成员”。</span><span class="sxs-lookup"><span data-stu-id="990c6-126">Click Import dimension members.</span></span>
    * <span data-ttu-id="990c6-127">将把主科目导入成本核算并用作成本要素。</span><span class="sxs-lookup"><span data-stu-id="990c6-127">Main accounts will be imported into Cost accounting and used as cost elements.</span></span>  
2. <span data-ttu-id="990c6-128">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="990c6-128">Click OK.</span></span>

## <a name="view-the-imported-accounts-as-cost-elements"></a><span data-ttu-id="990c6-129">将导入的科目作为成本要素查看</span><span class="sxs-lookup"><span data-stu-id="990c6-129">View the imported accounts as cost elements</span></span>
1. <span data-ttu-id="990c6-130">单击“查看维度成员”。</span><span class="sxs-lookup"><span data-stu-id="990c6-130">Click View dimension members.</span></span>
    * <span data-ttu-id="990c6-131">将导入的会计科目作为成本可流向的业务中的成本要素查看。</span><span class="sxs-lookup"><span data-stu-id="990c6-131">View the imported ledger accounts as cost elements in your business that costs can flow to.</span></span>  

