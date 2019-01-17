---
title: 高级筛选和查询语法
description: 本文介绍在“过滤器”窗格或网格列标题过滤器中使用“高级过滤器/排序”对话框或**匹配**运算符时的可用过滤和查询选项。
author: jasongre
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysQueryForm
audience: Application User
ms.reviewer: sericks
ms.search.scope: Core, Operations
ms.custom: 3811
ms.assetid: b4969b30-2fe1-4a3c-bbea-725dc37c8b60
ms.search.region: Global
ms.author: jasongre
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: a17f6f20e7ee08519211490487b441d8456201f7
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56151"
---
# <a name="advanced-filtering-and-query-syntax"></a><span data-ttu-id="b2cf5-103">高级筛选和查询语法</span><span class="sxs-lookup"><span data-stu-id="b2cf5-103">Advanced filtering and query syntax</span></span>

[!include [banner](../includes/banner.md)]

<span data-ttu-id="b2cf5-104">本文介绍在“过滤器”窗格或网格列标题过滤器中使用“高级过滤器/排序”对话框或**匹配**运算符时的可用过滤和查询选项。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-104">This article describes the filtering and query options that are available when you use the Advanced filter/sort dialog or the **matches** operator in the Filter pane or grid column header filters.</span></span> 

<a name="advanced-query-syntax"></a><span data-ttu-id="b2cf5-105">高级查询语法</span><span class="sxs-lookup"><span data-stu-id="b2cf5-105">Advanced query syntax</span></span>
---------------------

<table>
<colgroup>
<col width="25%" />
<col width="25%" />
<col width="25%" />
<col width="25%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b2cf5-106">语法</span><span class="sxs-lookup"><span data-stu-id="b2cf5-106">Syntax</span></span></th>
<th><span data-ttu-id="b2cf5-107">字符描述</span><span class="sxs-lookup"><span data-stu-id="b2cf5-107">Character description</span></span></th>
<th><span data-ttu-id="b2cf5-108">说明</span><span class="sxs-lookup"><span data-stu-id="b2cf5-108">Description</span></span></th>
<th><span data-ttu-id="b2cf5-109">示例</span><span class="sxs-lookup"><span data-stu-id="b2cf5-109">Example</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b2cf5-110"><em>值</em></span><span class="sxs-lookup"><span data-stu-id="b2cf5-110"><em>value</em></span></span></td>
<td><span data-ttu-id="b2cf5-111">等于输入的值</span><span class="sxs-lookup"><span data-stu-id="b2cf5-111">Equal to the value that is entered</span></span></td>
<td><span data-ttu-id="b2cf5-112">键入要查找的该值。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-112">Type the value to find.</span></span></td>
<td><span data-ttu-id="b2cf5-113"><strong>Smith</strong> 查找 &quot;Smith&quot;。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-113"><strong>Smith</strong> finds &quot;Smith&quot;.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b2cf5-114">!<em>值</em>（感叹号）</span><span class="sxs-lookup"><span data-stu-id="b2cf5-114">!<em>value</em> (exclamation point)</span></span></td>
<td><span data-ttu-id="b2cf5-115">不等于输入的值</span><span class="sxs-lookup"><span data-stu-id="b2cf5-115">Not equal to the value that is entered</span></span></td>
<td><span data-ttu-id="b2cf5-116">键入一个惊叹号，然后是要排除的值。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-116">Type an exclamation point and then the value to exclude.</span></span></td>
<td><span data-ttu-id="b2cf5-117"><strong>!Smith</strong> 查找除 &quot;Smith&quot; 之外的所有值。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-117"><strong>!Smith</strong> finds all values except &quot;Smith&quot;.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b2cf5-118"><em>开始值</em>..<em>结束值</em>（双句点）</span><span class="sxs-lookup"><span data-stu-id="b2cf5-118"><em>from-value</em>..<em>to-value</em> (double period)</span></span></td>
<td><span data-ttu-id="b2cf5-119">用双句点分隔的两个值之间</span><span class="sxs-lookup"><span data-stu-id="b2cf5-119">Between the two values that are separated by double periods</span></span></td>
<td><span data-ttu-id="b2cf5-120">键入开始值，然后是两个句点，最后键入结束值。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-120">Type the from-value, then two periods, and then the to-value.</span></span></td>
<td><span data-ttu-id="b2cf5-121"><strong>1..10</strong> 查找从 1 到 10 的所有值。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-121"><strong>1..10</strong> finds all values from 1 through 10.</span></span> <span data-ttu-id="b2cf5-122">不过，在字符串字段中，<strong>A..C</strong> 将查找以 &quot;A&quot; 开头和以 &quot;B&quot; 开头的所有值以及恰好为 &quot;C&quot; 的值。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-122">However, in a string field, <strong>A..C</strong> finds all values that start with &quot;A&quot; and &quot;B&quot;, and values that are exactly equal to &quot;C&quot;.</span></span> <span data-ttu-id="b2cf5-123">例如，此查询不会查找 &quot;Ca&quot;。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-123">For example, this query won&#39;t find &quot;Ca&quot;.</span></span> <span data-ttu-id="b2cf5-124">若要查找从 &quot;A<em>&quot; 到 &quot;C</em>&quot; 的所有值，请键入 <strong>A..D</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-124">To find all values from &quot;A<em>&quot; through &quot;C</em>&quot;, type <strong>A..D</strong>.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b2cf5-125">..<em>值</em>（双句点）</span><span class="sxs-lookup"><span data-stu-id="b2cf5-125">..<em>value</em> (double period)</span></span></td>
<td><span data-ttu-id="b2cf5-126">小于或等于输入的值</span><span class="sxs-lookup"><span data-stu-id="b2cf5-126">Less than or equal to the value that is entered</span></span></td>
<td><span data-ttu-id="b2cf5-127">键入两个句点，然后键入值。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-127">Type two periods and then the value.</span></span></td>
<td><span data-ttu-id="b2cf5-128"><strong>..1000</strong> 查找小于或等于 1000 的任何数字，例如 &quot;100&quot;、&quot;999.95&quot; 和 &quot;1,000&quot;。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-128"><strong>..1000</strong> finds any number that is less than or equal to 1000, such as &quot;100&quot;, &quot;999.95&quot;, and &quot;1,000&quot;.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b2cf5-129"><em>值</em>..</span><span class="sxs-lookup"><span data-stu-id="b2cf5-129"><em>value</em>..</span></span> <span data-ttu-id="b2cf5-130">（双句点）</span><span class="sxs-lookup"><span data-stu-id="b2cf5-130">(double period)</span></span></td>
<td><span data-ttu-id="b2cf5-131">大于或等于输入的值</span><span class="sxs-lookup"><span data-stu-id="b2cf5-131">Greater than or equal to the value that is entered</span></span></td>
<td><span data-ttu-id="b2cf5-132">键入值，然后键入两个句点。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-132">Type the value and then two periods.</span></span></td>
<td><span data-ttu-id="b2cf5-133"><strong>1000..</strong></span><span class="sxs-lookup"><span data-stu-id="b2cf5-133"><strong>1000..</strong></span></span> <span data-ttu-id="b2cf5-134">查找大于或等于 1000 的任何数字，例如 &quot;1,000&quot;、&quot;1,000.01&quot; 和 &quot;1,000,000&quot;。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-134">finds any number that is greater than or equal to 1000, such as &quot;1,000&quot;, &quot;1,000.01&quot;, and &quot;1,000,000&quot;.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b2cf5-135">&gt;<em>值</em>（大于符号）</span><span class="sxs-lookup"><span data-stu-id="b2cf5-135">&gt;<em>value</em> (greater than sign)</span></span></td>
<td><span data-ttu-id="b2cf5-136">大于输入的值</span><span class="sxs-lookup"><span data-stu-id="b2cf5-136">Greater than the value that is entered</span></span></td>
<td><span data-ttu-id="b2cf5-137">键入大于符号 (<strong>&gt;</strong>)，然后键入值。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-137">Type a greater than sign (<strong>&gt;</strong>) and then the value.</span></span></td>
<td><span data-ttu-id="b2cf5-138"><strong>&gt;1000</strong> 查找大于 1000 的任何数字，例如 &quot;1000.01&quot;、&quot;20,000&quot; 和 &quot;1,000,000&quot;。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-138"><strong>&gt;1000</strong> finds any number that is greater than 1000, such as &quot;1000.01&quot;, &quot;20,000&quot;, and &quot;1,000,000&quot;.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b2cf5-139">&lt;<em>值</em>（小于符号）</span><span class="sxs-lookup"><span data-stu-id="b2cf5-139">&lt;<em>value</em> (less than sign)</span></span></td>
<td><span data-ttu-id="b2cf5-140">小于输入的值</span><span class="sxs-lookup"><span data-stu-id="b2cf5-140">Less than the value that is entered</span></span></td>
<td><span data-ttu-id="b2cf5-141">键入小于符号 (<strong>&lt;</strong>)，然后键入值。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-141">Type a less than sign (<strong>&lt;</strong>) and then the value.</span></span></td>
<td><span data-ttu-id="b2cf5-142"><strong>&lt;1000</strong> 查找小于 1000 的任何数字，例如 &quot;999.99&quot;、&quot;1&quot; 和 &quot;-200&quot;。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-142"><strong>&lt;1000</strong> finds any number that is less than 1000, such as &quot;999.99&quot;, &quot;1&quot;, and &quot;-200&quot;.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b2cf5-143"><em>值</em>\*（星号）</span><span class="sxs-lookup"><span data-stu-id="b2cf5-143"><em>value</em>\* (asterisk)</span></span></td>
<td><span data-ttu-id="b2cf5-144">以输入的值开头</span><span class="sxs-lookup"><span data-stu-id="b2cf5-144">Starting from the value that is entered</span></span></td>
<td><span data-ttu-id="b2cf5-145">键入字符串值，然后键入星号 (<strong><em></strong>)。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-145">Type the starting value and then an asterisk (<strong><em></strong>).</span></span></td>
<td><span data-ttu-id="b2cf5-146"><strong>S</em></strong> 查找以“S”开头的任何字符串，例如“Stockholm”、“Sydney”和“San Francisco”。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-146"><strong>S</em></strong> finds any string that starts with &quot;S&quot;, such as &quot;Stockholm&quot;, &quot;Sydney&quot;, and &quot;San Francisco&quot;.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b2cf5-147"><em><em>值</em>（星号）</span><span class="sxs-lookup"><span data-stu-id="b2cf5-147"><em><em>value</em> (asterisk)</span></span></td>
<td><span data-ttu-id="b2cf5-148">以输入的值结尾</span><span class="sxs-lookup"><span data-stu-id="b2cf5-148">Ending with the value that is entered</span></span></td>
<td><span data-ttu-id="b2cf5-149">键入星号，然后键入结尾值。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-149">Type an asterisk and then the ending value.</span></span></td>
<td><span data-ttu-id="b2cf5-150"><strong></em>east</strong> 查找以“east”结尾的任何字符串，例如“Northeast”和“Southeast”。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-150"><strong></em>east</strong> finds any string that ends with &quot;east&quot;, such as &quot;Northeast&quot; and &quot;Southeast&quot;.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b2cf5-151"><em><em>值</em></em>（星号）</span><span class="sxs-lookup"><span data-stu-id="b2cf5-151"><em><em>value</em></em> (asterisk)</span></span></td>
<td><span data-ttu-id="b2cf5-152">包含输入的值</span><span class="sxs-lookup"><span data-stu-id="b2cf5-152">Containing the value that is entered</span></span></td>
<td><span data-ttu-id="b2cf5-153">键入星号，然后键入值，再键入另一个星号。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-153">Type an asterisk, then a value, and then another asterisk.</span></span></td>
<td><span data-ttu-id="b2cf5-154"><strong><em>th</em></strong>查找包含 &quot;th&quot; 的任何字符串，例如 &quot;Northeast&quot; 和 &quot;Southeast&quot;。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-154"><strong><em>th</em></strong> finds any string that contains &quot;th&quot;, such as &quot;Northeast&quot; and &quot;Southeast&quot;.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b2cf5-155">?</span><span class="sxs-lookup"><span data-stu-id="b2cf5-155">?</span></span> <span data-ttu-id="b2cf5-156">（问号）</span><span class="sxs-lookup"><span data-stu-id="b2cf5-156">(question mark)</span></span></td>
<td><span data-ttu-id="b2cf5-157">具有一个或多个未知字符</span><span class="sxs-lookup"><span data-stu-id="b2cf5-157">Having one or more unknown characters</span></span></td>
<td><span data-ttu-id="b2cf5-158">在值中未知字符的位置键入一个问号。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-158">Type a question mark at the position of the unknown character in the value.</span></span></td>
<td><span data-ttu-id="b2cf5-159"><strong>Sm?th</strong> 查找 &quot;Smith&quot; 和 &quot;Smyth&quot;。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-159"><strong>Sm?th</strong> finds &quot;Smith&quot; and &quot;Smyth&quot;.</span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b2cf5-160"><em>值</em>,<em>值</em>（逗号）</span><span class="sxs-lookup"><span data-stu-id="b2cf5-160"><em>value</em>,<em>value</em> (comma)</span></span></td>
<td><span data-ttu-id="b2cf5-161">匹配用逗号分隔的值</span><span class="sxs-lookup"><span data-stu-id="b2cf5-161">Matching the values that are separated by commas</span></span></td>
<td><span data-ttu-id="b2cf5-162">键入所有条件，用逗号分隔。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-162">Type all your criteria, and separate them by using commas.</span></span></td>
<td><span data-ttu-id="b2cf5-163"><strong>A, D, F, G</strong> 精确查找 &quot;A&quot;、&quot;D&quot;、&quot;F&quot; 和 &quot;G&quot;。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-163"><strong>A, D, F, G</strong> finds exactly &quot;A&quot;, &quot;D&quot;, &quot;F&quot;, and &quot;G&quot;.</span></span> <span data-ttu-id="b2cf5-164"><strong>10, 20, 30, 100</strong> 精确查找 &quot;10、20、30、100&quot;。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-164"><strong>10, 20, 30, 100</strong> finds exactly &quot;10, 20, 30, 100&quot;.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b2cf5-165">（<span class="code">SQL 语句</span>）（括号间的 SQL 语句）</span><span class="sxs-lookup"><span data-stu-id="b2cf5-165">(<span class="code">SQL statement</span>) (SQL statement between parentheses)</span></span></td>
<td><span data-ttu-id="b2cf5-166">匹配定义的查询</span><span class="sxs-lookup"><span data-stu-id="b2cf5-166">Matching a defined query</span></span></td>
<td><span data-ttu-id="b2cf5-167">在括号间键入查询，作为 SQL 语句。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-167">Type a query as an SQL statement between parentheses.</span></span></td>
<td><span data-ttu-id="b2cf5-168"><strong><span class="code">(data source.Fieldname != &quot;A&quot;)</span></strong></span><span class="sxs-lookup"><span data-stu-id="b2cf5-168"><strong><span class="code">(data source.Fieldname != &quot;A&quot;)</span></strong></span></span></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b2cf5-169">T</span><span class="sxs-lookup"><span data-stu-id="b2cf5-169">T</span></span></td>
<td><span data-ttu-id="b2cf5-170">今天的日期</span><span class="sxs-lookup"><span data-stu-id="b2cf5-170">Today&#39;s date</span></span></td>
<td><span data-ttu-id="b2cf5-171">类型 <strong>T</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-171">Type <strong>T</strong>.</span></span></td>
<td><span data-ttu-id="b2cf5-172"><strong>T</strong> 匹配今天的日期。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-172"><strong>T</strong> matches today&#39;s date.</span></span></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b2cf5-173">(methodName(parameters))（括号之间的 <strong>SysQueryRangeUtil</strong> 方法）</span><span class="sxs-lookup"><span data-stu-id="b2cf5-173">(methodName(parameters)) (<strong>SysQueryRangeUtil</strong> method between parentheses)</span></span></td>
<td><span data-ttu-id="b2cf5-174">匹配由 <strong>SysQueryRangeUtil</strong> 方法的参数指定的值或值范围</span><span class="sxs-lookup"><span data-stu-id="b2cf5-174">Matching the value or range of values that are specified by the parameters of the <strong>SysQueryRangeUtil</strong> method</span></span></td>
<td><span data-ttu-id="b2cf5-175">键入具有指定值或值的范围的参数的 <strong>SysQueryRangeUtil</strong> 方法。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-175">Type a <strong>SysQueryRangeUtil</strong> method that has parameters that specify the value or range of values.</span></span></td>
<td><ol>
<li><span data-ttu-id="b2cf5-176">单击<strong>应收账款</strong> &gt; <strong>发票</strong> &gt; <strong>未结客户发票</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-176">Click <strong>Accounts receivable</strong> &gt; <strong>Invoices</strong> &gt; <strong>Open customer invoices</strong>.</span></span></li>
<li><span data-ttu-id="b2cf5-177">按 Ctrl+Shift+F3 打开<strong>查询</strong>页。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-177">Press Ctrl+Shift+F3 to open the <strong>Inquiry</strong> page.</span></span></li>
<li><span data-ttu-id="b2cf5-178">在<strong>范围</strong>选项卡上，单击<strong>添加</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-178">On the <strong>Range</strong> tab, click <strong>Add</strong>.</span></span></li>
<li><span data-ttu-id="b2cf5-179">在<strong>表</strong>字段中，选择<strong>未结客户交易记录</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-179">In the <strong>Table</strong> field, select <strong>Open customer transactions</strong>.</span></span></li>
<li><span data-ttu-id="b2cf5-180">在<strong>字段</strong>字段中，选择<strong>到期日期</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-180">In the <strong>Field</strong> field, select <strong>Due date</strong>.</span></span></li>
<li><span data-ttu-id="b2cf5-181">在<strong>条件</strong>字段中，输入 <strong>(yearRange(-2,0))</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-181">In the <strong>Criteria</strong> field, enter <strong>(yearRange(-2,0))</strong>.</span></span></li>
<li><span data-ttu-id="b2cf5-182">单击<strong>OK</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-182">Click <strong>OK</strong>.</span></span> <span data-ttu-id="b2cf5-183">更新列表页并列出与输入的条件匹配的发票。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-183">The list page is updated and lists the invoices that match the criterion that you entered.</span></span> <span data-ttu-id="b2cf5-184">对于此示例，在前两年到期的发票将列出。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-184">For this example, invoices that were due in the previous two years are listed.</span></span></li>
</ol>
<span data-ttu-id="b2cf5-185">请参阅下一部分中的表了解有关 <strong>SysQueryRangeUtil</strong> 的其他详细信息和若干示例。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-185">See the table in the next section for additional details about <strong>SysQueryRangeUtil</strong> date methods, and several examples.</span></span></td>
</tr>
</tbody>
</table>

## <a name="advanced-date-queries-that-use-sysqueryrangeutil-methods"></a><span data-ttu-id="b2cf5-186">使用 SysQueryRangeUtil 方法的高级日期查询</span><span class="sxs-lookup"><span data-stu-id="b2cf5-186">Advanced date queries that use SysQueryRangeUtil methods</span></span>
<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<thead>
<tr class="header">
<th><span data-ttu-id="b2cf5-187">方法</span><span class="sxs-lookup"><span data-stu-id="b2cf5-187">Method</span></span></th>
<th><span data-ttu-id="b2cf5-188">描述</span><span class="sxs-lookup"><span data-stu-id="b2cf5-188">Description</span></span></th>
<th><span data-ttu-id="b2cf5-189">示例</span><span class="sxs-lookup"><span data-stu-id="b2cf5-189">Example</span></span></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><span data-ttu-id="b2cf5-190">Day (_relativeDays=0)</span><span class="sxs-lookup"><span data-stu-id="b2cf5-190">Day (_relativeDays=0)</span></span></td>
<td><span data-ttu-id="b2cf5-191">查找与会话日期相关的日期。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-191">Find a date relative to the session date.</span></span> <span data-ttu-id="b2cf5-192">正值表示将来日期，负值指示过去日期。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-192">Positive values indicate future dates, and negative values indicate past dates.</span></span></td>
<td><ul>
<li><span data-ttu-id="b2cf5-193"><strong>明天</strong> – 输入 <strong>(Day(1))</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-193"><strong>Tomorrow</strong> – Enter <strong>(Day(1))</strong>.</span></span></li>
<li><span data-ttu-id="b2cf5-194"><strong>今天</strong> – 输入 <strong>(Day(0))</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-194"><strong>Today</strong> – Enter <strong>(Day(0))</strong>.</span></span></li>
<li><span data-ttu-id="b2cf5-195"><strong>昨天</strong> – 输入 <strong>(Day(-1))</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-195"><strong>Yesterday</strong> – Enter <strong>(Day(-1))</strong>.</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b2cf5-196">DayRange (_relativeDaysFrom=0，_relativeDaysTo=0)</span><span class="sxs-lookup"><span data-stu-id="b2cf5-196">DayRange (_relativeDaysFrom=0, _relativeDaysTo=0)</span></span></td>
<td><span data-ttu-id="b2cf5-197">查找与会话日期相关的日期范围。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-197">Find a range of dates relative to the session date.</span></span> <span data-ttu-id="b2cf5-198">正值表示将来日期，负值指示过去日期。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-198">Positive values indicate future dates, and negative values indicate past dates.</span></span></td>
<td><ul>
<li><span data-ttu-id="b2cf5-199"><strong>最后 30 天</strong> – 输入 <strong>(DayRange(-30,0))</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-199"><strong>Last 30 days</strong> – Enter <strong>(DayRange(-30,0))</strong>.</span></span></li>
<li><span data-ttu-id="b2cf5-200"><strong>前 30 天和后 30 天</strong> – 输入 <strong>(DayRange(-30,30))</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-200"><strong>Previous 30 days and next 30 days</strong> – Enter <strong>(DayRange(-30,30))</strong>.</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b2cf5-201">GreaterThanDate (_relativeDays=0) GreaterThanUtcDate (_relativeDays=0)</span><span class="sxs-lookup"><span data-stu-id="b2cf5-201">GreaterThanDate (_relativeDays=0) GreaterThanUtcDate (_relativeDays=0)</span></span></td>
<td><span data-ttu-id="b2cf5-202">查找指定相关日期之后的所有日期。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-202">Find all dates after the specified relative date.</span></span></td>
<td><ul>
<li><span data-ttu-id="b2cf5-203"><strong>从现在起超过 30 天</strong> – 输入 <strong>(GreaterThanDate(30))</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-203"><strong>More than 30 days from now</strong> – Enter <strong>(GreaterThanDate(30))</strong>.</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b2cf5-204">GreaterThanUtcNow ()</span><span class="sxs-lookup"><span data-stu-id="b2cf5-204">GreaterThanUtcNow ()</span></span></td>
<td><span data-ttu-id="b2cf5-205">查找当前时间后的所有日期/时间条目。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-205">Find all date/time entries after the current time.</span></span></td>
<td><ul>
<li><span data-ttu-id="b2cf5-206"><strong>所有将来日期/时间</strong> – 输入 <strong>(GreaterThanUtcNow())</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-206"><strong>All future date/times</strong> – Enter <strong>(GreaterThanUtcNow())</strong>.</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b2cf5-207">LessThanDate (_relativeDays=0) LessThanUtcDate (_relativeDays=0)</span><span class="sxs-lookup"><span data-stu-id="b2cf5-207">LessThanDate (_relativeDays=0) LessThanUtcDate (_relativeDays=0)</span></span></td>
<td><span data-ttu-id="b2cf5-208">查找指定相关日期之前的所有日期。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-208">Find all dates before the specified relative date.</span></span></td>
<td><ul>
<li><span data-ttu-id="b2cf5-209"><strong>从现在起少于七天</strong> – 输入 <strong>(LessThanDate(7))</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-209"><strong>Less than seven days from now</strong> – Enter <strong>(LessThanDate(7))</strong>.</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b2cf5-210">LessThanUtcNow ()</span><span class="sxs-lookup"><span data-stu-id="b2cf5-210">LessThanUtcNow ()</span></span></td>
<td><span data-ttu-id="b2cf5-211">查找当前时间前的所有日期/时间条目。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-211">Find all date/time entries before the current time.</span></span></td>
<td><ul>
<li><span data-ttu-id="b2cf5-212"><strong>所有过去日期/时间</strong> – 输入 <strong>(LessThanUtcNow())</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-212"><strong>All past date/times</strong> – Enter <strong>(LessThanUtcNow())</strong>.</span></span></li>
</ul></td>
</tr>
<tr class="odd">
<td><span data-ttu-id="b2cf5-213">MonthRange (_relativeFrom=0, _relativeTo=0)</span><span class="sxs-lookup"><span data-stu-id="b2cf5-213">MonthRange (_relativeFrom=0, _relativeTo=0)</span></span></td>
<td><span data-ttu-id="b2cf5-214">基于与当前月份相关的月查找日期范围。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-214">Find a range of dates, based on months relative to the current month.</span></span></td>
<td><ul>
<li><span data-ttu-id="b2cf5-215"><strong>前两个月</strong> – 输入 <strong>(MonthRange(-2,0))</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-215"><strong>Previous two months</strong> – Enter <strong>(MonthRange(-2,0))</strong>.</span></span></li>
<li><span data-ttu-id="b2cf5-216"><strong>后三个月</strong> – 输入 <strong>(MonthRange(0,3))</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-216"><strong>Next three months</strong> – Enter <strong>(MonthRange(0,3))</strong>.</span></span></li>
</ul></td>
</tr>
<tr class="even">
<td><span data-ttu-id="b2cf5-217">YearRange (_relativeFrom=0, _relativeTo=0)</span><span class="sxs-lookup"><span data-stu-id="b2cf5-217">YearRange (_relativeFrom=0, _relativeTo=0)</span></span></td>
<td><span data-ttu-id="b2cf5-218">基于与当前年份相关的年份查找日期范围。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-218">Find a range of dates, based on years relative to the current year.</span></span></td>
<td><ul>
<li><span data-ttu-id="b2cf5-219"><strong>下一年</strong> – 输入 <strong>(YearRange(0, 1))</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-219"><strong>Next year</strong> – Enter <strong>(YearRange(0, 1))</strong>.</span></span></li>
<li><span data-ttu-id="b2cf5-220"><strong>前一年</strong> – 输入 <strong>(YearRange(-1,0))</strong>。</span><span class="sxs-lookup"><span data-stu-id="b2cf5-220"><strong>Previous year</strong> – Enter <strong>(YearRange(-1,0))</strong>.</span></span></li>
</ul></td>
</tr>
</tbody>
</table>




