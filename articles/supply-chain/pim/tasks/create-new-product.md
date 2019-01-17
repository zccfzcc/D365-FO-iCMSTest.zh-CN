---
title: 创建新产品
description: 此任务显示如何创建新的共享的产品。
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: EcoResProductListPage, EcoResProductCreate, EcoResProductDetails, EcoResProductInventoryDimensionGroups
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 447b47d6ef1d54c2a280d8b02513156913b61b3b
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "53266"
---
# <a name="create-a-new-product"></a><span data-ttu-id="d9542-103">创建新产品</span><span class="sxs-lookup"><span data-stu-id="d9542-103">Create a new product</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="d9542-104">此任务显示如何创建新的共享的产品。</span><span class="sxs-lookup"><span data-stu-id="d9542-104">This task shows how to create a new shared product.</span></span> <span data-ttu-id="d9542-105">它通常由产品设计器执行。</span><span class="sxs-lookup"><span data-stu-id="d9542-105">It is usually carried out by a product designer.</span></span> <span data-ttu-id="d9542-106">创建此任务的演示数据公司是 USMF。</span><span class="sxs-lookup"><span data-stu-id="d9542-106">The demo data company used to create this task is USMF.</span></span>

1. <span data-ttu-id="d9542-107">转到“产品信息管理”>“产品”>“产品”。</span><span class="sxs-lookup"><span data-stu-id="d9542-107">Go to Product information management > Products > Products.</span></span>

## <a name="create-a-product"></a><span data-ttu-id="d9542-108">创建产品</span><span class="sxs-lookup"><span data-stu-id="d9542-108">Create a product</span></span>
1. <span data-ttu-id="d9542-109">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="d9542-109">Click New.</span></span>
2. <span data-ttu-id="d9542-110">在“产品编号”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="d9542-110">In the Product number field, type a value.</span></span>
    * <span data-ttu-id="d9542-111">如果编号规则没有为产品编号设置，必须手动输入它。</span><span class="sxs-lookup"><span data-stu-id="d9542-111">If a number sequence has not been set up for the product number, it must be entered manually.</span></span>  
3. <span data-ttu-id="d9542-112">在“产品名称”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="d9542-112">In the Product name field, type a value.</span></span>
    * <span data-ttu-id="d9542-113">产品名称默认为搜索名称。</span><span class="sxs-lookup"><span data-stu-id="d9542-113">The product name defaults to the search name.</span></span> <span data-ttu-id="d9542-114">可以根据需要更改。</span><span class="sxs-lookup"><span data-stu-id="d9542-114">You can change this if needed.</span></span>  
4. <span data-ttu-id="d9542-115">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="d9542-115">Click OK.</span></span>

## <a name="set-up-dimension-groups"></a><span data-ttu-id="d9542-116">设置维度组</span><span class="sxs-lookup"><span data-stu-id="d9542-116">Set up dimension groups</span></span>
1. <span data-ttu-id="d9542-117">单击“维度组”以打开下拉对话框。</span><span class="sxs-lookup"><span data-stu-id="d9542-117">Click Dimension groups to open the drop dialog.</span></span>
2. <span data-ttu-id="d9542-118">在“存储维度组”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="d9542-118">In the Storage dimension group field, enter or select a value.</span></span>
    * <span data-ttu-id="d9542-119">存储维度组确定哪些存储维度您必须在产品的每个交易记录中输入，以及如何在库存中跟踪。</span><span class="sxs-lookup"><span data-stu-id="d9542-119">The storage dimension group determines which storage dimensions you must enter on each transaction for the product and how it will be tracked in inventory.</span></span>  
3. <span data-ttu-id="d9542-120">在“跟踪维度组”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="d9542-120">In the Tracking dimension group field, enter or select a value.</span></span>
    * <span data-ttu-id="d9542-121">跟踪维度组确定哪些跟踪维度您必须为产品的每个交易记录输入，以及如何在库存中处置。</span><span class="sxs-lookup"><span data-stu-id="d9542-121">The tracking dimension group determines which tracking dimensions you must enter for each transaction for the product, and how it will be handled in inventory.</span></span>  
4. <span data-ttu-id="d9542-122">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="d9542-122">Click OK.</span></span>

