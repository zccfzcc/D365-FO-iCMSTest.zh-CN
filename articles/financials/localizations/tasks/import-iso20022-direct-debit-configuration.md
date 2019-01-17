---
title: 导入 ISO20022 直接借记配置
description: 此过程演示如何导入客户付款电子申报配置。
author: mrolecki
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ERWorkspace, ERVendorPart, ERSolutionRepositoryTable, ERSolutionImport
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mrolecki
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: cb4048522c5bb779905231b8403033541e2771b7
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54501"
---
# <a name="import-iso20022-direct-debit-configuration"></a><span data-ttu-id="a2cd0-103">导入 ISO20022 直接借记配置</span><span class="sxs-lookup"><span data-stu-id="a2cd0-103">Import ISO20022 direct debit configuration</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="a2cd0-104">此过程演示如何导入客户付款电子申报配置。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-104">This procedure demonstrates how to import a customer payment electronic reporting configuration.</span></span> <span data-ttu-id="a2cd0-105">此过程以 ISO 20022 直接借记格式为例。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-105">This procedure uses the ISO 20022 direct debit format as an example.</span></span> 



<span data-ttu-id="a2cd0-106">此过程是使用演示数据公司 DEMF 创建的，但是您可以使用任何演示数据公司达成此目的。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-106">This procedure was created using the demo data company DEMF but you can use any demo data company for this purpose.</span></span>



<span data-ttu-id="a2cd0-107">这是五个用于演示使用电子申报配置的客户付款流程的过程中的第一个。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-107">This is the first of five procedures that demonstrate the customer payment process using electronic reporting configurations.</span></span>

1. <span data-ttu-id="a2cd0-108">转到“组织管理”>“工作区”>“电子申报”。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-108">Go to Organization administration > Workspaces > Electronic reporting.</span></span>
2. <span data-ttu-id="a2cd0-109">在可用配置提供商列表中，选择“Microsoft”。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-109">In the list of available configuration providers, select Microsoft.</span></span>
3. <span data-ttu-id="a2cd0-110">单击“设置有效”。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-110">Click Set active.</span></span>
4. <span data-ttu-id="a2cd0-111">单击“存储库”。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-111">Click Repositories.</span></span>
5. <span data-ttu-id="a2cd0-112">单击“打开”。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-112">Click Open.</span></span>
6. <span data-ttu-id="a2cd0-113">单击“显示筛选器”。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-113">Click Show filters.</span></span>
7. <span data-ttu-id="a2cd0-114">应用以下筛选器：使用“开头为”筛选器运算符在“配置名称”字段中输入筛选器值“ISO20022 直接借记（德国）”。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-114">Apply the following filters: Enter a filter value of "ISO20022 Direct debit (DE)" on the "Configuration name" field using the "begins with" filter operator</span></span>
    * <span data-ttu-id="a2cd0-115">也可以在列表中找到配置，选中，然后跳过此步骤。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-115">Optionally, you can find the configuration in the list, select it, and skip this step.</span></span>  
8. <span data-ttu-id="a2cd0-116">单击“导入”。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-116">Click Import.</span></span>
    * <span data-ttu-id="a2cd0-117">如果导入按钮没出现，表示该配置文件已经被导入了。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-117">If the Import button is not available, it means that the configuration has been imported already.</span></span>  
9. <span data-ttu-id="a2cd0-118">单击“是”。</span><span class="sxs-lookup"><span data-stu-id="a2cd0-118">Click Yes.</span></span>

