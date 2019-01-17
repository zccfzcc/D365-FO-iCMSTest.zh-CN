---
title: 供应商交易记录列表页
description: 此主题提供有关 Microsoft Dynamics 365 for Finance and Operations 的“供应商交易记录列表”页的信息。
author: mikefalkner
manager: aolson
ms.date: 08/24/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: VendTrans
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mikefalkner
ms.search.validFrom: 2018-10-31
ms.dyn365.ops.version: 8.0999999999999996
ms.openlocfilehash: 89468f536b977d3553790560a16bbd954f54304d
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "53785"
---
# <a name="vendor-transactions-list-page"></a><span data-ttu-id="803cb-103">供应商交易记录列表页</span><span class="sxs-lookup"><span data-stu-id="803cb-103">Vendor transactions list page</span></span>

[!include [banner](../includes/banner.md)]

## <a name="view-settlements"></a><span data-ttu-id="803cb-104">查看结算</span><span class="sxs-lookup"><span data-stu-id="803cb-104">View settlements</span></span>

<span data-ttu-id="803cb-105">操作窗格上的**查看结算**按钮提供对结算交易记录的结算历史记录和详细信息的快速访问。</span><span class="sxs-lookup"><span data-stu-id="803cb-105">The **View settlements** button on the Action Pane provides quick access to the settlement history and detailed information about the settlement transaction.</span></span> <span data-ttu-id="803cb-106">还可以显示与所选交易记录有关的其他交易记录，因为这些交易记录属于相同结算，或因为这些交易记录是同一个付款日记帐中创建的付款。</span><span class="sxs-lookup"><span data-stu-id="803cb-106">You can also show additional transactions that are related to the selected transaction, either because they were part of the same settlement or because they are payments that were created in the same payment journal.</span></span>

1. <span data-ttu-id="803cb-107">选择**应付帐款 \> 所有供应商**。</span><span class="sxs-lookup"><span data-stu-id="803cb-107">Select **Accounts payable \> All vendors**.</span></span>
2. <span data-ttu-id="803cb-108">选择具有交易记录的供应商，然后在操作窗格的**供应商**选项卡上选择**交易记录**。</span><span class="sxs-lookup"><span data-stu-id="803cb-108">Select a vendor that has transactions, and then, on the Action Pane, on the **Vendor** tab, select **Transactions**.</span></span>
3. <span data-ttu-id="803cb-109">选择要研究的交易记录，然后在操作窗格上选择**查看结算**。</span><span class="sxs-lookup"><span data-stu-id="803cb-109">Select a transaction to research, and then, on the Action Pane, select **View settlements**.</span></span>

    <span data-ttu-id="803cb-110">将显示**查看结算**对话框，其中显示所选交易记录以及已为其结算的所有单据。</span><span class="sxs-lookup"><span data-stu-id="803cb-110">The **View settlements** dialog box appears, and shows the selected transaction and all documents that have been settled against it.</span></span> <span data-ttu-id="803cb-111">此对话框类似结算历史记录视图，不过其中包含所有相关单据。</span><span class="sxs-lookup"><span data-stu-id="803cb-111">This dialog box resembles the settlement history view, but it includes all related documents.</span></span>

4. <span data-ttu-id="803cb-112">可在此对话框中执行多种任务。</span><span class="sxs-lookup"><span data-stu-id="803cb-112">In the dialog box, you can perform various tasks.</span></span> <span data-ttu-id="803cb-113">选择一个或多个凭证，然后选择以下按钮之一：</span><span class="sxs-lookup"><span data-stu-id="803cb-113">Select one or more vouchers, and then select one of the following buttons:</span></span>

    - <span data-ttu-id="803cb-114">–**查看相关**  – 显示在与所选单据关联的付款日记帐中创建的所有付款日记帐交易记录。</span><span class="sxs-lookup"><span data-stu-id="803cb-114">**View related** – Show all the payment journal transactions that were created in the payment journal that is related to the selected document.</span></span> <span data-ttu-id="803cb-115">此外，还将显示与这些付款有关的所有结算。</span><span class="sxs-lookup"><span data-stu-id="803cb-115">In addition, all the settlements that are related to those payments are shown.</span></span> <span data-ttu-id="803cb-116">查看相关付款时，此按钮的标签将变为**查看结算**。</span><span class="sxs-lookup"><span data-stu-id="803cb-116">While you're viewing related payments, the label of this button changes to **View settlements**.</span></span> <span data-ttu-id="803cb-117">选择**查看结算**将仅显示首次打开**查看结算**对话框时显示的交易记录。</span><span class="sxs-lookup"><span data-stu-id="803cb-117">Select **View settlements** to show only the transactions that were shown when you first opened the **View settlements** dialog box.</span></span>
    - <span data-ttu-id="803cb-118">**查看历史记录** – 显示凭证的结算历史记录。</span><span class="sxs-lookup"><span data-stu-id="803cb-118">**View history** – Show the settlement history for the vouchers.</span></span> <span data-ttu-id="803cb-119">选择**关闭**关闭对话框。</span><span class="sxs-lookup"><span data-stu-id="803cb-119">Select **Close** to close the dialog box.</span></span>
    - <span data-ttu-id="803cb-120">**查看记帐** – 显示与所选单据相关的所有凭证。</span><span class="sxs-lookup"><span data-stu-id="803cb-120">**View accounting** – Show all vouchers that are related to the selected documents.</span></span> <span data-ttu-id="803cb-121">选择**关闭**关闭对话框。</span><span class="sxs-lookup"><span data-stu-id="803cb-121">Select **Close** to close the dialog box.</span></span>
    - <span data-ttu-id="803cb-122">**导出** – 将所选凭证导出到 Microsoft Excel。</span><span class="sxs-lookup"><span data-stu-id="803cb-122">**Export** – Export the selected vouchers to Microsoft Excel.</span></span>
    - <span data-ttu-id="803cb-123">**结算交易记录** – 仅当未完全结算选择的原始单据，才显示此按钮。</span><span class="sxs-lookup"><span data-stu-id="803cb-123">**Settle transactions** – This button appears only if the original document that was selected wasn't fully settled.</span></span> <span data-ttu-id="803cb-124">选择此按钮后，将显示**结算交易记录**对话框，可在此处选择要结算的交易记录。</span><span class="sxs-lookup"><span data-stu-id="803cb-124">When you select this button, the **Settle transactions** dialog box appears, where you can select transactions for settlement.</span></span>
    - <span data-ttu-id="803cb-125">**撤消结算** – 仅当已完全结算选择的原始单据，才显示此按钮。</span><span class="sxs-lookup"><span data-stu-id="803cb-125">**Undo settlements** – This button appears only if the original document that was selected was fully settled.</span></span> <span data-ttu-id="803cb-126">选择此按钮后，将显示**撤消结算**对话框，可在此处撤消已对该单据执行的结算。</span><span class="sxs-lookup"><span data-stu-id="803cb-126">When you select this button, the **Undo settlements** dialog box appears, where you can undo the settlements that were done for that document.</span></span>

## <a name="global-transactions"></a><span data-ttu-id="803cb-127">全球交易</span><span class="sxs-lookup"><span data-stu-id="803cb-127">Global transactions</span></span>

<span data-ttu-id="803cb-128">**全局交易记录**按钮也会显示在**供应商交易记录**列表页中。</span><span class="sxs-lookup"><span data-stu-id="803cb-128">The **Global transactions** button also displays on the **Vendor transactions** list page.</span></span> <span data-ttu-id="803cb-129">此按钮用于查看某个供应商在所有法人中的所有交易记录。</span><span class="sxs-lookup"><span data-stu-id="803cb-129">This button lets you view all transactions for a vendor across all legal entities.</span></span> <span data-ttu-id="803cb-130">**供应商交易记录**列表页仅显示用户根据自己的安全设置可访问的法人的交易记录。</span><span class="sxs-lookup"><span data-stu-id="803cb-130">The **Vendor transactions** list page shows transactions only for the legal entities that the user has access to, based on his or her security settings.</span></span>

<span data-ttu-id="803cb-131">该列表页显示当事方 ID 与您开始处理的供应商相同的供应商的所有交易记录。</span><span class="sxs-lookup"><span data-stu-id="803cb-131">The list page will show all transactions for vendors that have the same party ID as the vendor that you started with.</span></span> <span data-ttu-id="803cb-132">例如，如果一个法人中的供应商 US-001 的当事方 ID 与另一个法人中的供应商 DE-001 相同，则显示这两个供应商 ID 的所有交易记录。</span><span class="sxs-lookup"><span data-stu-id="803cb-132">For example, if vendor US-001 in one legal entity has the same party ID as vendor DE-001 in another legal entity, all transactions for both vendor IDs are shown.</span></span>

<span data-ttu-id="803cb-133">**供应商交易记录**列表页中的菜单取决于交易记录的法人。</span><span class="sxs-lookup"><span data-stu-id="803cb-133">The menus on the **Vendor transactions** list page vary, depending on the legal entity for the transaction.</span></span> <span data-ttu-id="803cb-134">例如，如果某项功能仅可用于瑞士法人，则仅当选择了瑞士交易记录时才显示该功能的菜单选项。</span><span class="sxs-lookup"><span data-stu-id="803cb-134">For example, if a feature is available only for Swiss legal entities, the menu options for that feature appear only when a Swiss transaction is selected.</span></span>

<span data-ttu-id="803cb-135">若要访问该功能，请执行以下步骤。</span><span class="sxs-lookup"><span data-stu-id="803cb-135">To access the feature, follow these steps.</span></span>

1. <span data-ttu-id="803cb-136">选择**应付帐款** \> **所有供应商**。</span><span class="sxs-lookup"><span data-stu-id="803cb-136">Select **Accounts payable** \> **All vendors**.</span></span>
2. <span data-ttu-id="803cb-137">选择供应商，然后在操作窗格的**供应商**选项卡上的**交易记录**组中，选择**全局交易记录**。</span><span class="sxs-lookup"><span data-stu-id="803cb-137">Select a vendor, and then, on the Action Pane, on the **Vendor** tab, in the **Transactions** group, select **Global transactions**.</span></span>

## <a name="more-transaction-filters"></a><span data-ttu-id="803cb-138">其他交易记录筛选器</span><span class="sxs-lookup"><span data-stu-id="803cb-138">More transaction filters</span></span>

<span data-ttu-id="803cb-139">已将用于显示未结交易记录的筛选器替换为了新筛选器，可通过该筛选器查看更多交易记录组合。</span><span class="sxs-lookup"><span data-stu-id="803cb-139">The filter for showing open transactions has been replaced with a new filter that lets you view more combinations of transactions.</span></span> <span data-ttu-id="803cb-140">**显示**字段中具有以下选项：</span><span class="sxs-lookup"><span data-stu-id="803cb-140">The following options are available in the **Show** field:</span></span>

- <span data-ttu-id="803cb-141">**全部** – 显示所选供应商的所有交易记录（未结和已结）。</span><span class="sxs-lookup"><span data-stu-id="803cb-141">**All** – Show all transactions for the selected vendors (open and closed).</span></span>
- <span data-ttu-id="803cb-142">**已结** – 仅显示已完全结算并结束的交易记录。</span><span class="sxs-lookup"><span data-stu-id="803cb-142">**Closed** – Show only transactions that have been fully settled and closed.</span></span>
- <span data-ttu-id="803cb-143">**未结** – 仅显示尚未完全结算的交易记录。</span><span class="sxs-lookup"><span data-stu-id="803cb-143">**Open** – Show only transactions that haven't been fully settled.</span></span>
- <span data-ttu-id="803cb-144">**未结(包括已结日期或之后日期)** – 仅显示未在您指定日期或之后完全结算的交易记录。</span><span class="sxs-lookup"><span data-stu-id="803cb-144">**Open including closed on or after date** – Show only transactions that haven't been fully settled on or after a date that you specify.</span></span> <span data-ttu-id="803cb-145">如果选择此选项你，则可更改筛选器旁边显示的日期。</span><span class="sxs-lookup"><span data-stu-id="803cb-145">When you select this option, you can change the date that is shown next to the filter.</span></span> <span data-ttu-id="803cb-146">列表中显示**最后结算日期**值在您指定的日期或之后的交易记录，即使这些交易记录在当天完全结算。</span><span class="sxs-lookup"><span data-stu-id="803cb-146">Transactions that have a **Last settlement date** value on or after the date that you specify are shown in the list, even if those transactions are fully settled as of the current date.</span></span> <span data-ttu-id="803cb-147">但是，余额显示截止当前日期的余额，而不是截止所选日期的余额。</span><span class="sxs-lookup"><span data-stu-id="803cb-147">However, the balance represents the balances as of the current date, not as of the selected date.</span></span>

<span data-ttu-id="803cb-148">选择**隐藏货币重估**复选框隐藏货币折算交易记录。</span><span class="sxs-lookup"><span data-stu-id="803cb-148">Select the **Hide currency revaluations** check box to hide currency translation transactions.</span></span>

## <a name="modify-due-dates-and-discount-dates"></a><span data-ttu-id="803cb-149">修改到期日期和折扣日期</span><span class="sxs-lookup"><span data-stu-id="803cb-149">Modify due dates and discount dates</span></span>

<span data-ttu-id="803cb-150">可以更新未结客户交易记录的到期日期和折扣日期。</span><span class="sxs-lookup"><span data-stu-id="803cb-150">You can update due dates and discount dates for open customer transactions.</span></span> <span data-ttu-id="803cb-151">在版本 8.1 中，现在可以向**供应商交易记录**列表页添加到期日期。</span><span class="sxs-lookup"><span data-stu-id="803cb-151">In release 8.1, you can now add due dates to the **Vendor transactions** list page.</span></span> <span data-ttu-id="803cb-152">也可以通过在**供应商交易记录**列表页中单击到期日期，更改**更新到期日期和现金折扣日期**对话框中的到期日期、折扣日期、付款期限和现金折扣期限。</span><span class="sxs-lookup"><span data-stu-id="803cb-152">By clicking on the due date in the **Vendor transactions** list page, you can also change due dates, discount dates, payment terms, and cash discount terms in the **Update due date and cash discount dates**  dialog box.</span></span>

### <a name="activate-the-feature"></a><span data-ttu-id="803cb-153">激活功能</span><span class="sxs-lookup"><span data-stu-id="803cb-153">Activate the feature</span></span>

<span data-ttu-id="803cb-154">要通过使用 **更新到期日期和现金折扣日期**对话框向**供应商交易记录**列表页添加到到期日期和更改交易记录的付款设置，请执行以下步骤。</span><span class="sxs-lookup"><span data-stu-id="803cb-154">To add due dates to the **Vendor transactions** list page and change payment settings for a transaction by using the **Update due date and cash discount dates** dialog box, follow these steps.</span></span>

1. <span data-ttu-id="803cb-155">选择**应付帐款 \> 设置 \> 应付帐款参数**。</span><span class="sxs-lookup"><span data-stu-id="803cb-155">Select **Accounts payable \> Setup \> Accounts payable parameters**.</span></span>
2. <span data-ttu-id="803cb-156">在**结算**选项卡上，将**显示到期日期并允许编辑**选项设置为**是**。</span><span class="sxs-lookup"><span data-stu-id="803cb-156">On the **Settlements** tab, set the **Show due date and allow edit** option to **Yes**.</span></span>
3. <span data-ttu-id="803cb-157">要启用此功能，应该已将新字段添加到了供应商交易记录。</span><span class="sxs-lookup"><span data-stu-id="803cb-157">To enable this feature, new fields have been added to vendor transactions.</span></span> <span data-ttu-id="803cb-158">完成新交易记录时，将填写这些字段。</span><span class="sxs-lookup"><span data-stu-id="803cb-158">Those fields will be filled in when a new transaction is completed.</span></span> <span data-ttu-id="803cb-159">打开**更新到期日期和现金折扣日期**对话框时，也将填写这些字段。</span><span class="sxs-lookup"><span data-stu-id="803cb-159">They will also be filled in when you open the **Update due date and cash discount dates** dialog box.</span></span> <span data-ttu-id="803cb-160">如果将**显示到期日期并允许编辑**选项设置为**是**，将显示**更新付款信息**对话框。</span><span class="sxs-lookup"><span data-stu-id="803cb-160">When you set the **Show due date and allow edit** option to **Yes**, you will see the **Update payment information** dialog box.</span></span>  <span data-ttu-id="803cb-161">要立即更新现有交易记录，请选择**更新所有现有交易记录**。</span><span class="sxs-lookup"><span data-stu-id="803cb-161">To update existing transactions immediately, select **Update all existing transactions**.</span></span> <span data-ttu-id="803cb-162">此外，要仅为新交易记录填写这些字段，请选择**继续但不更新**。</span><span class="sxs-lookup"><span data-stu-id="803cb-162">Alternatively, to fill in the fields only for new transactions, select **Continue without update**.</span></span>

<span data-ttu-id="803cb-163">到期日期现在已添加到**供应商交易记录**列表页，以便您可以轻松地修改交易记录的到期日期和现金折扣日期。</span><span class="sxs-lookup"><span data-stu-id="803cb-163">The due date is now added to the **Vendor transactions** list page, so you can easily modify the due date and cash discount dates for transactions.</span></span>

### <a name="modify-the-payment-settings"></a><span data-ttu-id="803cb-164">修改付款设置</span><span class="sxs-lookup"><span data-stu-id="803cb-164">Modify the payment settings</span></span>

<span data-ttu-id="803cb-165">**供应商交易记录**列表页显示供应商的所有交易记录。</span><span class="sxs-lookup"><span data-stu-id="803cb-165">The **Vendor transactions** list page shows all transactions for a vendor.</span></span> <span data-ttu-id="803cb-166">选择交易记录的到期日期时，将显示一个对话框。</span><span class="sxs-lookup"><span data-stu-id="803cb-166">When you select the due date for a transaction, a dialog box appears.</span></span> <span data-ttu-id="803cb-167">此对话框显示到期日期和折扣计算、到期日期、付款期限、现金折扣期限和现金折扣日期的基准日期。</span><span class="sxs-lookup"><span data-stu-id="803cb-167">This dialog box shows the base date for due date and discount calculations, due date, payment terms, cash discount terms, and cash discount dates.</span></span>

<span data-ttu-id="803cb-168">编辑时，每个字段对交易记录的影响各不相同：</span><span class="sxs-lookup"><span data-stu-id="803cb-168">Each field has a different effect on the transaction when you edit it:</span></span>

- <span data-ttu-id="803cb-169">**编辑基准日期** - 将单据日期视为基准日期来更改到期日期和折扣日期。</span><span class="sxs-lookup"><span data-stu-id="803cb-169">**Edit the base date** - The due date and discount dates are changed as if the base date is the document date.</span></span>
- <span data-ttu-id="803cb-170">**编辑到期日期** - 仅更改了到期日期</span><span class="sxs-lookup"><span data-stu-id="803cb-170">**Edit the due date** - Only the due date is changed</span></span>
- <span data-ttu-id="803cb-171">**编辑折扣日期** - 仅更改折扣日期。</span><span class="sxs-lookup"><span data-stu-id="803cb-171">**Edit the discount dates** - Only the discount dates are changed.</span></span>
- <span data-ttu-id="803cb-172">**编辑付款期限** - 根据基准日期和付款期限更改到期日期。</span><span class="sxs-lookup"><span data-stu-id="803cb-172">**Edit the payment terms** - The due date is changed, based on the base date and the payment terms.</span></span>
- <span data-ttu-id="803cb-173">**编辑现金折扣期限** - 根据基准日期和现金折扣期限更改现金折扣。</span><span class="sxs-lookup"><span data-stu-id="803cb-173">**Edit the cash discount terms** - The cash discounts are changed, based on the base date and the cash discount terms.</span></span>

<span data-ttu-id="803cb-174">付款设置编辑完毕后，请选择**关闭**以保存更改。</span><span class="sxs-lookup"><span data-stu-id="803cb-174">When you've finished editing the payment settings, select **Close** to save your changes.</span></span>
