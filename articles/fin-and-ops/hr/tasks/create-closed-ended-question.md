---
title: 创建封闭式问题
description: 封闭式问题允许您为回答者提供供选择的选项。
author: kherr75
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: KMAnswerCollection, KMAnswer, KMQuestion
audience: Application User
ms.reviewer: rschloma
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: kherr
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 3b9745474f337799b48bc2eee6d75bda1d61ac84
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55083"
---
# <a name="create-a-closed-ended-question"></a><span data-ttu-id="06bcd-103">创建封闭式问题</span><span class="sxs-lookup"><span data-stu-id="06bcd-103">Create a closed ended question</span></span>

[!include [task guide banner](../../includes/task-guide-banner.md)]

<span data-ttu-id="06bcd-104">封闭式问题允许您为回答者提供供选择的选项。</span><span class="sxs-lookup"><span data-stu-id="06bcd-104">Closed-ended questions allow you to provide options for the respondent to choose from.</span></span> <span data-ttu-id="06bcd-105">首先，您需要创建有回答的回答组，然后创建使用该回答组的问题。</span><span class="sxs-lookup"><span data-stu-id="06bcd-105">First, you need to create the Answer group with the answers, then create the question that will use the answer group.</span></span> <span data-ttu-id="06bcd-106">创建此程序的演示数据公司是 USMF。</span><span class="sxs-lookup"><span data-stu-id="06bcd-106">The demo data company used to create this procedure is USMF.</span></span>


## <a name="create-an-answer-group"></a><span data-ttu-id="06bcd-107">创建回答组</span><span class="sxs-lookup"><span data-stu-id="06bcd-107">Create an answer group</span></span>
1. <span data-ttu-id="06bcd-108">转到“调查表”>“设计”>“回答组”。</span><span class="sxs-lookup"><span data-stu-id="06bcd-108">Go to Questionnaire > Design > Answer groups.</span></span>
2. <span data-ttu-id="06bcd-109">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="06bcd-109">Click New.</span></span>
3. <span data-ttu-id="06bcd-110">在“回答组”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="06bcd-110">In the Answer group field, type a value.</span></span>
4. <span data-ttu-id="06bcd-111">在“描述”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="06bcd-111">In the Description field, type a value.</span></span>
    * <span data-ttu-id="06bcd-112">每次将回答组用于问题时，使用随机功能以随机在不同订单中设置回答。</span><span class="sxs-lookup"><span data-stu-id="06bcd-112">Use the Randomize functionality to randomly place the answers in a different order each time the answer group is used for a question.</span></span>  
5. <span data-ttu-id="06bcd-113">单击“回答”。</span><span class="sxs-lookup"><span data-stu-id="06bcd-113">Click Answer.</span></span>
6. <span data-ttu-id="06bcd-114">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="06bcd-114">Click New.</span></span>
    * <span data-ttu-id="06bcd-115">序列号控制回答显示的顺序，除非回答组已选择“随机”。</span><span class="sxs-lookup"><span data-stu-id="06bcd-115">Sequence number controls the order in which the answers are displayed, unless Randomize is selected for the Answer group.</span></span>  
    * <span data-ttu-id="06bcd-116">可规定回答项分数，以对调查表进行评分。</span><span class="sxs-lookup"><span data-stu-id="06bcd-116">Points can be awarded to answers for use in scoring the questionnaire.</span></span>  
7. <span data-ttu-id="06bcd-117">在“分数”字段中，输入一个数字。</span><span class="sxs-lookup"><span data-stu-id="06bcd-117">In the Points field, enter a number.</span></span>
    * <span data-ttu-id="06bcd-118">可以标记正确答案，以指示所选答案正确。</span><span class="sxs-lookup"><span data-stu-id="06bcd-118">The correct answer can be marked to indicate that the selected answer is the correct one.</span></span> <span data-ttu-id="06bcd-119">这可用于对调查表进行评分。</span><span class="sxs-lookup"><span data-stu-id="06bcd-119">This can be used for scoring the questionnaire.</span></span>  
8. <span data-ttu-id="06bcd-120">在“回答”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="06bcd-120">In the Answer field, type a value.</span></span>
    * <span data-ttu-id="06bcd-121">继续为回答组创建回答选项。</span><span class="sxs-lookup"><span data-stu-id="06bcd-121">Continue to create answer selection options for the answer group.</span></span>  
9. <span data-ttu-id="06bcd-122">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="06bcd-122">Click New.</span></span>
10. <span data-ttu-id="06bcd-123">在“分数”字段中，输入一个数字。</span><span class="sxs-lookup"><span data-stu-id="06bcd-123">In the Points field, enter a number.</span></span>
11. <span data-ttu-id="06bcd-124">在“回答”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="06bcd-124">In the Answer field, type a value.</span></span>
12. <span data-ttu-id="06bcd-125">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="06bcd-125">Click New.</span></span>
13. <span data-ttu-id="06bcd-126">在“分数”字段中，输入一个数字。</span><span class="sxs-lookup"><span data-stu-id="06bcd-126">In the Points field, enter a number.</span></span>
14. <span data-ttu-id="06bcd-127">在“回答”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="06bcd-127">In the Answer field, type a value.</span></span>
15. <span data-ttu-id="06bcd-128">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="06bcd-128">Click New.</span></span>
16. <span data-ttu-id="06bcd-129">在“分数”字段中，输入一个数字。</span><span class="sxs-lookup"><span data-stu-id="06bcd-129">In the Points field, enter a number.</span></span>
17. <span data-ttu-id="06bcd-130">在“回答”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="06bcd-130">In the Answer field, type a value.</span></span>
18. <span data-ttu-id="06bcd-131">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="06bcd-131">Click New.</span></span>
19. <span data-ttu-id="06bcd-132">在“分数”字段中，输入一个数字。</span><span class="sxs-lookup"><span data-stu-id="06bcd-132">In the Points field, enter a number.</span></span>
20. <span data-ttu-id="06bcd-133">在“回答”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="06bcd-133">In the Answer field, type a value.</span></span>
21. <span data-ttu-id="06bcd-134">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="06bcd-134">Close the page.</span></span>
22. <span data-ttu-id="06bcd-135">关闭该页面。</span><span class="sxs-lookup"><span data-stu-id="06bcd-135">Close the page.</span></span>

## <a name="create-the-question"></a><span data-ttu-id="06bcd-136">创建问题</span><span class="sxs-lookup"><span data-stu-id="06bcd-136">Create the question</span></span>
1. <span data-ttu-id="06bcd-137">转到“调查表”>“设计”>“问题”。</span><span class="sxs-lookup"><span data-stu-id="06bcd-137">Go to Questionnaire > Design > Questions.</span></span>
2. <span data-ttu-id="06bcd-138">单击“新建”。</span><span class="sxs-lookup"><span data-stu-id="06bcd-138">Click New.</span></span>
3. <span data-ttu-id="06bcd-139">使用“类型”字段，以将相关问题分组。</span><span class="sxs-lookup"><span data-stu-id="06bcd-139">Use the Type field to group related questions together.</span></span>
    * <span data-ttu-id="06bcd-140">您可以选择输入类型：复选框、备选按钮或封闭式问题的组合框。</span><span class="sxs-lookup"><span data-stu-id="06bcd-140">You can use input types of Check box, Alternative button, or Combo box for closed-ended questions.</span></span>  
4. <span data-ttu-id="06bcd-141">在“输入类型”字段中，选择一个选项。</span><span class="sxs-lookup"><span data-stu-id="06bcd-141">In the Input type field, select an option.</span></span>
5. <span data-ttu-id="06bcd-142">在“回答组”字段中，输入或选择一个值。</span><span class="sxs-lookup"><span data-stu-id="06bcd-142">In the Answer group field, enter or select a value.</span></span>
6. <span data-ttu-id="06bcd-143">在“文本”字段中，键入一个值。</span><span class="sxs-lookup"><span data-stu-id="06bcd-143">In the Text field, type a value.</span></span>

