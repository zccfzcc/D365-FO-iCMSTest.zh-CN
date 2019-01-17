---
title: 创建 POS 收银机的财务维度并配置收银机上的维度值
description: 此程序会逐步演示如何创建销售点 (POS) 收银机的财务维度，以及演示如何配置收银机的财务维度值。
author: jashanno
manager: AnnBe
ms.date: 11/14/2016
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Operations, Retail
ms.search.region: Global
ms.search.industry: Retail
ms.author: jashanno
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: d94aec6a49f8e9a259d3f339a10d13f6545aaa08
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56150"
---
# <a name="create-financial-dimensions-for-pos-registers-and-configure-dimension-values-on-registers"></a><span data-ttu-id="291ce-103">创建 POS 收银机的财务维度并配置收银机上的维度值</span><span class="sxs-lookup"><span data-stu-id="291ce-103">Create financial dimensions for POS registers and configure dimension values on registers</span></span>

[!include [task guide banner](../includes/task-guide-banner.md)]

<span data-ttu-id="291ce-104">此程序会逐步演示如何创建销售点 (POS) 收银机的财务维度，以及演示如何配置收银机的财务维度值。</span><span class="sxs-lookup"><span data-stu-id="291ce-104">This procedure walks through creating financial dimensions for point of sale (POS) registers, and demonstrates how to configure financial dimension values on registers.</span></span> <span data-ttu-id="291ce-105">此程序不包括其他相关步骤，例如创建维度集和科目结构。</span><span class="sxs-lookup"><span data-stu-id="291ce-105">This procedure doesn’t include other related steps, such as creating dimension sets and account structures.</span></span> <span data-ttu-id="291ce-106">这些任务可在其他主题中找到。</span><span class="sxs-lookup"><span data-stu-id="291ce-106">Those tasks can be found in other topics.</span></span> <span data-ttu-id="291ce-107">此记录使用 USRT 演示公司。</span><span class="sxs-lookup"><span data-stu-id="291ce-107">This recording uses USRT demo company.</span></span>

1. <span data-ttu-id="291ce-108">转到“总帐”>“会计科目表”>“维度”>“财务维度”。</span><span class="sxs-lookup"><span data-stu-id="291ce-108">Go to General ledger > Chart of accounts > Dimensions > Financial dimensions.</span></span>
2. <span data-ttu-id="291ce-109">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="291ce-109">Click New.</span></span>
3. <span data-ttu-id="291ce-110">在“使用以下来源中的值”字段中，选择一个选项。</span><span class="sxs-lookup"><span data-stu-id="291ce-110">In the Use values from field, select an option.</span></span>
4. <span data-ttu-id="291ce-111">在“维度名称”字段中，输入一个值。</span><span class="sxs-lookup"><span data-stu-id="291ce-111">In the Dimension name field, type a value.</span></span>
5. <span data-ttu-id="291ce-112">单击“启用”。</span><span class="sxs-lookup"><span data-stu-id="291ce-112">Click Activate.</span></span>
6. <span data-ttu-id="291ce-113">单击“关闭”。</span><span class="sxs-lookup"><span data-stu-id="291ce-113">Click Close.</span></span>
7. <span data-ttu-id="291ce-114">单击“启用”。</span><span class="sxs-lookup"><span data-stu-id="291ce-114">Click Activate.</span></span>
8. <span data-ttu-id="291ce-115">单击“维度值”。</span><span class="sxs-lookup"><span data-stu-id="291ce-115">Click Dimension values.</span></span>
9. <span data-ttu-id="291ce-116">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="291ce-116">Close the page.</span></span>
10. <span data-ttu-id="291ce-117">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="291ce-117">Click Save.</span></span>
11. <span data-ttu-id="291ce-118">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="291ce-118">Close the page.</span></span>
12. <span data-ttu-id="291ce-119">转至“零售和商业”>“渠道设置”>“POS 设置”>“收银机”。</span><span class="sxs-lookup"><span data-stu-id="291ce-119">Go to Retail and commerce > Channel setup > POS setup > Registers.</span></span>
13. <span data-ttu-id="291ce-120">在列表中，找到并选择所需记录。</span><span class="sxs-lookup"><span data-stu-id="291ce-120">In the list, find and select the desired record.</span></span>
14. <span data-ttu-id="291ce-121">切换“财务维度”部分的展开项。</span><span class="sxs-lookup"><span data-stu-id="291ce-121">Toggle the expansion of the Financial dimensions section.</span></span>
15. <span data-ttu-id="291ce-122">单击“编辑”。</span><span class="sxs-lookup"><span data-stu-id="291ce-122">Click Edit.</span></span>
16. <span data-ttu-id="291ce-123">在“终端”字段中，单击下拉按钮以打开查找。</span><span class="sxs-lookup"><span data-stu-id="291ce-123">In the Terminal field, click the drop-down button to open the lookup.</span></span>
17. <span data-ttu-id="291ce-124">在列表中，查找并选择正在更新的收银机的维度值。</span><span class="sxs-lookup"><span data-stu-id="291ce-124">In the list, find and select the dimension value for the register being updated.</span></span>
18. <span data-ttu-id="291ce-125">单击“保存”。</span><span class="sxs-lookup"><span data-stu-id="291ce-125">Click Save.</span></span>
