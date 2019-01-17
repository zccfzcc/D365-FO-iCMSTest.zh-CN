---
title: 更改多项固定资产的折旧惯例
description: 此任务更新特定固定资产组的折旧惯例。
author: saraschi2
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysQueryForm, SrsReportViewerForm
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 5d140007b1e30460e248e81d3efe208b3917e017
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56377"
---
# <a name="change-depreciation-conventions-for-multiple-fixed-assets"></a><span data-ttu-id="88b88-103">更改多项固定资产的折旧惯例</span><span class="sxs-lookup"><span data-stu-id="88b88-103">Change depreciation conventions for multiple fixed assets</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="88b88-104">此任务更新特定固定资产组的折旧惯例。</span><span class="sxs-lookup"><span data-stu-id="88b88-104">This task updates the depreciation convention for a specified fixed asset group.</span></span> <span data-ttu-id="88b88-105">此任务指南使用 USMF 公司演示。</span><span class="sxs-lookup"><span data-stu-id="88b88-105">This task guide uses the USMF demo company.</span></span>

1. <span data-ttu-id="88b88-106">转到“固定资产”>“定期任务”>“成批更新”</span><span class="sxs-lookup"><span data-stu-id="88b88-106">Go to Fixed assets > Periodic tasks > Mass update</span></span>
2. <span data-ttu-id="88b88-107">在“折旧帐簿”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="88b88-107">In the Depreciation book field, click the drop-down button to open the lookup.</span></span>
3. <span data-ttu-id="88b88-108">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="88b88-108">In the list, click the link in the selected row.</span></span>
4. <span data-ttu-id="88b88-109">在“开始投入使用”字段，输入日期。</span><span class="sxs-lookup"><span data-stu-id="88b88-109">In the Placed in service start field, enter a date.</span></span>
5. <span data-ttu-id="88b88-110">在“投入使用结束”字段，输入日期。</span><span class="sxs-lookup"><span data-stu-id="88b88-110">In the Placed in service end field, enter a date.</span></span>
    * <span data-ttu-id="88b88-111">仅所选折旧帐簿中的且在该等日期之间投入使用的资产才会更新。</span><span class="sxs-lookup"><span data-stu-id="88b88-111">Only assets that are a part of the select depreciation book and that have been placed in service between these dates will be updated.</span></span>  
6. <span data-ttu-id="88b88-112">在“当前折旧惯例”字段中，选择一个选项。</span><span class="sxs-lookup"><span data-stu-id="88b88-112">In the Current depreciation convention field, select an option.</span></span>
    * <span data-ttu-id="88b88-113">仅属于当前折旧惯例的资产才会更新。</span><span class="sxs-lookup"><span data-stu-id="88b88-113">Only assets that have the current depreciation convention will be updated.</span></span>  
7. <span data-ttu-id="88b88-114">在“新折旧惯例”字段中，选择一个选项。</span><span class="sxs-lookup"><span data-stu-id="88b88-114">In the New depreciation convention field, select an option.</span></span>
    * <span data-ttu-id="88b88-115">验证报表将打印给所选目标。</span><span class="sxs-lookup"><span data-stu-id="88b88-115">Verify the report will print to the desired destination.</span></span>  
8. <span data-ttu-id="88b88-116">扩展“要包括的记录”部分。</span><span class="sxs-lookup"><span data-stu-id="88b88-116">Expand the Records to include section.</span></span>
9. <span data-ttu-id="88b88-117">单击“筛选器”。</span><span class="sxs-lookup"><span data-stu-id="88b88-117">Click Filter.</span></span>
10. <span data-ttu-id="88b88-118">在列表中选择固定资产组。</span><span class="sxs-lookup"><span data-stu-id="88b88-118">In the list, select the Fixed asset group.</span></span>
11. <span data-ttu-id="88b88-119">在“标准”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="88b88-119">In the Criteria field, click the drop-down button to open the lookup.</span></span>
12. <span data-ttu-id="88b88-120">选择期望的固定资产组。</span><span class="sxs-lookup"><span data-stu-id="88b88-120">Select the desired Fixed asset group.</span></span>
13. <span data-ttu-id="88b88-121">在列表中，单击所选行中的链接。</span><span class="sxs-lookup"><span data-stu-id="88b88-121">In the list, click the link in the selected row.</span></span>
14. <span data-ttu-id="88b88-122">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="88b88-122">Click OK.</span></span>
15. <span data-ttu-id="88b88-123">单击“确定”。</span><span class="sxs-lookup"><span data-stu-id="88b88-123">Click OK.</span></span>
    *  <span data-ttu-id="88b88-124">流程结果将在成批更新报表中显示。</span><span class="sxs-lookup"><span data-stu-id="88b88-124">Results of the process are shown on the Mass update report.</span></span>     
