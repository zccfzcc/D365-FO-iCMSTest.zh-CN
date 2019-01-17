---
title: Dynamics 365 for Talent Core HR（2018 年 11 月 15 日）中的新增功能或更改的功能
description: 此主题介绍了 Microsoft Dynamics 365 for Talent Core HR 中的新功能和更改的功能。
author: Darinkramer
manager: AnnBe
ms.date: 11/15/2018
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
ms.search.validFrom: 2018-11-15
ms.dyn365.ops.version: Talent
ms.openlocfilehash: 2adad48e347f3fff8e33302a9c7bcd9442278b6d
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "60320"
---
# <a name="whats-new-or-changed-in-dynamics-365-for-talent-core-hr-november-15-2018"></a><span data-ttu-id="73fda-103">Dynamics 365 for Talent Core HR（2018 年 11 月 15 日）中的新增功能或更改的功能</span><span class="sxs-lookup"><span data-stu-id="73fda-103">What's new or changed in Dynamics 365 for Talent Core HR (November 15, 2018)</span></span>

[!include [banner](includes/banner.md)]

<span data-ttu-id="73fda-104">**内部版本 8.1.2045**</span><span class="sxs-lookup"><span data-stu-id="73fda-104">**Build 8.1.2045**</span></span>

<span data-ttu-id="73fda-105">此主题介绍了 Core HR 中的新增功能和更改的功能。</span><span class="sxs-lookup"><span data-stu-id="73fda-105">This topic describes features that are either new or changed in Core HR.</span></span>

## <a name="other-changesfixes"></a><span data-ttu-id="73fda-106">其他更改/修复</span><span class="sxs-lookup"><span data-stu-id="73fda-106">Other changes/fixes</span></span>

### <a name="unable-to-change-employees-current-position-to-a-future-open-position"></a><span data-ttu-id="73fda-107">无法将员工的当前职位更改为将来的空缺职位</span><span class="sxs-lookup"><span data-stu-id="73fda-107">Unable to change employee´s current position to a future open position</span></span>

<span data-ttu-id="73fda-108">已进行了更改来在职位仅在未来可用时启用职位转移。</span><span class="sxs-lookup"><span data-stu-id="73fda-108">A change has been made to enable position transfers when the position is only available in the future.</span></span> 

### <a name="position-does-not-display-when-creating-a-new-employee"></a><span data-ttu-id="73fda-109">职位在创建新员工时不显示</span><span class="sxs-lookup"><span data-stu-id="73fda-109">Position does not display when creating a new employee</span></span>

<span data-ttu-id="73fda-110">已经进行了更改来在 Talent 中招聘新员工时显示可用于分配的所有空缺职位。</span><span class="sxs-lookup"><span data-stu-id="73fda-110">A change has been made to display all open positions that are available for assignment when hiring new employees in Talent.</span></span> <span data-ttu-id="73fda-111">这包括历史职位或被设置了将来日期的职位。</span><span class="sxs-lookup"><span data-stu-id="73fda-111">This includes historical positions or if the postitions have been future dated.</span></span> <span data-ttu-id="73fda-112">职位现在将根据雇用开始日期正确显示。</span><span class="sxs-lookup"><span data-stu-id="73fda-112">Positions will now appear correctly based on the employment start date.</span></span> 

### <a name="termination-date-is-displaying-based-on-user-settings"></a><span data-ttu-id="73fda-113">终止雇用日期基于用户设置显示</span><span class="sxs-lookup"><span data-stu-id="73fda-113">Termination date is displaying based on user settings</span></span>

<span data-ttu-id="73fda-114">已对以往员工列表进行了更改来解释在查看终止雇用日期时员工首选时区的任何时区偏移。</span><span class="sxs-lookup"><span data-stu-id="73fda-114">A change has been made to the past employees list to account for any time zone offsets for the employees preferred time zone when viewing the termination date.</span></span>

### <a name="work-items-assigned-to-me-links-not-displaying-the-correct-information"></a><span data-ttu-id="73fda-115">分配给我的工作项链接不显示正确信息</span><span class="sxs-lookup"><span data-stu-id="73fda-115">Work items assigned to me links not displaying the correct information</span></span>

<span data-ttu-id="73fda-116">通过此更改，导航到列表中各个工作项的详细信息将显示所选项目的正确信息。</span><span class="sxs-lookup"><span data-stu-id="73fda-116">With this change, navigation to the details of the individual work items in the list will display the correct information for the item selected.</span></span> <span data-ttu-id="73fda-117">此问题只在高级安全选项中出现。</span><span class="sxs-lookup"><span data-stu-id="73fda-117">This issue only occurred with advanced security options.</span></span>


## <a name="known-issue"></a><span data-ttu-id="73fda-118">已知问题</span><span class="sxs-lookup"><span data-stu-id="73fda-118">Known issue</span></span>

- <span data-ttu-id="73fda-119">**问题**：在将新附件添加到工作人员时，**新建**和**编辑**按钮变灰。</span><span class="sxs-lookup"><span data-stu-id="73fda-119">**Issue**: When adding a new attachment to a worker, the **New** and **Edit** buttons are grayed out.</span></span> 
- <span data-ttu-id="73fda-120">**解决方法：** 打开附件页面之前，确保已关闭**工作人员**页面中的速见表。</span><span class="sxs-lookup"><span data-stu-id="73fda-120">**Workaround:** Before opening the attachment page, make sure that the FactBoxes on the **Worker** page are closed.</span></span> <span data-ttu-id="73fda-121">如果加载**工作人员**页面时速见表已关闭，将启用附件按钮。</span><span class="sxs-lookup"><span data-stu-id="73fda-121">If the FactBoxes are closed when the **Worker** page is loaded, the attachments buttons will be enabled.</span></span> <span data-ttu-id="73fda-122">（下一个平台更新中将解决这个问题。）</span><span class="sxs-lookup"><span data-stu-id="73fda-122">(This issue will be fixed in the next platform update.)</span></span>