---
title: 固定资产集成
description: 固定资产可以与总帐、库存管理、应收账款和应付账款一起集成。 您也可以设置固定资产，以便与采购订单相集成。
author: ShylaThompson
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: AssetTable
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 3501
ms.assetid: f0639053-d99c-432a-8ead-5c26e0d4eaec
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 1e0d2cc15422c921ff0ef05da66d05340d5500c5
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54338"
---
# <a name="fixed-assets-integration"></a>固定资产集成

[!include [banner](../includes/banner.md)]

固定资产可以与总帐、库存管理、应收账款和应付账款一起集成。 您也可以设置固定资产，以便与采购订单相集成。

<a name="general-ledger"></a>总帐
--------------

在总帐中，所有固定资产的值通常都汇总到进行财务报告时所需的多个主科目。 但是，在**固定资产**页中，您可以创建许多固定资产记录。 这些记录可以包含诸如购置价格、折旧和评估等信息。 只要过帐固定资产的交易记录，就会更新相应的主科目。 固定资产的主科目始终显示固定资产的更新值。

在**固定资产过帐模板**页中，定义固定资产帐簿交易记录过帐到的主科目。 您还可以指定过账到每个主科目的固定资产交易记录的类型。 您可以创建固定资产主科目的各种组合，具体情况视总帐中固定资产所需的明细级别而定。 主科目可以基于交易记录类型、帐簿和其他主科目。

## <a name="inventory-management"></a>库存管理
在固定资产的库存日志中，您可以输入法人具有为自身生产或构建固定资产的购置。 您可以将库存物料转移到固定资产，或者将库存物料作为购置或购置的一部分。 

您也可以使用采购订单购置资产。 在采购订单包含指定为固定资产的库存物料时，**固定资产**页中的**允许从采购中购置资产**选项的设置确定在过帐发票时是否为固定资产过帐购置。 固定资产购置对库存的影响取决于法人的设置。 

如果库存物料通过库存日志、采购订单或购置方案变为固定资产购置，将会创建一个固定资产帐簿购置交易记录。 如果帐簿购置包括衍生帐簿，也会创建衍生帐簿购置交易记录。 

在库存管理的**过帐**页中设置的过帐规则控制在过帐购置时库存的减少。 但是，在您过帐与固定资产相关的发票时，不会始终减少库存。 在某些情况下，固定资产可能会出于内部使用目的而采购。 示例是为销售部门采购的笔记本电脑。 在您处理采购订单时，可以使用为经销以及内部使用目的而设置的物料。 

如果您在固定资产的物料组上使用特定的收货和发货帐户，则可以使用相同的库存物料来同时用于内部采购和作为经销存货。 

设置供内部使用的固定资产，以便具有**固定资产收货**帐户类型。 此账户类型用于跟踪固定资产的收货。 在过帐供应商发票时，如果以下条件为真，使用固定资产收货帐户：

-   发票行包含供内部使用的现有固定资产。
-   为已过帐的产品收据行选中**是否新建固定资产？** 复选框。
-   为供应商发票行选择**创建新的固定资产**复选框。

此帐户通常是支出帐户。 通过使用**物料组**或**过帐**页中的**采购订单**选项卡，您可为物料组或单独的物料设置**固定资产收货**帐户类型。

同样，可以设置供内部使用的固定资产，以便具有**固定资产发货**帐户类型。 此账户类型用于跟踪收据的固定资产的签发。 在使用采购订单购置资产时，该固定资产发货帐户抵销固定资产借方账户。 在您过帐供货商发票或在固定资产日记帐中过帐该资产购置时，可以通过使用购置方案过帐资产购置。 通过使用**物料组**或**物料过帐**页中的**库存**选项卡，您可为物料组或单独的物料设置**固定资产发货**帐户类型。 

最终，用于过帐的主科目由该选项为物料模型组指定的分类帐集成确定。 此外，使用的主科目各不相同，取决于是否将资产分配到采购订单行。 这些会计科目从用于各个物料组的过帐模板派生。 
**注意：** 在产品收据过帐后，如果存在某一库存预留，则您不能分配固定资产或从该行创建固定资产。 

固定资产交易记录要过帐到的账户取决于该资产是由法人采购还是由法人构建，还取决于该资产的交易记录类型。 

通过交易记录类型可以在库存交易记录与固定资产中的过帐模板之间建立联系。 因为固定资产中的过帐模板定义了更新的科目，所以，对固定资产交易记录类型的选择也会间接影响对交易记录过帐到的主科目的选择。 对于构建和采购的固定资产，交易记录类型通常是**购置**或**购置调整**。

## <a name="accounts-receivable"></a>应收账款
具有应收账款的固定资产集成使用固定资产中设置的过帐模板。 在过账客户发票前，为该客户发票选择固定资产、帐簿和固定资产交易类型时，启用这些过帐模板。 因为固定资产不是库存管理的一部分，在出售固定资产时您必须使用**普通发票**页面。 

如果帐簿包括衍生帐簿，过帐客户发票时，会创建衍生帐簿交易记录。

## <a name="accounts-payable"></a>应付账款
固定资产通常向外部供应商购置。 您可以使用**固定资产参数**页指定在过帐供应商发票时是否始终过帐资产购置，或者是否只能从固定资产过帐资产购置。 如果您启用从应付账款过帐资产购置，则只要过帐某一固定资产购置的供应商发票，就会更新固定资产科目。 

如果将该系统设置为在过帐发票时的过帐资产购置，则交易记录将根据固定资产中用于不同固定资产交易记录类型设置过帐模板进行过帐。 在过帐供应商发票之前，该过帐由在**采购订单**页中选择的固定资产、帐簿和固定资产交易记录类型控制。 

如果帐簿包括衍生帐簿，过帐供应商发票时，会创建衍生帐簿交易记录。

每个订单行的集成在**采购订单**页的**行明细**快速选项卡的**固定资产**选项卡中激活。 您可以发送固定资产的采购订单到供应商。 但是，仅当您过账供应商发票时接受固定资产后，才更新固定资产和主科目。 因为采购订单只能包含库存物料，固定资产购置对库存的影响取决于法人的设置。

## <a name="project-management-and-accounting"></a>项目管理与核算
您可以将某一项目与受该项目影响的资产相关联。 您还可以将各个阶段、任务或下级项目与不同的资产相关联。 一个资产可与每个项目记录关联。 当您在**项目**页的**固定资产**编号字段中输入某一固定资产编号时创建该关联。 项目类型必须为**内部**或**成本项目**。 

您还可以使用**项目**页查看与项目相关联的资产的有关详细信息。 若要查看固定资产记录，请单击**设置**快速选项卡上的资产链接，以打开**固定资产**页。 然后单击**项目** &gt; **所有项目**以查看与固定资产相关联的项目。 

在项目与针对固定资产的工作、维护或改进相关时，您通常将固定资产与这些项目相关联。 在完成项目时，不自动为该资产创建调高。 因此，如果需要调高，您必须手动创建。 

若要删除项目和资产之间的关联，请在**项目**页中取消选中**固定资产编号**字段。 

您还可以将您正创建或制造的固定资产设计为评估项目的一部分。 在某一评估项目结束时，您可以自动过帐资产购置交易记录。

有关详细信息，请参阅[通过采购购置资产](acquire-assets-procurement.md)


