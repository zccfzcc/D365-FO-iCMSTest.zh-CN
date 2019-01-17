---
title: 商店订单履行
description: 此主题概要介绍了商店订单履行。
author: rubencdelgado
manager: AnnBe
ms.date: 10/30/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
ms.search.form: RetailStoreTable, RetailTillLayout
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.search.region: Global
ms.search.industry: retail
ms.author: rubencdelgado
ms.search.validFrom: 2017-10-30
ms.dyn365.ops.version: ''
ms.openlocfilehash: 30cfac9462616cbc81ec6e193488b5adde4e8f04
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56196"
---
# <a name="store-order-fulfillment"></a>商店订单履行

[!include [banner](includes/banner.md)]

许多零售商希望通过让商店填写订单的方式优化订单履行。 商店级别的订单履行有助于缓解特定商店的存货过剩情况，或者当商店产能过剩或与客户之间的装运距离较短时，从物流的角度而言具有必要性。 为了解决此需求，在销售点提供了统一订单履行操作。

要在特定商店履行的订单在订单标头或行上指定了商店的仓库。 

销售点中的订单履行操作是销售点中用于处理订单的一个统一工作区。 这里包括从接受订单，到将订单标记为已装运或发起商店提货在内的一切操作。 

## <a name="access-unified-order-fulfillment-in-the-point-of-sale"></a>访问销售点中的统一订单履行

订单履行[操作 ID 928](https://docs.microsoft.com/en-us/dynamics365/unified-operations/retail/pos-operations) 可用于访问销售点中的商店订单履行工作区。 

订单履行操作没有自己现成的权限，但用户将来可以使用**允许检索订单**权限从销售点调用操作。

在商店级别，配置设置可用于确定是否应手动接受来自销售点内部的订单行。 如果未设置该配置选项，将默认接受订单行。 如果已启用该配置选项，销售点的用户需选择**允许接受订单**权限，以便接受来自销售点内部的订单。
也可拒绝来自销售点的订单行。 拒绝订单行表示不会在该商店履行该订单行，并且会将该订单行发回去，以重新分配到另一个商店或仓库。 订单行拒绝权限通过**允许订单拒绝**权限授予。 

## <a name="order-fulfillment-operation-parameters"></a>订单履行操作参数

订单履行提供现成的参数，在销售点中调用操作时可将这些参数应用到操作。 如果配置了**所有订单**参数，在使用操作时将显示所有订单。 **要装运的订单**参数仅显示必须从商店装运的订单，**要提货的订单**显示将在商店内提货的订单。 

## <a name="orders-for-fulfillment"></a>要履行的订单

订单履行操作仅显示要在当前商店提货或要从当前商店装运的订单。 使用订单履行操作时，不会列出要供其他商店履行的订单。 

## <a name="line-selection"></a>行选择

使用操作窗格中的**选择**功能可以选择行。 如果启用了**选择**，可以选择多行进行处理。 再次单击相同行可以清除选定行。 

## <a name="line-details"></a>行明细

使用行明细弹出菜单可以显示行明细。 使用此菜单时，提供三个选项卡，以显示选定行的额外信息。 第一个选项卡，**行明细**，显示行本身的详细信息，例如订购的数量和剩余数量。 提供的其他详细信息包括领料数量、包装数量、开票数量以及交货方式和交货地址。 **订单明细**选项卡提供订单头信息，包括客户、客户 ID、订单编号、订单合计和余额。 **库存**选项卡根据物理可用库存、保留库存和已订购库存显示所选行的信息。

如果选择了多行，订单行明细弹出菜单将仅指示已选择多行。 若要显示某一行的详细信息，则取消选中行，直到仅有一行被选中。 

## <a name="pending-order-lines"></a>待处理的订单行

统一订单履行包括手动接受订单的功能。 默认情况下，已经接受要在本商店履行的订单。 但如果业务流程指示本商店级别的工作人员必须接受订单，可以在零售商店级别启用手动接受。 要启用订单接受，转到**零售** > **渠道** > **零售商店** > **所有零售商店**。 打开需要的商店，在**常规**选项卡上找到**订单履行**子标题。 该子标题有一个**手动接受**选项已默认设定为**否**。 将此选项设定为**是**并将更改同步到渠道数据库后，订单行可完成接受流程。

拥有**允许接受订单**权限的工作人员可以打开订单履行并选择要接受的行。 一旦接受行后，其状态从**挂起**更改为**已接受**，并且可以继续完成订单履行流程的其余部分。 如果启用了**手动接受**，则需在接受订单后才会处理订单。 

用于商店提货的订单永远都不会处于**挂起**状态。 这样做是为了避免出现这样的情况：当客户到达商店时，由于拥有相关权限的工作人员不在，而导致无法处理订单行。

## <a name="accepted-order-lines"></a>已接受的订单行

行状态为**已接受**的订单可以继续在销售点完成订单履行流程的其余部分。 接受订单后，可以对该订单行执行任何其余操作。 

例如，可以选择已接受的订单行，然后直接提货，无需进行领料和包装。

## <a name="line-actions"></a>行操作

### <a name="pick"></a>领料

The  **Pick** category of actions is provided to aid in the process of picking order lines from shelves. 只能对之前已经接受的订单行执行领料操作。 

**操作：领料**

- 生成的 POS 状态：领料
- 生成的后端办公系统状态：无更改

一旦接受订单后，可以选择行并标记为**领料**。 将行标记为**领料**是指示已经开始对行执行领料工作的一种方式。 这样可以防止两名工作人员试图同时对相同的订单行领料。  

**操作：打印领料单**

- 生成的状态：领料
- 生成的后端办公系统状态：无更改

可以在销售点打印领料单，以便协助工作人员执行领料过程。 工作人员领料时可以携带打印的领料单，并且在领取产品时，工作人员将在领料单上手动标记为已领料。 

领料单格式在 Dynamics 365 for Retail 上进行配置并添加到收据模板中。 有关设置收据模板的详细信息，请参阅[收据模板和打印](https://docs.microsoft.com/en-us/dynamics365/unified-operations/retail/receipt-templates-printing)。

如果选择了行并打印了这些行的领料单，会自动将其更新为**领料**状态。 

**操作：标记为已领料**

- 生成的状态：已领料或部分领料
- 生成的后端办公系统状态：已领料或部分领料

在执行实际领料流程后，可以将行标记为**已领料**。 选择行并将其标记为**已领料**会执行一个实时调用，以更新 Dynamics 365 for Retail 中的订单行。 在销售点将行标记为**已领料**后，后端办公系统的状态也会更新为**已领料**，且库存交易记录反映指定的数量已递减。

在一段时间内处理订单时，可以处理特定行的部分数量。 如果选择了一行并执行了**标记为已领料**操作，而且数量大于 1，则系统会提示用户输入数量。 系统将自动填充要领取的剩余数量。 如果指定的数量少于剩余数量，行的状态变为**已部分领料**。 在后端办公系统更新订单行时，它还将反映部分领料状态，并使用用户输入的数量进行库存更新。 

如果订单行领料错误，必须在后端办公系统对订单行执行取消领料流程。 销售点目前不支持取消领料操作。 

可以选择来自不同订单的订单行、标记为**领料**、打印在相同领料单上或标记为**已领料**。 

### <a name="pack"></a>包装

接受订单行后，可以在任何时间点对订单行进行包装。 

**操作：打印装箱单**

- 生成的状态：已包装或部分包装
- 生成的后端办公系统状态：已交货或部分交货

此操作将行标记为已包装或部分包装并打印装箱单。 可以打印装箱单以核实包装在一起的产品。 装箱单格式在 Dynamics 365 for Retail 上进行配置并添加到收据模板中。 有关设置收据模板的详细信息，请参阅[收据模板和打印](https://docs.microsoft.com/en-us/dynamics365/unified-operations/retail/receipt-templates-printing)。

**操作：标记为已包装**

- 生成的状态：已包装或部分包装
- 生成的后端办公系统状态：已交货或部分交货

**标记为已包装**操作可用于指示对行进行包装，而不打印装箱单。 **打印装箱单**和**标记为已包装**都会在后端办公系统产生库存交易记录。 销售点中的装箱行可能导致在后端办公系统中生成装箱单日记帐。 

如果订单行包装出现错误，必须在后端办公系统更正装箱单日记帐。 

只能同时包装位于相同订单上且具有相同交货方式的行。

目前，将商店提货行标记为**已包装**的选项被禁用。 在将来的版本中将增加该功能。 装箱单创建流程将得到增强，以支持将第三方装运信息注入到装箱单流程中。

### <a name="pick-up"></a>领料

用于商店提货的订单在销售点中检索到后，可以直接提货。 商店提货订单无需接受。 

**操作：提货**

- 生成的状态：已开票或部分开票
- 生成的后端办公系统状态：已开票或部分开票

如果从统一订单履行中选中用于提货的行，整个订单将被载入到销售点，且标记选定行的全部数量。 该订单上的其他行也被载入到该销售点的交易记录视图中，但数量标记为零。 

用于提货的行载入到交易记录视图中后，可以照常支付交易记录。 

已通过提货完全开票的行不再显示在统一订单处理中。 已部分提货的行将继续显示在统一订单履行中，直到全部提货。 

如果某行提货错误，必须执行退货以更正错误。  

只能同时对位于相同订单上且具有相同交货方式的行提货。 

### <a name="shipping"></a>装运

使用**装运**操作进行统一订单履行只能处理从商店装运的订单行。 如果在渠道级别配置了手动接受订单行，必须在装运前接受订单。 订单行被接受并处于**挂起**或其他状态后，可以对行进行装运。 

**操作：装运**

- 生成的状态：已开票或部分开票
- 生成的后端办公系统状态：已开票或部分开票

从统一订单履行装运的行从后端办公系统开票，类似于从后端办公系统直接对订单开票。 从统一订单履行装运的行不会载入到交易记录视图中，且在装运行时不会进行支付。 

已完全装运的订单行不会再显示在统一订单履行中。 已部分装运的行将继续显示在统一订单履行中，直到全部装运。 

只能同时装运来自相同订单的行。 如果来自相同订单的行具有不同的交货方式，仍然可以选中这些行进行同时装运。 

### <a name="reject"></a>拒绝

可以拒绝行或部分行。 可以从后端办公系统将它们重新分配到另外一个商店或仓库。 只有尚未领料或包装的行才可以被拒绝。 要拒绝已领料或包装的行，必须从后端办公系统对该行取消领料或取消包装。 

**操作：拒绝**

- 生成的状态：拒绝
- 生成的后端办公系统状态：无更改 

从**销售订单处理和查询**工作区可以查看被拒绝的订单行。 清除工作区上的人员筛选器可以查看所有商店的所有被拒绝的订单行。 **订单和收藏**部分下的**拒绝的订单行**显示订单行详细信息。 此外，用户单击**摘要**部分下的**拒绝的订单行**按钮可以导航到销售订单视图。 这将显示包含一个或多个被拒绝的订单行的所有订单。 如果启用了“配送的订单管理”(DOM)，这些被拒绝的订单将被自动重新分配到适当的商店进行履行，但是也可手动重新分配这些订单行。 若要执行此操作，请选择**履行状态**显示为**已拒绝**的行并根据需要更改站点/仓库。 单击**更新行**下拉菜单并单击**重置履行状态**可以根据订单履行设置将履行状态从**已拒绝**更改为**已接受**或**挂起**。 重置履行状态后，商店工作人员可以查看 POS 中的订单行。

## <a name="line-quantity-tracking"></a>行数量跟踪

数量大于 1 的单个订单行可以在一段时间内进行处理，因而使订单行具有多个子状态。 例如，如果有一个建筑商有一个项目需要 500 个电路板，但该建筑商在项目过程中一次性只领取或交付几个电路板，就会同时存在领料、包装和装运的数量。 

无论在任何时候选中一行，都会假定正在处理该行的剩余数量而自动填充该剩余数量。 按照上述例子，如果已经领取了 200 个电路板，且选中电路板行进行领料，则在数量中将自动填充剩余的 300 个数量。 如果已经对 200 个电路板开票，也是一样的情况。 在这种情况下，只会自动填充剩余数量。 

继续上一个例子，如果有 200 个电路板标记为已包装，并选中装运，则会自动填充全部数量，500。 如果只有 200 个电路板装运，系统将假定要装运之前包装的电路板，因此会减少包装的数量。 如果有 201 个电路板装运，将先减少包装的电路板，从剩余数量中减少最后一个剩余的电路板。 

## <a name="line-statuses"></a>行状态

销售点中的订单行具有多个状态来反映该订单行的状态。 销售点和后端办公系统中的状态并非总是一致。 通过销售点使用订单履行操作可以查看订单行状态。 在后端办公系统中，可以从订单明细中查看订单行。 通过**零售** > **客户** > **所有客户订单**可以访问订单详细信息。 选择**订单 ID** 可以查看订单详细信息。 从订单明细中选择**销售订单**选项卡，然后选择**查看**子标题下的**详细状态**。 

**挂起** - 已分配到商店但尚未接受的订单行在销售点进行查看时的状态为**挂起**。 等待销售点接受的行在后端办公系统中的状态为**订单处理中**。

**已接受** - 已手动接受或自动接受的订单行在销售点中进行查看时的状态为**已接受**。 具有**已接受**状态的行在后端办公系统中将显示为**订单处理中**。

**领料** - 目前正在商店级别领料的行的状态为**领料**。 这些相同的行在后端办公系统进行查看时将显示为**订单处理中**。

**已领料**和**已部分领料** - 已经在销售点领料或部分领料的行的状态为**已领料**或**已部分领料**。 相同的行在后端办公系统中也将显示为**已领料**或**已部分领料**。

**已包装**和**已部分包装** - 已经在销售点包装或部分包装的行的状态为**已包装**或**已部分包装**。 相同的行在后端办公系统中也将显示为**已交货**或**已部分交货**。

**已部分开票** - 已经部分提货或部分装运的行在销售点和后端办公系统中的状态均为**已部分开票**。

**已开票** - 已经在销售点完全开票的行将不再显示为可供履行。 这些行在后端办公系统中的状态为**已开票**。

## <a name="order-fulfillment-filtering"></a>订单履行筛选

在销售点的订单履行包括筛选，以帮助用户轻松找到他们需要的东西。 通过**销售点**屏幕底部的操作窗格可以更改筛选器。 默认情况下，根据设置的操作方式应用**交货类型**筛选器。 如果使用**所有订单**参数设置操作，则在访问订单履行时应用该筛选器。 相同的规则适用于**商店提货**和**从商店装运**参数。 可以应用到订单履行视图的其他筛选器包括：

  - 客户编号
  - 客户名称
  - 客户电子邮件
  - 转移单编号
  - 交货方式
  - 收据编号
  - 渠道引用 ID
  - 源商店编号
  - 行状态
  - 创建日期
  - 交货日期
  - 接收日期