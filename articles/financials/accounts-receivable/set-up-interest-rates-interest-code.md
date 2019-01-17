---
title: 为利息代码设置多种利率
description: 利息代码包含相关的设置利息时计费，以及如何在逾期科目计算。
author: ShivamPandey-msft
manager: AnnBe
ms.date: 01/12/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: Interest
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 59402
ms.assetid: 3b945333-1eaf-4658-ab5a-1a7791a7eb40
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 7748128099588182ae4f99077cd26f36fb330672
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56006"
---
# <a name="set-up-interest-rates-for-an-interest-code"></a><span data-ttu-id="90131-103">为利息代码设置多种利率</span><span class="sxs-lookup"><span data-stu-id="90131-103">Set up interest rates for an interest code</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="90131-104">利息代码包含相关的设置利息时计费，以及如何在逾期科目计算。</span><span class="sxs-lookup"><span data-stu-id="90131-104">Interest codes contain settings that determine when interest is charged and how it is calculated on overdue accounts.</span></span>

<span data-ttu-id="90131-105">您可以设置一个唯一利息代码和将它应用于多个客户过帐模板，计费代码，或者特定于发票行。</span><span class="sxs-lookup"><span data-stu-id="90131-105">You can set up a single interest code and apply it to multiple customer posting profiles, billing codes, or to specific invoice lines.</span></span> <span data-ttu-id="90131-106">在更改利息代码详细信息，使用该代码的所有功能将自动执行在新的交易记录的更改。</span><span class="sxs-lookup"><span data-stu-id="90131-106">When the interest code details are changed, all features that use the code will automatically implement the changes on new transactions.</span></span> <span data-ttu-id="90131-107">对于每个利息代码，您可以设置比率的两种类型:</span><span class="sxs-lookup"><span data-stu-id="90131-107">For each interest code, you can set up two types of rates:</span></span>
-   <span data-ttu-id="90131-108">利息收入-的汇率表示通过这些收取利息供在发票或利息单的收入。</span><span class="sxs-lookup"><span data-stu-id="90131-108">Rates for interest earnings − These represent revenue that is earned by charging interest on invoices or interest notes.</span></span>
-   <span data-ttu-id="90131-109">−这些付息的汇率表示为贷方通知单的利息支付的成本。</span><span class="sxs-lookup"><span data-stu-id="90131-109">Rates for interest payments − These represent a cost that is paid for interest on credit notes.</span></span>

<span data-ttu-id="90131-110">这两个成本率类型可能存在同时在同一和利息代码。</span><span class="sxs-lookup"><span data-stu-id="90131-110">Both of these rate types can exist at the same time and in the same interest code.</span></span> <span data-ttu-id="90131-111">可以基于从三种计算类型:</span><span class="sxs-lookup"><span data-stu-id="90131-111">Interest rates can be based on three calculation types:</span></span>
-   <span data-ttu-id="90131-112">利率。</span><span class="sxs-lookup"><span data-stu-id="90131-112">Interest by percentage.</span></span>
-   <span data-ttu-id="90131-113">利息金额。</span><span class="sxs-lookup"><span data-stu-id="90131-113">Interest by amount.</span></span>
-   <span data-ttu-id="90131-114">按范围的利息，将生成一个百分比或金额。</span><span class="sxs-lookup"><span data-stu-id="90131-114">Interest by range, which results in a single percentage or amount.</span></span>

<span data-ttu-id="90131-115">在计算利息时，为在付款超出了交易到期日期的时间段中生效的每个利率，都创建单独的利息单。</span><span class="sxs-lookup"><span data-stu-id="90131-115">When an interest code is used to calculate interest, a separate interest note is created for each interest rate that is in effect during the time that the payment has exceeded the transaction due date.</span></span> <span data-ttu-id="90131-116">您可以使用**利息代码**页上的**收入**选项卡为您通过收取利息获取的利息设置利率。</span><span class="sxs-lookup"><span data-stu-id="90131-116">You use the **Earnings** tab on the **Interest code** page to set up interest rates for interest that you earn by charging interest.</span></span> <span data-ttu-id="90131-117">使用**付款**选项卡可为您支付的利息设置利率。</span><span class="sxs-lookup"><span data-stu-id="90131-117">Use the **Payments** tab to set up interest rates for interest that you pay.</span></span>

## <a name="interest-rates-based-on-a-percentage"></a><span data-ttu-id="90131-118">基于百分比的利率</span><span class="sxs-lookup"><span data-stu-id="90131-118">Interest rates based on a percentage</span></span>
<span data-ttu-id="90131-119">您可以设置多种利率计算指定的百分比。</span><span class="sxs-lookup"><span data-stu-id="90131-119">You can set up interest rates that calculate a specified percentage.</span></span>

- <span data-ttu-id="90131-120">利息金额应用于所有币种。</span><span class="sxs-lookup"><span data-stu-id="90131-120">Interest amount applies to all currencies.</span></span>
- <span data-ttu-id="90131-121">可输入可选利息金额限制。</span><span class="sxs-lookup"><span data-stu-id="90131-121">Optional interest amount limits can be entered.</span></span>
- <span data-ttu-id="90131-122"><strong>设置利息代码</strong>页上的<strong>利息计算依据</strong>字段中已选择<strong>百分比</strong>。</span><span class="sxs-lookup"><span data-stu-id="90131-122"><strong>Percentage</strong> is selected\*\* <strong>in the \*\*Calculate interest based on</strong> field on the <strong>Set up Interest codes</strong> page.</span></span>

<span data-ttu-id="90131-123">例如，设置项目 5 的利息每两个月的利息代码发票付款超过交易到期日期，则在**计算利息间隔**字段中输入“2”，然后选择**月**。</span><span class="sxs-lookup"><span data-stu-id="90131-123">For example, to set up an interest code that assesses 5 percent interest for every two months that the invoice payment exceeds the transaction due date, you would enter 2 in the **Calculate interest every** field and select **Month**.</span></span>

## <a name="interest-rates-based-on-amounts"></a><span data-ttu-id="90131-124">基于金额的利率</span><span class="sxs-lookup"><span data-stu-id="90131-124">Interest rates based on amounts</span></span>
<span data-ttu-id="90131-125">您可以设置计算针对指定币种的利率金额。</span><span class="sxs-lookup"><span data-stu-id="90131-125">You can set up interest rates that calculate a specified amount per currency.</span></span>
- <span data-ttu-id="90131-126">为利息代码中的每个币种指定利息金额。</span><span class="sxs-lookup"><span data-stu-id="90131-126">An interest amount is specified for each currency in the interest code.</span></span>
- <span data-ttu-id="90131-127">可输入可选利息金额限制。</span><span class="sxs-lookup"><span data-stu-id="90131-127">Optional interest amount limits can be entered.</span></span>
- <span data-ttu-id="90131-128">**金额**是在**设置利息代码**页上的**利息计算依据**字段中选择的。</span><span class="sxs-lookup"><span data-stu-id="90131-128">**Amount** is selected in the **Calculate interest based on** field on the **Set up Interest codes** page.</span></span>

<span data-ttu-id="90131-129">例如，若要设置发票付款超过交易到期日期每 20 天的 25.00 的利息的利息代码，则在**计算利息间隔**字段中输入“20”，然后选择**天**。</span><span class="sxs-lookup"><span data-stu-id="90131-129">For example, to set up an interest code that assesses interest of 25.00 for every 20 days that the invoice payment exceeds the transaction due date, you would enter 20 in the **Calculate interest every** field and select **Day**.</span></span>

## <a name="interest-rates-based-on-ranges"></a><span data-ttu-id="90131-130">基于范围的利率</span><span class="sxs-lookup"><span data-stu-id="90131-130">Interest rates based on ranges</span></span>
<span data-ttu-id="90131-131">您可以设置根据逾期金额更改金额的利率，晚的天数，或金额晚的月份数。</span><span class="sxs-lookup"><span data-stu-id="90131-131">You can set up interest rates that vary depending on the overdue amount, the number of days that the amount is late, or the number of months that the amount is late.</span></span>
-   <span data-ttu-id="90131-132">您可以使用**原币收益**选项卡定义每个币种的特定利息设置。</span><span class="sxs-lookup"><span data-stu-id="90131-132">You can use the **Earnings by Currency** tab to define specific interest settings for each currency.</span></span> <span data-ttu-id="90131-133">这也是您要定义范围的位置。</span><span class="sxs-lookup"><span data-stu-id="90131-133">This is also where you will define the range.</span></span>
-   <span data-ttu-id="90131-134">使用**范围**按钮可添加表示您要设孩子的范围的行。</span><span class="sxs-lookup"><span data-stu-id="90131-134">Use the **Ranges** button to add lines that represent the ranges that you want to set up.</span></span> <span data-ttu-id="90131-135">**从**值表示该范围的开始，**利息值**数字表示百分比或金额，具体取决于**设置利息代码**页上的**利息计算依据**字段中的选择。</span><span class="sxs-lookup"><span data-stu-id="90131-135">The **From** value represents the beginning of the range and the **Interest value** number represents either a percentage or an amount, depending on the selection in the **Calculate interest based on** field on the **Set up Interest codes** page.</span></span>

## <a name="example-1-interest-by-range--amount"></a><span data-ttu-id="90131-136">示例 1：按大小的利息 = 金额</span><span class="sxs-lookup"><span data-stu-id="90131-136">Example 1: Interest by range = Amount</span></span>
<span data-ttu-id="90131-137">您设置估计利息一次每三个月的利息代码发票付款超过交易到期日期。</span><span class="sxs-lookup"><span data-stu-id="90131-137">You set up an interest code that assesses interest one time for every three months that the invoice payment exceeds the transaction due date.</span></span> <span data-ttu-id="90131-138">要基于计算利息百分比值，根据步骤的金额间隔。</span><span class="sxs-lookup"><span data-stu-id="90131-138">You want to base the calculation on a percentage interest value, according to stepped amount intervals.</span></span> <span data-ttu-id="90131-139">利息值将与发票金额的 1 金额的 1,000.00，从 1,001.00 到 2 的金额的 5,000.00 和 3，超过 5,000.00。</span><span class="sxs-lookup"><span data-stu-id="90131-139">The interest value will be 1 percent for invoice amounts up to 1,000.00, 2 percent for amounts from 1,001.00 to 5,000.00, and 3 percent for amounts larger than 5,000.00.</span></span> <span data-ttu-id="90131-140">您为利息代码设置了字段的值。</span><span class="sxs-lookup"><span data-stu-id="90131-140">You set up the interest code field values as follows.</span></span>

| <span data-ttu-id="90131-141">**字段名称**</span><span class="sxs-lookup"><span data-stu-id="90131-141">**Field name**</span></span>                  | <span data-ttu-id="90131-142">**字段值**</span><span class="sxs-lookup"><span data-stu-id="90131-142">**Field value**</span></span> |
|---------------------------------|-----------------|
| <span data-ttu-id="90131-143">**利息代码**</span><span class="sxs-lookup"><span data-stu-id="90131-143">**Interest code**</span></span>               | <span data-ttu-id="90131-144">3M%ByAmt</span><span class="sxs-lookup"><span data-stu-id="90131-144">3M%ByAmt</span></span>        |
| <span data-ttu-id="90131-145">**计算利息间隔**</span><span class="sxs-lookup"><span data-stu-id="90131-145">**Calculate interest every**</span></span>    | <span data-ttu-id="90131-146">3/月</span><span class="sxs-lookup"><span data-stu-id="90131-146">3/Month</span></span>         |
| <span data-ttu-id="90131-147">**按范围的利息**</span><span class="sxs-lookup"><span data-stu-id="90131-147">**Interest by range**</span></span>           | <span data-ttu-id="90131-148">金额</span><span class="sxs-lookup"><span data-stu-id="90131-148">Amount</span></span>          |
| <span data-ttu-id="90131-149">**利息计算依据**</span><span class="sxs-lookup"><span data-stu-id="90131-149">**Calculate interest based on**</span></span> | <span data-ttu-id="90131-150">百分比</span><span class="sxs-lookup"><span data-stu-id="90131-150">Percentage</span></span>      |

<span data-ttu-id="90131-151">您按如下所示设置了范围信息。</span><span class="sxs-lookup"><span data-stu-id="90131-151">You set up the range information as follows.</span></span>

| <span data-ttu-id="90131-152">**源值**</span><span class="sxs-lookup"><span data-stu-id="90131-152">**From value**</span></span> | <span data-ttu-id="90131-153">**利息值**</span><span class="sxs-lookup"><span data-stu-id="90131-153">**Interest value**</span></span> |
|----------------|--------------------|
| <span data-ttu-id="90131-154">0</span><span class="sxs-lookup"><span data-stu-id="90131-154">0</span></span>              | <span data-ttu-id="90131-155">1</span><span class="sxs-lookup"><span data-stu-id="90131-155">1</span></span>                  |
| <span data-ttu-id="90131-156">1,001</span><span class="sxs-lookup"><span data-stu-id="90131-156">1,001</span></span>          | <span data-ttu-id="90131-157">2</span><span class="sxs-lookup"><span data-stu-id="90131-157">2</span></span>                  |
| <span data-ttu-id="90131-158">5,001</span><span class="sxs-lookup"><span data-stu-id="90131-158">5,001</span></span>          | <span data-ttu-id="90131-159">3</span><span class="sxs-lookup"><span data-stu-id="90131-159">3</span></span>                  |


## <a name="example-2-interest-by-range--days"></a><span data-ttu-id="90131-160">示例 2：按大小的利息 = 天</span><span class="sxs-lookup"><span data-stu-id="90131-160">Example 2: Interest by range = Days</span></span>
--------------------------------------------------

<span data-ttu-id="90131-161">您设置发票付款超过交易到期日期每 15 天估计一次利息的利息代码。</span><span class="sxs-lookup"><span data-stu-id="90131-161">You set up an interest code that assesses interest one time for every 15 days that the invoice payment exceeds the transaction due date.</span></span> <span data-ttu-id="90131-162">要基于计算利息百分比值，根据步骤的金额间隔。</span><span class="sxs-lookup"><span data-stu-id="90131-162">You want to base the calculation on an amount interest value, according to stepped day intervals.</span></span> <span data-ttu-id="90131-163">在过去 60 天以来，利息值将为 10.00 (每 15 天，在每 15.00 天 61 到 90 和 20.00 个期间的 15 天，从第 91 天的 15 天前和之后。</span><span class="sxs-lookup"><span data-stu-id="90131-163">The interest value will be 10.00 per 15 days during the first 60 days, 15.00 per 15 days during days 61 to 90, and 20.00 per 15 days from day 91 and after.</span></span> <span data-ttu-id="90131-164">您为利息代码设置了字段的值。</span><span class="sxs-lookup"><span data-stu-id="90131-164">You set up the interest code field values as follows.</span></span>

| <span data-ttu-id="90131-165">**字段名称**</span><span class="sxs-lookup"><span data-stu-id="90131-165">**Field name**</span></span>                  | <span data-ttu-id="90131-166">**字段值**</span><span class="sxs-lookup"><span data-stu-id="90131-166">**Field value**</span></span> |
|---------------------------------|-----------------|
| <span data-ttu-id="90131-167">**利息代码**</span><span class="sxs-lookup"><span data-stu-id="90131-167">**Interest code**</span></span>               | <span data-ttu-id="90131-168">15DAmtXDay</span><span class="sxs-lookup"><span data-stu-id="90131-168">15DAmtXDay</span></span>      |
| <span data-ttu-id="90131-169">**计算利息间隔**</span><span class="sxs-lookup"><span data-stu-id="90131-169">**Calculate interest every**</span></span>    | <span data-ttu-id="90131-170">15/天</span><span class="sxs-lookup"><span data-stu-id="90131-170">15/Day</span></span>          |
| <span data-ttu-id="90131-171">**按范围的利息**</span><span class="sxs-lookup"><span data-stu-id="90131-171">**Interest by range**</span></span>           | <span data-ttu-id="90131-172">天</span><span class="sxs-lookup"><span data-stu-id="90131-172">Days</span></span>            |
| <span data-ttu-id="90131-173">**利息计算依据**</span><span class="sxs-lookup"><span data-stu-id="90131-173">**Calculate interest based on**</span></span> | <span data-ttu-id="90131-174">金额</span><span class="sxs-lookup"><span data-stu-id="90131-174">Amount</span></span>          |

<span data-ttu-id="90131-175">您按如下所示设置了范围信息。</span><span class="sxs-lookup"><span data-stu-id="90131-175">You set up the range information as follows.</span></span>

| <span data-ttu-id="90131-176">**源值**</span><span class="sxs-lookup"><span data-stu-id="90131-176">**From value**</span></span> | <span data-ttu-id="90131-177">**利息值**</span><span class="sxs-lookup"><span data-stu-id="90131-177">**Interest value**</span></span> |
|----------------|--------------------|
| <span data-ttu-id="90131-178">0</span><span class="sxs-lookup"><span data-stu-id="90131-178">0</span></span>              | <span data-ttu-id="90131-179">10</span><span class="sxs-lookup"><span data-stu-id="90131-179">10</span></span>                 |
| <span data-ttu-id="90131-180">61</span><span class="sxs-lookup"><span data-stu-id="90131-180">61</span></span>             | <span data-ttu-id="90131-181">15</span><span class="sxs-lookup"><span data-stu-id="90131-181">15</span></span>                 |
| <span data-ttu-id="90131-182">91</span><span class="sxs-lookup"><span data-stu-id="90131-182">91</span></span>             | <span data-ttu-id="90131-183">20</span><span class="sxs-lookup"><span data-stu-id="90131-183">20</span></span>                 |


## <a name="example-3-interest-by-range--months"></a><span data-ttu-id="90131-184">示例 3：按大小的利息 = 月</span><span class="sxs-lookup"><span data-stu-id="90131-184">Example 3: Interest by range = Months</span></span>
----------------------------------------------------

<span data-ttu-id="90131-185">您设置估计利息一次每三个月的利息代码发票付款超过交易到期日期。</span><span class="sxs-lookup"><span data-stu-id="90131-185">You set up an interest code that assesses interest one time for every month that the invoice payment exceeds the transaction due date.</span></span> <span data-ttu-id="90131-186">要基于计算利息百分比值，根据步骤的金额间隔。</span><span class="sxs-lookup"><span data-stu-id="90131-186">You want to base the calculation on a percentage interest value, according to stepped month intervals.</span></span> <span data-ttu-id="90131-187">对于前三个月逾期，利息值将为每月 1.5%，对于第二个三个月逾期，为每月 2.0%，对于超出前六个月之外的每个月，为每月 2.5%。</span><span class="sxs-lookup"><span data-stu-id="90131-187">The interest value will be 1.5 percent per month for the first three overdue months, 2.0 percent per month for the second three months, and 2.5 percent per month for each month beyond the first six months.</span></span> <span data-ttu-id="90131-188">您为利息代码设置了字段的值。</span><span class="sxs-lookup"><span data-stu-id="90131-188">You set up the interest code field values as follows.</span></span>

| <span data-ttu-id="90131-189">**字段名称**</span><span class="sxs-lookup"><span data-stu-id="90131-189">**Field name**</span></span>                  | <span data-ttu-id="90131-190">**字段值**</span><span class="sxs-lookup"><span data-stu-id="90131-190">**Field value**</span></span> |
|---------------------------------|-----------------|
| <span data-ttu-id="90131-191">**利息代码**</span><span class="sxs-lookup"><span data-stu-id="90131-191">**Interest code**</span></span>               | <span data-ttu-id="90131-192">1M%ByMth</span><span class="sxs-lookup"><span data-stu-id="90131-192">1M%ByMth</span></span>        |
| <span data-ttu-id="90131-193">**计算利息间隔**</span><span class="sxs-lookup"><span data-stu-id="90131-193">**Calculate interest every**</span></span>    | <span data-ttu-id="90131-194">1/月</span><span class="sxs-lookup"><span data-stu-id="90131-194">1/Month</span></span>         |
| <span data-ttu-id="90131-195">**按范围的利息**</span><span class="sxs-lookup"><span data-stu-id="90131-195">**Interest by range**</span></span>           | <span data-ttu-id="90131-196">月份</span><span class="sxs-lookup"><span data-stu-id="90131-196">Months</span></span>          |
| <span data-ttu-id="90131-197">**利息计算依据**</span><span class="sxs-lookup"><span data-stu-id="90131-197">**Calculate interest based on**</span></span> | <span data-ttu-id="90131-198">百分比</span><span class="sxs-lookup"><span data-stu-id="90131-198">Percentage</span></span>      |

<span data-ttu-id="90131-199">您按如下所示设置了范围信息。</span><span class="sxs-lookup"><span data-stu-id="90131-199">You set up the range information as follows.</span></span>

| <span data-ttu-id="90131-200">**源值**</span><span class="sxs-lookup"><span data-stu-id="90131-200">**From value**</span></span> | <span data-ttu-id="90131-201">**利息值**</span><span class="sxs-lookup"><span data-stu-id="90131-201">**Interest value**</span></span> |
|----------------|--------------------|
| <span data-ttu-id="90131-202">0</span><span class="sxs-lookup"><span data-stu-id="90131-202">0</span></span>              | <span data-ttu-id="90131-203">1.5</span><span class="sxs-lookup"><span data-stu-id="90131-203">1.5</span></span>                |
| <span data-ttu-id="90131-204">4</span><span class="sxs-lookup"><span data-stu-id="90131-204">4</span></span>              | <span data-ttu-id="90131-205">2</span><span class="sxs-lookup"><span data-stu-id="90131-205">2</span></span>                  |
| <span data-ttu-id="90131-206">7</span><span class="sxs-lookup"><span data-stu-id="90131-206">7</span></span>              | <span data-ttu-id="90131-207">2.5</span><span class="sxs-lookup"><span data-stu-id="90131-207">2.5</span></span>                |

## <a name="new-versions"></a><span data-ttu-id="90131-208">新版本</span><span class="sxs-lookup"><span data-stu-id="90131-208">New versions</span></span>
<span data-ttu-id="90131-209">利息代码是有生效日期的。</span><span class="sxs-lookup"><span data-stu-id="90131-209">Interest codes are date effective.</span></span> <span data-ttu-id="90131-210">如果您要修改利率，您可以创建截至将来日期生效的**新版本**。</span><span class="sxs-lookup"><span data-stu-id="90131-210">If you want to modify the interest rate, you can create a **new version** that is effective as of a future date.</span></span>

<span data-ttu-id="90131-211">若要查看不同的版本，您可以使用**开始日期**菜单选项来选择截止日期。</span><span class="sxs-lookup"><span data-stu-id="90131-211">To view different versions, you can use the **As of Date** menu choice to select the cutoff date.</span></span> <span data-ttu-id="90131-212">您还可以选择**显示所有记录**来查看该页中的所有利息代码。</span><span class="sxs-lookup"><span data-stu-id="90131-212">You can also select the **Display all records** to view all interest codes in the page.</span></span>


