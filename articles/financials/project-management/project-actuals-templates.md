---
title: 将项目实际值直接从 Project Service Automation 同步到 Finance and Operations 中的项目集成日记帐进行过帐
description: 本主题介绍用于将项目实际值直接从 Microsoft Dynamics 365 for Project Service Automation 同步到 Microsoft Dynamics 365 for Finance and Operations 的模板和基础任务。
author: KimANelson
manager: AnnBe
ms.date: 07/20/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 87983
ms.assetid: b454ad57-2fd6-46c9-a77e-646de4153067
ms.search.region: Global
ms.author: knelson
ms.search.validFrom: 2016-11-28
ms.dyn365.ops.version: AX 7.3.0
ms.openlocfilehash: 9a5154259ee1e92c8c80128e7fadcea3cc3b7632
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56177"
---
# <a name="synchronize-project-actuals-directly-from-project-service-automation-to-the-project-integration-journal-for-posting-in-finance-and-operations"></a><span data-ttu-id="7327a-103">将项目实际值直接从 Project Service Automation 同步到 Finance and Operations 中的项目集成日记帐进行过帐</span><span class="sxs-lookup"><span data-stu-id="7327a-103">Synchronize project actuals directly from Project Service Automation to the project integration journal for posting in Finance and Operations</span></span>

[!include[banner](../includes/banner.md)]

<span data-ttu-id="7327a-104">本主题介绍用于将项目实际值直接从 Microsoft Dynamics 365 for Project Service Automation 同步到 Microsoft Dynamics 365 for Finance and Operations 的模板和基础任务。</span><span class="sxs-lookup"><span data-stu-id="7327a-104">This topic describes the templates and underlying tasks that are used to synchronize project actuals directly from Microsoft Dynamics 365 for Project Service Automation to Microsoft Dynamics 365 for Finance and Operations.</span></span>

<span data-ttu-id="7327a-105">此模板将交易记录从 Project Service Automation 同步到 Finance and Operations 中的暂存表内。</span><span class="sxs-lookup"><span data-stu-id="7327a-105">The template synchronizes transactions from Project Service Automation into a staging table in Finance and Operations.</span></span> <span data-ttu-id="7327a-106">同步完成后，**必须**将数据从暂存表导入集成日记帐。</span><span class="sxs-lookup"><span data-stu-id="7327a-106">After synchronization is completed, you **must** import the data from the staging table into the integration journal.</span></span>

> [!NOTE]
> - <span data-ttu-id="7327a-107">Microsoft Dynamics 365 for Finance and Operations 版本 8.0.1 或更高版本中支持项目实际值集成。</span><span class="sxs-lookup"><span data-stu-id="7327a-107">Project actuals integration is available in Microsoft Dynamics 365 for Finance and Operations version 8.0.1 or later.</span></span>
> - <span data-ttu-id="7327a-108">如果您正在使用 Microsoft Dynamics 365 for Finance and Operations Enterprise Edition 7.3.0，则安装 KB 4132657 和 KB 4132660 之后，可以使用模板集成项目任务、费用交易记录类别、工时估计值、费用估计值和实际值和配置功能锁定。</span><span class="sxs-lookup"><span data-stu-id="7327a-108">If you're using Microsoft Dynamics 365 for Finance and Operations, Enterprise edition 7.3.0, after you install KB 4132657 and KB 4132660, you will be able to use the templates to integrate project tasks, expense transaction categories, hour estimates, expense estimates, and actuals, and to configure functionality locking.</span></span> <span data-ttu-id="7327a-109">如果必须重置会计分配，建议也安装 KB 4131710。</span><span class="sxs-lookup"><span data-stu-id="7327a-109">If you must reset the accounting distributions, we recommend that you also install KB 4131710.</span></span>
> - <span data-ttu-id="7327a-110">如果在使用 Finance and Operations 7.3.0，并从 Project Service Automation 导入免费交易记录，则必须安装 KB 4345320，以便将这些费用添加到该项目发票中。</span><span class="sxs-lookup"><span data-stu-id="7327a-110">If you're using Finance and Operations 7.3.0, and you are bringing fee transactions over from Project Service Automation, you must install KB 4345320 in order to include those fees in the project invoice.</span></span>
> - <span data-ttu-id="7327a-111">如果要在 Project Service Automation 中输入时间或支出交易记录的销售税金额，则必须安装 Project Service Automation 更新 7。</span><span class="sxs-lookup"><span data-stu-id="7327a-111">If you're entering sales tax amounts on time or expense transactions in Project Service Automation, you must install Project Service Automation Update 7.</span></span> <span data-ttu-id="7327a-112">否则，将不会把税金实际值链接到关联的时间或支出实际值，因此不会同步到 Finance and Operations。</span><span class="sxs-lookup"><span data-stu-id="7327a-112">Otherwise, the tax actuals won't be linked to the associated time or expense actuals, and they won't be synchronized to Finance and Operations.</span></span> <span data-ttu-id="7327a-113">有关详细信息，请联系支持人员。</span><span class="sxs-lookup"><span data-stu-id="7327a-113">For more information, contact Support.</span></span>

## <a name="data-flow-for-project-service-automation-to-finance-and-operations"></a><span data-ttu-id="7327a-114">Project Service Automation 到 Finance and Operations 的数据传输</span><span class="sxs-lookup"><span data-stu-id="7327a-114">Data flow for Project Service Automation to Finance and Operations</span></span>

<span data-ttu-id="7327a-115">Project Service Automation 到 Finance and Operations 集成解决方案使用数据集成功能在 Project Service Automation 和 Finance and Operations 的实例之间同步数据。</span><span class="sxs-lookup"><span data-stu-id="7327a-115">The Project Service Automation to Finance and Operations integration solution uses the Data integration feature to synchronize data across instances of Project Service Automation and Finance and Operations.</span></span> <span data-ttu-id="7327a-116">可通过数据集成功能提供的集成模板将有关项目实际值的数据从 Project Service Automation 传输到 Finance and Operations。</span><span class="sxs-lookup"><span data-stu-id="7327a-116">The integration templates that are available with the Data integration feature enable the flow of data about project actuals from Project Service Automation to Finance and Operations.</span></span>

<span data-ttu-id="7327a-117">下图显示 Project Service Automation 与 Finance and Operations 之间中如何同步数据。</span><span class="sxs-lookup"><span data-stu-id="7327a-117">The following illustration shows how the data is synchronized between Project Service Automation and Finance and Operations.</span></span>

<span data-ttu-id="7327a-118">[![Project Service Automation 与 Finance and Operations 集成的数据传输](./media/ProjectActualsFlow.jpg)](./media/ProjectActualsFlow.jpg)</span><span class="sxs-lookup"><span data-stu-id="7327a-118">[![Data flow for Project Service Automation integration with Finance and Operations](./media/ProjectActualsFlow.jpg)](./media/ProjectActualsFlow.jpg)</span></span>

## <a name="project-actuals-from-project-service-automation"></a><span data-ttu-id="7327a-119">来自 Project Service Automation 的项目实际值</span><span class="sxs-lookup"><span data-stu-id="7327a-119">Project actuals from Project Service Automation</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="7327a-120">模板和任务</span><span class="sxs-lookup"><span data-stu-id="7327a-120">Template and tasks</span></span>

<span data-ttu-id="7327a-121">若要访问可用模板，请在 Microsoft PowerApps 管理员中心中选择**项目**，然后在右上角中选择**新建项目**以选择公共模板。</span><span class="sxs-lookup"><span data-stu-id="7327a-121">To access the available templates, in the Microsoft PowerApps admin center, select **Projects**, and then, in the upper-right corner, select **New project** to select public templates.</span></span>

<span data-ttu-id="7327a-122">以下模板和基础任务用于将项目实际值从 Project Service Automation 同步到 Finance and Operations：</span><span class="sxs-lookup"><span data-stu-id="7327a-122">The following template and underlying tasks are used to synchronize project actuals from Project Service Automation to Finance and Operations:</span></span>

- <span data-ttu-id="7327a-123">**数据集成中的模板名称：** 项目实际值（PSA 到 Fin and Ops）</span><span class="sxs-lookup"><span data-stu-id="7327a-123">**Name of the template in Data integration:** Project actuals (PSA to Fin and Ops)</span></span>
- <span data-ttu-id="7327a-124">**项目中的任务名称：**</span><span class="sxs-lookup"><span data-stu-id="7327a-124">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="7327a-125">实际值</span><span class="sxs-lookup"><span data-stu-id="7327a-125">Actuals</span></span>
    - <span data-ttu-id="7327a-126">TransactionConnections</span><span class="sxs-lookup"><span data-stu-id="7327a-126">TransactionConnections</span></span>

### <a name="entity-set"></a><span data-ttu-id="7327a-127">实体集</span><span class="sxs-lookup"><span data-stu-id="7327a-127">Entity set</span></span>

| <span data-ttu-id="7327a-128">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="7327a-128">Project Service Automation</span></span> | <span data-ttu-id="7327a-129">Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="7327a-129">Finance and Operations</span></span>                                   |
|----------------------------|----------------------------------------------------------|
| <span data-ttu-id="7327a-130">实际值</span><span class="sxs-lookup"><span data-stu-id="7327a-130">Actuals</span></span>                    | <span data-ttu-id="7327a-131">项目实际值的集成实体</span><span class="sxs-lookup"><span data-stu-id="7327a-131">Integration entity for project actuals</span></span>                   |
| <span data-ttu-id="7327a-132">交易记录连接</span><span class="sxs-lookup"><span data-stu-id="7327a-132">Transaction Connections</span></span>    | <span data-ttu-id="7327a-133">项目交易记录关系的集成实体</span><span class="sxs-lookup"><span data-stu-id="7327a-133">Integration entity for project transaction relationships</span></span> |

### <a name="entity-flow"></a><span data-ttu-id="7327a-134">实体流</span><span class="sxs-lookup"><span data-stu-id="7327a-134">Entity flow</span></span>

<span data-ttu-id="7327a-135">项目实际值在 Project Service Automation 中管理，并同步到 Finance and Operations 中的项目集成日记帐。</span><span class="sxs-lookup"><span data-stu-id="7327a-135">Project actuals are managed in Project Service Automation, and they are synchronized to the project integration journal in Finance and Operations.</span></span> <span data-ttu-id="7327a-136">将根据默认财务维度和过帐设置应用核算。</span><span class="sxs-lookup"><span data-stu-id="7327a-136">The accounting will be applied based on default financial dimensions and the posting setup.</span></span>

### <a name="prerequisites"></a><span data-ttu-id="7327a-137">必备项</span><span class="sxs-lookup"><span data-stu-id="7327a-137">Prerequisites</span></span>

<span data-ttu-id="7327a-138">必须先配置 Project Service Automation 集成参数并同步项目、项目任务和项目支出类别，才能同步实际值。</span><span class="sxs-lookup"><span data-stu-id="7327a-138">Before synchronization of actuals can occur, you must configure the Project Service Automation integration parameters and synchronize projects, project tasks, and project expense transaction categories.</span></span>

### <a name="power-query"></a><span data-ttu-id="7327a-139">Power Query</span><span class="sxs-lookup"><span data-stu-id="7327a-139">Power Query</span></span>

<span data-ttu-id="7327a-140">在项目实际值模板中，必须使用 Microsoft Power Query for Excel 才能完成以下任务：</span><span class="sxs-lookup"><span data-stu-id="7327a-140">In the project actuals template, you must use Microsoft Power Query for Excel to complete these tasks:</span></span>

- <span data-ttu-id="7327a-141">将 Project Service Automation 中的交易记录类型转换为 Finance and Operations 中的正确交易记录类型。</span><span class="sxs-lookup"><span data-stu-id="7327a-141">Transform the transaction type in Project Service Automation to the correct transaction type in Finance and Operations.</span></span> <span data-ttu-id="7327a-142">已经在项目实际值（PSA 到 Fin and Ops）模板中定义了此项转换。</span><span class="sxs-lookup"><span data-stu-id="7327a-142">This transformation is already defined in the Project actuals (PSA to Fin and Ops) template.</span></span>
- <span data-ttu-id="7327a-143">将 Project Service Automation 中的计费类型转换为 Finance and Operations 中的正确计费类型。</span><span class="sxs-lookup"><span data-stu-id="7327a-143">Transform the billing type in Project Service Automation to the correct billing type in Finance and Operations.</span></span> <span data-ttu-id="7327a-144">已经在项目实际值（PSA 到 Fin and Ops）模板中定义了此项转换。</span><span class="sxs-lookup"><span data-stu-id="7327a-144">This transformation is already defined in the Project actuals (PSA to Fin and Ops) template.</span></span> <span data-ttu-id="7327a-145">然后将根据 **Dynamics 365 for Project Service Automation 集成参数**页面中的配置把计费类型映射到行属性。</span><span class="sxs-lookup"><span data-stu-id="7327a-145">The billing type is then mapped to the line property, based on the configuration on the **Project Service Automation integration parameters** page.</span></span>
- <span data-ttu-id="7327a-146">筛选出必须使用此模板同步的特定资源组织单位。</span><span class="sxs-lookup"><span data-stu-id="7327a-146">Filter to specific resource organizational units that must be synchronized with this template.</span></span>
- <span data-ttu-id="7327a-147">如果公司间时间或公司间支出实际值将同步到 Finance and Operations，您必须在 Finance and Operations 中将合同组织单位转换为正确的法人。</span><span class="sxs-lookup"><span data-stu-id="7327a-147">If intercompany time or intercompany expense actuals will be synchronized to Finance and Operations, you must transform the contract organizational unit to the correct legal entity in Finance and Operations.</span></span> <span data-ttu-id="7327a-148">在项目实际值（PSA 到 Fin and Ops）模板中已基于演示数据定义了一个条件列。</span><span class="sxs-lookup"><span data-stu-id="7327a-148">In the Project actuals (PSA to Fin and Ops) template, a conditional column is defined based on demo data.</span></span> <span data-ttu-id="7327a-149">必须将最后插入的条件列更新为正确的法人。</span><span class="sxs-lookup"><span data-stu-id="7327a-149">You must update the last inserted conditional column to the correct legal entities.</span></span> <span data-ttu-id="7327a-150">否则可能出现错误或将不正确的交易记录导入 Finance and Operations 中。</span><span class="sxs-lookup"><span data-stu-id="7327a-150">Otherwise, either an integration error might occur, or incorrect actual transactions might be imported into Finance and Operations.</span></span>
- <span data-ttu-id="7327a-151">如果不将公司间时间或公司间支出实际值同步到 Finance and operations，则必须从模板中删除最后插入的条件列。</span><span class="sxs-lookup"><span data-stu-id="7327a-151">If intercompany time or intercompany expense actuals won't be synchronized to Finance and operations, you must delete the last inserted conditional column from your template.</span></span> <span data-ttu-id="7327a-152">否则可能出现错误或将不正确的交易记录导入 Finance and Operations 中。</span><span class="sxs-lookup"><span data-stu-id="7327a-152">Otherwise, either an integration error might occur, or incorrect actual transactions might be imported into Finance and Operations.</span></span>

#### <a name="contract-organizational-unit"></a><span data-ttu-id="7327a-153">合同组织单位</span><span class="sxs-lookup"><span data-stu-id="7327a-153">Contract organizational unit</span></span>
<span data-ttu-id="7327a-154">若要更新模板中插入的条件列，请单击**映射**箭头打开映射。</span><span class="sxs-lookup"><span data-stu-id="7327a-154">To update the inserted conditional column in the template, click the **Map** arrow to open the mapping.</span></span> <span data-ttu-id="7327a-155">选择**高级查询和筛选**链接以打开 Power Query。</span><span class="sxs-lookup"><span data-stu-id="7327a-155">Select the **Advanced Query and Filtering** link to open Power Query.</span></span>

- <span data-ttu-id="7327a-156">如果在使用默认的项目实际值（PSA 到 Fin and Ops）模板，请在 Power Query, 中从**应用的步骤**部分选择最后一个**插入的条件**。</span><span class="sxs-lookup"><span data-stu-id="7327a-156">If you're using the default Project actuals (PSA to Fin and Ops) template, in Power Query, select the last **Inserted Condition** from the **Applied Steps** section.</span></span> <span data-ttu-id="7327a-157">在**函数**条目中，将 **USSI** 替换为集成应使用的法人 的名称。</span><span class="sxs-lookup"><span data-stu-id="7327a-157">In the **Function** entry, replace **USSI** with the name of the legal entity that should be used with the integration.</span></span> <span data-ttu-id="7327a-158">根据需要向**函数**条目添加更多条件，然后将 **else** 条件从 **USMF** 更新为正确的法人。</span><span class="sxs-lookup"><span data-stu-id="7327a-158">Add additional conditions to the **Function** entry as you require, and update the **else** condition from **USMF** to the correct legal entity.</span></span>
- <span data-ttu-id="7327a-159">如果要新建模板，必须添加此列来为公司间数据和支出提供支持。</span><span class="sxs-lookup"><span data-stu-id="7327a-159">If you're creating a new template, you must add the column to support intercompany time and expenses.</span></span> <span data-ttu-id="7327a-160">选择**添加条件列**，然后为列输入名称，如 **LegalEntity**。</span><span class="sxs-lookup"><span data-stu-id="7327a-160">Select **Add Conditional Column**, and enter a name for the column, such as **LegalEntity**.</span></span> <span data-ttu-id="7327a-161">为该列输入条件，其中，如果 **msdyn\_contractorganizationalunitid.msdyn\_name** 为 \<组织单位\>，则 \<输入法人\>，否则为空。</span><span class="sxs-lookup"><span data-stu-id="7327a-161">Enter a condition for the column, where, if **msdyn\_contractorganizationalunitid.msdyn\_name** is \<organizational unit\>, then \<enter the legal entity\>; else null.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="7327a-162">数据集成中的模板映射</span><span class="sxs-lookup"><span data-stu-id="7327a-162">Template mapping in Data integration</span></span>

<span data-ttu-id="7327a-163">下图显示了数据集成中的模板任务映射的一个示例。</span><span class="sxs-lookup"><span data-stu-id="7327a-163">The following illustrations show an example of the template task mapping in Data integration.</span></span> <span data-ttu-id="7327a-164">此映射显示将从 Project Service Automation 同步到 Finance and Operations 的字段信息。</span><span class="sxs-lookup"><span data-stu-id="7327a-164">The mapping shows the field information that will be synchronized from Project Service Automation to Finance and Operations.</span></span>

<span data-ttu-id="7327a-165">[![模板映射](./media/ActualsMapping.jpg)](./media/ActualsMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="7327a-165">[![Template mapping](./media/ActualsMapping.jpg)](./media/ActualsMapping.jpg)</span></span>

<span data-ttu-id="7327a-166">[![模板映射](./media/TransactionConnections.jpg)](./media/TransactionConnections.jpg)</span><span class="sxs-lookup"><span data-stu-id="7327a-166">[![Template mapping](./media/TransactionConnections.jpg)](./media/TransactionConnections.jpg)</span></span>

## <a name="import-from-staging-table-after-integration-from-project-service-automation"></a><span data-ttu-id="7327a-167">从 Project Service Automation 集成后从暂存表导入</span><span class="sxs-lookup"><span data-stu-id="7327a-167">Import from staging table after integration from Project Service Automation</span></span>

<span data-ttu-id="7327a-168">将实际值从 Project Service Automation 同步到 Finance and Operations 之后，必须运行“从暂存表导入”定期流程。</span><span class="sxs-lookup"><span data-stu-id="7327a-168">The Import from staging table periodic process must be run after the synchronization of actuals from Project Service Automation to Finance and Operations.</span></span> <span data-ttu-id="7327a-169">此流程将把项目交易记录从暂存表导入 Project Service Automation 集成日记帐中，可在其中应用核算和过帐导入的交易记录。</span><span class="sxs-lookup"><span data-stu-id="7327a-169">This process will import the project transactions from the staging table into the Project Service Automation integration journal, where the accounting is applied and the imported transactions can be posted.</span></span> <span data-ttu-id="7327a-170">建议以批处理模式运行此流程，也可以选择将其设置为以重复执行的批处理运行。</span><span class="sxs-lookup"><span data-stu-id="7327a-170">We recommend that you run this process in batch mode and optionally can be set up to run as a recurring batch.</span></span>

## <a name="update-actuals-from-finance-and-operations"></a><span data-ttu-id="7327a-171">从 Finance and Operations 更新实际值</span><span class="sxs-lookup"><span data-stu-id="7327a-171">Update actuals from Finance and Operations</span></span>

### <a name="template-and-tasks"></a><span data-ttu-id="7327a-172">模板和任务</span><span class="sxs-lookup"><span data-stu-id="7327a-172">Template and tasks</span></span>

<span data-ttu-id="7327a-173">以下模板和基础任务用于将所过帐项目交易记录的凭证号和销售税从 Finance and Operations 同步到 Project Service Automation。</span><span class="sxs-lookup"><span data-stu-id="7327a-173">The following template and underlying tasks are used to synchronize the voucher number and sales taxes for posted project transactions from Finance and Operations to Project Service Automation:</span></span>

- <span data-ttu-id="7327a-174">**数据集成中的模板名称：** 项目实际值更新（Fin Ops 到 PSA）</span><span class="sxs-lookup"><span data-stu-id="7327a-174">**Name of the template in Data integration:** Project actuals update (Fin Ops to PSA)</span></span>
- <span data-ttu-id="7327a-175">**项目中的任务名称：**</span><span class="sxs-lookup"><span data-stu-id="7327a-175">**Name of the tasks in the project:**</span></span>

    - <span data-ttu-id="7327a-176">实际值</span><span class="sxs-lookup"><span data-stu-id="7327a-176">Actuals</span></span> 
    - <span data-ttu-id="7327a-177">TransactionConnections</span><span class="sxs-lookup"><span data-stu-id="7327a-177">TransactionConnections</span></span>

### <a name="entity-set"></a><span data-ttu-id="7327a-178">实体集</span><span class="sxs-lookup"><span data-stu-id="7327a-178">Entity set</span></span>

| <span data-ttu-id="7327a-179">Finance and Operations</span><span class="sxs-lookup"><span data-stu-id="7327a-179">Finance and Operations</span></span>                                   | <span data-ttu-id="7327a-180">Project Service Automation</span><span class="sxs-lookup"><span data-stu-id="7327a-180">Project Service Automation</span></span> |
|----------------------------------------------------------|----------------------------|
| <span data-ttu-id="7327a-181">项目实际值的集成实体</span><span class="sxs-lookup"><span data-stu-id="7327a-181">Integration entity for project actuals</span></span>                   | <span data-ttu-id="7327a-182">实际值</span><span class="sxs-lookup"><span data-stu-id="7327a-182">Actuals</span></span>                    |
| <span data-ttu-id="7327a-183">项目交易记录关系的集成实体</span><span class="sxs-lookup"><span data-stu-id="7327a-183">Integration entity for project transaction relationships</span></span> | <span data-ttu-id="7327a-184">交易记录连接</span><span class="sxs-lookup"><span data-stu-id="7327a-184">Transaction Connections</span></span>    |

### <a name="entity-flow"></a><span data-ttu-id="7327a-185">实体流</span><span class="sxs-lookup"><span data-stu-id="7327a-185">Entity flow</span></span>

<span data-ttu-id="7327a-186">项目实际值在 Project Service Automation 中管理，并同步到 Finance and Operations 中的项目集成日记帐。</span><span class="sxs-lookup"><span data-stu-id="7327a-186">Project actuals are managed in Project Service Automation, and they are synchronized to the project integration journal in Finance and Operations.</span></span> <span data-ttu-id="7327a-187">实际值在 Finance and Operations 中过帐之后，将在 Project Service Automation 中使用来自 Finance and Operations 的凭证号更新。</span><span class="sxs-lookup"><span data-stu-id="7327a-187">After actuals are posted in Finance and Operations, they are updated in Project Service Automation with the voucher number from Finance and Operations.</span></span> <span data-ttu-id="7327a-188">如果在 Finance and Operations 中添加了销售税，将在 Project Service Automation 中创建新的税金实际值。</span><span class="sxs-lookup"><span data-stu-id="7327a-188">If sales taxes were added in Finance and Operations, new tax actuals are created in Project Service Automation.</span></span>

### <a name="power-query"></a><span data-ttu-id="7327a-189">Power Query</span><span class="sxs-lookup"><span data-stu-id="7327a-189">Power Query</span></span>

<span data-ttu-id="7327a-190">在项目实际值更新模板中，必须使用 Power Query 才能完成以下任务：</span><span class="sxs-lookup"><span data-stu-id="7327a-190">In the project actuals update template, you must use Power Query to complete these tasks:</span></span>

- <span data-ttu-id="7327a-191">将 Finance and Operations 中的交易记录类型转换为 Project Service Automation 中的正确交易记录类型。</span><span class="sxs-lookup"><span data-stu-id="7327a-191">Transform the transaction type in Finance and Operations to the correct transaction type in Project Service Automation.</span></span> <span data-ttu-id="7327a-192">已经在项目实际值更新（Fin Ops 到 PSA）模板中定义了此项转换。</span><span class="sxs-lookup"><span data-stu-id="7327a-192">This transformation is already defined in the Project actuals update (Fin Ops to PSA) template.</span></span>
- <span data-ttu-id="7327a-193">将 Finance and Operations 中的计费类型转换为 Project Service Automation 中的正确计费类型。</span><span class="sxs-lookup"><span data-stu-id="7327a-193">Transform the billing type in Finance and Operations to the correct billing type in Project Service Automation.</span></span> <span data-ttu-id="7327a-194">已经在项目实际值更新（Fin Ops 到 PSA）模板中定义了此项转换。</span><span class="sxs-lookup"><span data-stu-id="7327a-194">This transformation is already defined in the Project actuals update (Fin Ops to PSA) template.</span></span>

### <a name="template-mapping-in-data-integration"></a><span data-ttu-id="7327a-195">数据集成中的模板映射</span><span class="sxs-lookup"><span data-stu-id="7327a-195">Template mapping in Data integration</span></span>

<span data-ttu-id="7327a-196">下图显示了数据集成中的模板任务映射的示例。</span><span class="sxs-lookup"><span data-stu-id="7327a-196">The following illustrations show examples of the template task mappings in Data integration.</span></span> <span data-ttu-id="7327a-197">此映射显示将从 Finance and Operations 同步到 Project Service Automation 的字段信息。</span><span class="sxs-lookup"><span data-stu-id="7327a-197">The mapping shows the field information that will be synchronized from Finance and Operations to Project Service Automation.</span></span>

<span data-ttu-id="7327a-198">[![模板映射](./media/ActualsUpdateMapping.jpg)](./media/ActualsUpdateMapping.jpg)</span><span class="sxs-lookup"><span data-stu-id="7327a-198">[![Template mapping](./media/ActualsUpdateMapping.jpg)](./media/ActualsUpdateMapping.jpg)</span></span>

<span data-ttu-id="7327a-199">[![模板映射](./media/TransactionConnectionsUpdate.jpg)](./media/TransactionConnectionsUpdate.jpg)</span><span class="sxs-lookup"><span data-stu-id="7327a-199">[![Template mapping](./media/TransactionConnectionsUpdate.jpg)](./media/TransactionConnectionsUpdate.jpg)</span></span>