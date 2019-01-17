---
title: Dynamics 365 for Talent Core HR（2018 年 10 月 15 日）中的新增功能或更改的功能
description: 此主题介绍了 Microsoft Dynamics 365 for Talent Core HR 中的新功能和更改的功能。
author: Darinkramer
manager: AnnBe
ms.date: 10/15/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-talent
ms.technology: ''
ms.search.form: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Talent
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: dkrame
ms.search.validFrom: 2018-10-11
ms.dyn365.ops.version: Talent
ms.openlocfilehash: 2733225129e149b667e970f4d3483fe3892e9936
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "60314"
---
# <a name="whats-new-or-changed-in-dynamics-365-for-talent-core-hr-october-15-2018"></a><span data-ttu-id="6d0b5-103">Dynamics 365 for Talent Core HR（2018 年 10 月 15 日）中的新增功能或更改的功能</span><span class="sxs-lookup"><span data-stu-id="6d0b5-103">What's new or changed in Dynamics 365 for Talent Core HR (October 15, 2018)</span></span>

[!include [banner](includes/banner.md)]

<span data-ttu-id="6d0b5-104">**内部版本 8.1.1056**</span><span class="sxs-lookup"><span data-stu-id="6d0b5-104">**Build 8.1.1056**</span></span>

<span data-ttu-id="6d0b5-105">此主题介绍了 Core HR 中的新增功能和更改的功能。</span><span class="sxs-lookup"><span data-stu-id="6d0b5-105">This topic describes features that are either new or changed in Core HR.</span></span>


## <a name="changes"></a><span data-ttu-id="6d0b5-106">更改</span><span class="sxs-lookup"><span data-stu-id="6d0b5-106">Changes</span></span>
<span data-ttu-id="6d0b5-107">除了杂项修复之外，此版本还进行了以下更新：</span><span class="sxs-lookup"><span data-stu-id="6d0b5-107">In addition to miscellanous fixes, the following updates have been made in this release:</span></span>
- <span data-ttu-id="6d0b5-108">现在，在招聘或设置雇用结束日期时，将设置最后工作日期。</span><span class="sxs-lookup"><span data-stu-id="6d0b5-108">Last Day worked now set when hiring or setting an employment end date.</span></span>
- <span data-ttu-id="6d0b5-109">在非美国公司时删除了美国符合性引用（ACA、ADA 和 I9）。</span><span class="sxs-lookup"><span data-stu-id="6d0b5-109">US compliance references removed when in non US companies (ACA, ADA, and I9).</span></span>
- <span data-ttu-id="6d0b5-110">无效日期 (1/1/1900) 现在在分析页面上隐藏。</span><span class="sxs-lookup"><span data-stu-id="6d0b5-110">Invalid dates (1/1/1900) are now hidden on analytics pages.</span></span>

## <a name="known-issue"></a><span data-ttu-id="6d0b5-111">已知问题</span><span class="sxs-lookup"><span data-stu-id="6d0b5-111">Known issue</span></span>

<span data-ttu-id="6d0b5-112">**问题：** 向工作人员添加新附件时，**新建**和**编辑**按钮灰显。**解决方法：** 打开附件页面之前，确保已关闭**工作人员**页面中的速见表。</span><span class="sxs-lookup"><span data-stu-id="6d0b5-112">**Issue:** When adding a new attachment to a worker, the **New** and **Edit** buttons are grayed out. **Workaround:** Before opening the attachment page, make sure that the FactBoxes on the **Worker** page are closed.</span></span> <span data-ttu-id="6d0b5-113">如果加载**工作人员**页面时速见表已关闭，将启用附件按钮。</span><span class="sxs-lookup"><span data-stu-id="6d0b5-113">If the FactBoxes are closed when the **Worker** page is loaded, the attachments buttons will be enabled.</span></span> <span data-ttu-id="6d0b5-114">（下一个平台更新中将解决这个问题。）</span><span class="sxs-lookup"><span data-stu-id="6d0b5-114">(This issue will be fixed in the next platform update.)</span></span>