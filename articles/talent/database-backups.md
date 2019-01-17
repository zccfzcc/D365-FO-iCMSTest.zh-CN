---
title: 处理数据库备份的方式
description: 本主题将帮助要了解 SQL 备份的客户。
author: Darinkramer
manager: AnnBe
ms.date: 11/02/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-talent
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Talent
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: dkrame
ms.search.validFrom: 2018-11-02
ms.dyn365.ops.version: Talent
ms.openlocfilehash: c74b2caa63c3044f9c260246acc8639da0d3d211
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "60295"
---
# <a name="how-database-backups-are-handled"></a><span data-ttu-id="914a1-103">处理数据库备份的方式</span><span class="sxs-lookup"><span data-stu-id="914a1-103">How database backups are handled</span></span>

[!include [banner](includes/banner.md)]

<span data-ttu-id="914a1-104">**环境详细信息**</span><span class="sxs-lookup"><span data-stu-id="914a1-104">**Environment details**</span></span>

<span data-ttu-id="914a1-105">通过 Microsoft Dynamics Lifecycle Services (LCS) 设置的生产环境</span><span class="sxs-lookup"><span data-stu-id="914a1-105">Production environments that are provisioned through Microsoft Dynamics Lifecycle Services (LCS)</span></span>

<span data-ttu-id="914a1-106">**发货**</span><span class="sxs-lookup"><span data-stu-id="914a1-106">**Issue**</span></span>

- <span data-ttu-id="914a1-107">客户想要了解 Microsoft Dynamics 365 for Talent 的 SQL 备份计划。</span><span class="sxs-lookup"><span data-stu-id="914a1-107">The customer wants to understand the SQL backup plan for Microsoft Dynamics 365 for Talent.</span></span>
- <span data-ttu-id="914a1-108">客户想要还原生产环境的 SQL 备份。</span><span class="sxs-lookup"><span data-stu-id="914a1-108">The customer wants to restore a SQL backup for a production environment.</span></span>
- <span data-ttu-id="914a1-109">客户希望将数据库从生产环境移至测试环境。</span><span class="sxs-lookup"><span data-stu-id="914a1-109">The customer wants to move a database from a production environment to a test environment.</span></span>

<span data-ttu-id="914a1-110">**解决方案**</span><span class="sxs-lookup"><span data-stu-id="914a1-110">**Solution**</span></span>

- <span data-ttu-id="914a1-111">Talent 使用标准 Microsoft Azure SQL 数据库库存单位 (SKU)。</span><span class="sxs-lookup"><span data-stu-id="914a1-111">Talent uses a standard Microsoft Azure SQL Database stock keeping unit (SKU).</span></span> <span data-ttu-id="914a1-112">有关备份的详细信息，请参阅[了解自动 SQL 数据库备份](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-automated-backups)。</span><span class="sxs-lookup"><span data-stu-id="914a1-112">For more information about backups, see [Learn about automatic SQL Database backups](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-automated-backups).</span></span>
- <span data-ttu-id="914a1-113">就地生产环境备份的还原是应被视为昂贵的 Development Operations (DevOps) 操作。</span><span class="sxs-lookup"><span data-stu-id="914a1-113">Restoration of an in-place production environment backup is a Development Operations (DevOps) operation that should be considered expensive.</span></span> <span data-ttu-id="914a1-114">实际上，对备份的还原程度是有限制的。</span><span class="sxs-lookup"><span data-stu-id="914a1-114">In fact, there are limits on how far back we can restore backups.</span></span> <span data-ttu-id="914a1-115">由于代码包几乎每周升级，我们不希望还原与代码包的当前版本兼容的备份。</span><span class="sxs-lookup"><span data-stu-id="914a1-115">Because the code packages are upgraded almost every week, we don't want to restore a backup that isn't compatible with the current version of the code package.</span></span> <span data-ttu-id="914a1-116">因此，我们必须根据实际情况具体考虑最佳方法。</span><span class="sxs-lookup"><span data-stu-id="914a1-116">Therefore, we must consider the best approach on a case-by-case basis.</span></span>
- <span data-ttu-id="914a1-117">目前，将数据库从生产环境移至测试环境是一项 DevOps 操作。</span><span class="sxs-lookup"><span data-stu-id="914a1-117">Currently, moving a database from a production environment to a test environment is a DevOps operation.</span></span> <span data-ttu-id="914a1-118">Microsoft 当前不提供在 LCS 体验中移动或复制数据库的途径。</span><span class="sxs-lookup"><span data-stu-id="914a1-118">Microsoft doesn't currently provide a way to move or copy databases in the LCS experience.</span></span> <span data-ttu-id="914a1-119">此功能已经请求，但尚未完成。</span><span class="sxs-lookup"><span data-stu-id="914a1-119">This feature has been requested but hasn't yet been completed.</span></span> <span data-ttu-id="914a1-120">我们建议您使用数据实体包在环境之间导出/导入。</span><span class="sxs-lookup"><span data-stu-id="914a1-120">We recommend that you use data entity packages to export/import between environments.</span></span>

<span data-ttu-id="914a1-121">**长期解决方案**</span><span class="sxs-lookup"><span data-stu-id="914a1-121">**Long-term solution**</span></span>

<span data-ttu-id="914a1-122">作为我们长期未来计划的一部分，我们计划添加将生产数据库复制到测试环境的选项。</span><span class="sxs-lookup"><span data-stu-id="914a1-122">As part of our longer-term future plans, we intend to add an option to copy a production database to a test environment.</span></span>
