---
title: 创建组织层次结构。
description: 使用以下过程创建组织层次结构。
author: sericks007
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: OMHierarchyManager, OMHierarchyPurposeAssociation, OMHierarchySelection, HierarchyDesigner
audience: Application User
ms.reviewer: sericks
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: sericks
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 5bec52874ff89fc656d23865d6010a7f750ed85c
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56037"
---
# <a name="create-an-organization-hierarchy"></a><span data-ttu-id="0a06e-103">创建组织层次结构。</span><span class="sxs-lookup"><span data-stu-id="0a06e-103">Create an organization hierarchy</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="0a06e-104">使用以下过程创建组织层次结构。</span><span class="sxs-lookup"><span data-stu-id="0a06e-104">Use the following procedure to create an organizational hierarchy.</span></span> <span data-ttu-id="0a06e-105">可以使用组织层次结构查看和申报来自各种视角的业务。</span><span class="sxs-lookup"><span data-stu-id="0a06e-105">You can use organizational hierarchies to view and report on your business from various perspectives.</span></span> <span data-ttu-id="0a06e-106">例如，您可以针对纳税、法律或法定申报设置一种层次结构。</span><span class="sxs-lookup"><span data-stu-id="0a06e-106">For example, you can set up one hierarchy for tax, legal, or statutory reporting.</span></span> <span data-ttu-id="0a06e-107">然后，您可以设置另一层次结构，以报告不是法律要求但用于内部报表的财务信息。</span><span class="sxs-lookup"><span data-stu-id="0a06e-107">You can then set up another hierarchy to report financial information that is not legally required, but that is used for internal reporting.</span></span> 



<span data-ttu-id="0a06e-108">在创建某一组织层次结构之前，必须先创建组织。</span><span class="sxs-lookup"><span data-stu-id="0a06e-108">Before you create an organizational hierarchy, you must create organizations.</span></span> <span data-ttu-id="0a06e-109">有关详细信息，请参阅“创建法人”或“创建运营单位”任务。</span><span class="sxs-lookup"><span data-stu-id="0a06e-109">For more information, see the “Create a legal entity” or “Create an operating unit” tasks.</span></span> <span data-ttu-id="0a06e-110">您还可以创建部门和团队。</span><span class="sxs-lookup"><span data-stu-id="0a06e-110">You can also create departments and teams.</span></span> 



<span data-ttu-id="0a06e-111">创建此程序的演示数据公司是 USMF。</span><span class="sxs-lookup"><span data-stu-id="0a06e-111">The demo data company used to create this procedure is USMF.</span></span>


## <a name="create-a-hierarchy"></a><span data-ttu-id="0a06e-112">创建层次结构</span><span class="sxs-lookup"><span data-stu-id="0a06e-112">Create a hierarchy</span></span>
1. <span data-ttu-id="0a06e-113">转到“组织管理”>“组织”>“组织层次结构”。</span><span class="sxs-lookup"><span data-stu-id="0a06e-113">Go to Organization administration > Organizations > Organization hierarchies.</span></span>
2. <span data-ttu-id="0a06e-114">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="0a06e-114">Click New.</span></span>
3. <span data-ttu-id="0a06e-115">在“名称”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="0a06e-115">In the Name field, type a value.</span></span>
4. <span data-ttu-id="0a06e-116">单击“分配用途”。</span><span class="sxs-lookup"><span data-stu-id="0a06e-116">Click Assign purpose.</span></span>
5. <span data-ttu-id="0a06e-117">在列表中，找到并选择所需记录。</span><span class="sxs-lookup"><span data-stu-id="0a06e-117">In the list, find and select the desired record.</span></span>
    * <span data-ttu-id="0a06e-118">选择分配给组织层次结构的用途。</span><span class="sxs-lookup"><span data-stu-id="0a06e-118">Select a purpose to assign to your organization hierarchy.</span></span>  
6. <span data-ttu-id="0a06e-119">单击“添加”。</span><span class="sxs-lookup"><span data-stu-id="0a06e-119">Click Add.</span></span>
7. <span data-ttu-id="0a06e-120">在列表中，标记所选的行。</span><span class="sxs-lookup"><span data-stu-id="0a06e-120">In the list, mark the selected row.</span></span>
    * <span data-ttu-id="0a06e-121">查找您刚才创建的层次结构。</span><span class="sxs-lookup"><span data-stu-id="0a06e-121">Find the hierarchy you just created.</span></span>  
8. <span data-ttu-id="0a06e-122">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="0a06e-122">Click OK.</span></span>

## <a name="add-organizations-to-the-hierarchy"></a><span data-ttu-id="0a06e-123">将组织添加到层次结构</span><span class="sxs-lookup"><span data-stu-id="0a06e-123">Add organizations to the hierarchy</span></span>
1. <span data-ttu-id="0a06e-124">在列表中，找到并选择所需记录。</span><span class="sxs-lookup"><span data-stu-id="0a06e-124">In the list, find and select the desired record.</span></span>
    * <span data-ttu-id="0a06e-125">选择层次结构。</span><span class="sxs-lookup"><span data-stu-id="0a06e-125">Select your hierarchy.</span></span>  
2. <span data-ttu-id="0a06e-126">单击“查看层次结构”。</span><span class="sxs-lookup"><span data-stu-id="0a06e-126">Click View hierarchy.</span></span>
    * <span data-ttu-id="0a06e-127">根据需要添加组织。</span><span class="sxs-lookup"><span data-stu-id="0a06e-127">Add organizations, as necessary.</span></span>  
    * <span data-ttu-id="0a06e-128">若要添加组织，单击“编辑”，然后单击“插入”来添加组织。</span><span class="sxs-lookup"><span data-stu-id="0a06e-128">To add an organization, click Edit and then Insert to add the organization.</span></span>     <span data-ttu-id="0a06e-129">在进行更改后，您可以保存草稿和/或发布更改。</span><span class="sxs-lookup"><span data-stu-id="0a06e-129">When you are done making changes you can save a draft and/or publish the changes.</span></span>  

