---
title: 创建记录模板以加快数据输入
description: 此过程演示如何创建报表模板，以便不必明确为每条记录输入常用字段值。
author: margoc
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: AssetTable, SysRecordInfo, SysRecordTemplatePromptOnCreate
audience: Application User
ms.reviewer: margoc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: margoc
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: bc3c69b98a0f1d447de7d9ab620d140a2a26e4c6
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54655"
---
# <a name="create-a-record-template-to-facilitate-data-entry"></a><span data-ttu-id="f43fa-103">创建记录模板以加快数据输入</span><span class="sxs-lookup"><span data-stu-id="f43fa-103">Create a record template to facilitate data entry</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="f43fa-104">此过程演示如何创建报表模板，以便不必明确为每条记录输入常用字段值。</span><span class="sxs-lookup"><span data-stu-id="f43fa-104">This procedure demonstrates how to create a record template so that field values that are used often do not have to be entered explicitly for each new record.</span></span> <span data-ttu-id="f43fa-105">在此过程中，您将为应添加到固定资产的新笔记本电脑创建一条新记录。</span><span class="sxs-lookup"><span data-stu-id="f43fa-105">In this procedure, you’ll create a new record for new laptops that should be added to your fixed assets.</span></span> <span data-ttu-id="f43fa-106">本流程使用了 USMF 示例公司。</span><span class="sxs-lookup"><span data-stu-id="f43fa-106">This procedure uses the USMF sample company.</span></span>

1. <span data-ttu-id="f43fa-107">转到“固定资产”>“固定资产”>“固定资产”。</span><span class="sxs-lookup"><span data-stu-id="f43fa-107">Go to Fixed assets > Fixed assets > Fixed assets.</span></span>
2. <span data-ttu-id="f43fa-108">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="f43fa-108">Click New.</span></span>
3. <span data-ttu-id="f43fa-109">在“固定资产组”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="f43fa-109">In the Fixed asset group field, enter or select a value.</span></span>
4. <span data-ttu-id="f43fa-110">在“名称”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="f43fa-110">In the Name field, type a value.</span></span>
    * <span data-ttu-id="f43fa-111">例如，输入“公司潜在客户笔记本电脑”。</span><span class="sxs-lookup"><span data-stu-id="f43fa-111">For example, enter 'Corporate lead laptop'.</span></span>  
5. <span data-ttu-id="f43fa-112">在“搜索名称”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="f43fa-112">In the Search name field, type a value.</span></span>
    * <span data-ttu-id="f43fa-113">例如，输入“笔记本电脑”。</span><span class="sxs-lookup"><span data-stu-id="f43fa-113">For example, enter 'laptop.'</span></span>  
6. <span data-ttu-id="f43fa-114">展开“技术信息”部分。</span><span class="sxs-lookup"><span data-stu-id="f43fa-114">Expand the Technical information section.</span></span>
7. <span data-ttu-id="f43fa-115">在“创建”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="f43fa-115">In the Make field, type a value.</span></span>
8. <span data-ttu-id="f43fa-116">在“型号”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="f43fa-116">In the Model field, type a value.</span></span>
9. <span data-ttu-id="f43fa-117">在“型号年份”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="f43fa-117">In the Model year field, type a value.</span></span>
10. <span data-ttu-id="f43fa-118">在“操作窗格”上，单击“选项”。</span><span class="sxs-lookup"><span data-stu-id="f43fa-118">On the Action Pane, click Options.</span></span>
11. <span data-ttu-id="f43fa-119">单击“记录信息”。</span><span class="sxs-lookup"><span data-stu-id="f43fa-119">Click Record info.</span></span>
12. <span data-ttu-id="f43fa-120">单击“用户模板”。</span><span class="sxs-lookup"><span data-stu-id="f43fa-120">Click User template.</span></span>
13. <span data-ttu-id="f43fa-121">在“名称”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="f43fa-121">In the Name field, type a value.</span></span>
    * <span data-ttu-id="f43fa-122">例如，输入“公司笔记本电脑”。</span><span class="sxs-lookup"><span data-stu-id="f43fa-122">For example, enter 'Corporate laptop.'</span></span>  
14. <span data-ttu-id="f43fa-123">在“描述”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="f43fa-123">In the Description field, type a value.</span></span>
    * <span data-ttu-id="f43fa-124">例如，输入“公司笔记本电脑”。</span><span class="sxs-lookup"><span data-stu-id="f43fa-124">For example, enter 'Corporate laptop'.</span></span>  
15. <span data-ttu-id="f43fa-125">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="f43fa-125">Click OK.</span></span>
16. <span data-ttu-id="f43fa-126">单击“关闭”。</span><span class="sxs-lookup"><span data-stu-id="f43fa-126">Click Close.</span></span>

