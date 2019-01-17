---
title: 手动修改需求预测
description: 此过程显示如何修改物料预测。
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: EcoResProductDetailsExtended, ForecastSales
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: b908bbdce61751f873c8c05fc4aacbf1ee74f4a1
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56259"
---
# <a name="modify-a-demand-forecast-manually"></a><span data-ttu-id="97bfc-103">手动修改需求预测</span><span class="sxs-lookup"><span data-stu-id="97bfc-103">Modify a demand forecast manually</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="97bfc-104">此过程显示如何修改物料预测。</span><span class="sxs-lookup"><span data-stu-id="97bfc-104">This procedure shows how to modify the forecast for an item.</span></span> <span data-ttu-id="97bfc-105">创建此程序的演示数据公司是 USMF。</span><span class="sxs-lookup"><span data-stu-id="97bfc-105">The demo data company used to create this procedure is USMF.</span></span> <span data-ttu-id="97bfc-106">此记录专供生产规划员使用。</span><span class="sxs-lookup"><span data-stu-id="97bfc-106">This recording is intended for the production planner.</span></span> 


## <a name="modify-the-forecast-for-an-item"></a><span data-ttu-id="97bfc-107">修改物料预测</span><span class="sxs-lookup"><span data-stu-id="97bfc-107">Modify the forecast for an item</span></span>
1. <span data-ttu-id="97bfc-108">转到“产品信息管理”>“产品”>“已发布产品”。</span><span class="sxs-lookup"><span data-stu-id="97bfc-108">Go to Product information management > Products > Released products.</span></span>
2. <span data-ttu-id="97bfc-109">在列表中，找到并选择所需记录。</span><span class="sxs-lookup"><span data-stu-id="97bfc-109">In the list, find and select the desired record.</span></span>
    * <span data-ttu-id="97bfc-110">选择要更改预测的物料。</span><span class="sxs-lookup"><span data-stu-id="97bfc-110">Select the item for which you want to modify the forecast.</span></span> <span data-ttu-id="97bfc-111">例如，可以选择物料 D0001。</span><span class="sxs-lookup"><span data-stu-id="97bfc-111">For example, you can select item D0001.</span></span>  
3. <span data-ttu-id="97bfc-112">在操作窗格上，单击“计划”。</span><span class="sxs-lookup"><span data-stu-id="97bfc-112">On the Action Pane, click Plan.</span></span>
4. <span data-ttu-id="97bfc-113">单击“需求预测”。</span><span class="sxs-lookup"><span data-stu-id="97bfc-113">Click Demand forecast.</span></span>
5. <span data-ttu-id="97bfc-114">在列表中，标记所选的行。</span><span class="sxs-lookup"><span data-stu-id="97bfc-114">In the list, mark the selected row.</span></span>
    * <span data-ttu-id="97bfc-115">如果没有预测行，则单击“在应用程序栏上新建”</span><span class="sxs-lookup"><span data-stu-id="97bfc-115">If there are no forecast lines, create a new line by  .</span></span> <span data-ttu-id="97bfc-116">来创建一个新行。</span><span class="sxs-lookup"><span data-stu-id="97bfc-116">clicking New on the app bar.</span></span>  
6. <span data-ttu-id="97bfc-117">在“销售数量”字段中，输入一个数字。</span><span class="sxs-lookup"><span data-stu-id="97bfc-117">In the Sales quantity field, enter a number.</span></span>
    * <span data-ttu-id="97bfc-118">此数字代表该物料的预测数量。</span><span class="sxs-lookup"><span data-stu-id="97bfc-118">This number represents the forecasted quantity for the item.</span></span>  
7. <span data-ttu-id="97bfc-119">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="97bfc-119">Click Save.</span></span>

## <a name="modify-the-forecast-in-excel"></a><span data-ttu-id="97bfc-120">在 Excel 中修改预测</span><span class="sxs-lookup"><span data-stu-id="97bfc-120">Modify the forecast in Excel</span></span>
1. <span data-ttu-id="97bfc-121">单击“在 Microsoft Office 中打开”。</span><span class="sxs-lookup"><span data-stu-id="97bfc-121">Click Open in Microsoft Office.</span></span>
2. <span data-ttu-id="97bfc-122">单击“在 Excel 中编辑需求预测”。</span><span class="sxs-lookup"><span data-stu-id="97bfc-122">Click Edit Demand forecast in Excel.</span></span>
    * <span data-ttu-id="97bfc-123">在 Excel 中，您可以添加、删除和编辑需求预测行。</span><span class="sxs-lookup"><span data-stu-id="97bfc-123">In Excel, you can add, delete and edit demand forecast lines.</span></span> <span data-ttu-id="97bfc-124">如果您将无法看到在 Excel 中的数据，需要使用已启用的“登录”选项登录 Microsoft Dynamics 365 for Finance and Operations Enterprise Edition，并且需要信任数据连接应用程序。</span><span class="sxs-lookup"><span data-stu-id="97bfc-124">If you are not able to see the data in Excel, you need to sign in to Microsoft Dynamics 365 for Finance and Operations, Enterprise edition with the "Keep me signed in" option enabled and you need to trust the data connection app.</span></span>  
