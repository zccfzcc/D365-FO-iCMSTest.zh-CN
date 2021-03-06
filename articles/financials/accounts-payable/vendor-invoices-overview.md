---
title: 供应商发票概览
description: 本文提供有关供应商发票的一般信息。 供应商发票收到的产品和服务的付款请求。 供应商发票可以表示正在进行中的服务的帐单，也可以基于特定物料和服务的采购订单。
author: ShivamPandey-msft
manager: AnnBe
ms.date: 01/10/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: VendorInvoiceWorkspace, VendInvoiceInfoListPage
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 13971
ms.assetid: 0ec4dbc0-2eeb-423b-8592-4b5d37e559d3
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 420ee8fbae6e500105da2e7ddb75495d413b82c6
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55268"
---
# <a name="vendor-invoices-overview"></a>供应商发票概览

[!include [banner](../includes/banner.md)]

本文提供有关供应商发票的一般信息。 供应商发票收到的产品和服务的付款请求。 供应商发票可以表示正在进行中的服务的帐单，也可以基于特定物料和服务的采购订单。 

<a name="vendor-invoices"></a>供应商发票
---------------

采购订单中的供应商发票是在根据对供应商下达的采购订单收到产品或服务时生产的发票。 供应商发票包含一个标题以及一个或多个物料或服务行。 供应商发票完成从采购订单到物料收货到供应商发票的周期。 

尽管某些供应商发票连接到采购订单，但供应商发票还可以包含不对应于采购订单行的行。 您还可以创建与任何采购订单都没有关联的供应商发票。 这些供应商发票可能代表正在进行中的服务，例如电费单，并且您不必在添加它们时参考采购订单。 

有多种方式来输入供应商发票：

-   供应商发票登记簿能让您快速输入不引用采购订单的发票，因此，您可以计入费用。 通过使用供应商发票审核日记帐，您可以选择这些发票并将其过帐到供应商余额以冲销应计。
-   供应商发票日记帐能让您仅用一个步骤即可快速输入不引用采购订单的发票。
-   与供应商发票池一起，供应商发票登记簿能让您快速输入发票以计入费用。 您可以以后打开关联的采购订单以比对支出帐户过帐发票。
-   **打开供应商发票**和**待定供应商发票**页能让您从已确认的采购订单创建供应商发票。

以下讨论提供有关如何使用**未结供应商发票**或**待定供应商发票**页从采购订单创建供应商发票的详细信息。

## <a name="understanding-invoice-line-quantities"></a>了解发票行数量
当从相关采购订单中打开供应商发票时，会从采购订单创建发票行。 默认情况下，会从产品收货数量中减去此数量。 但是，您可以使用以下任何默认行为：

-   **当前接收量** – 对部分装运使用此选项。 **数量**字段中的默认值来自采购订单上的**当前接收量**。
-   **订购数量** – 对整个装运使用此选项。 **数量**字段中的默认数量来自采购订单上的**订购数量**。
-   **登记数量** – 如果物料需要登记，则使用此选项，如在**物料模型组**页上指定的一样。 **数量**字段中的默认值是已登记的实际更新数量。
-   **产品收据数量** – 如果已经针对订单收到了产品收据，则使用此选项。 **数量**字段中的默认值来自可用产品收据的总数量。
-   **已注册数量和服务** – 如果已经针对已库存或未库存的物料在到达日志中登记数量，则使用此选项。 此选项还包括服务（无论是否登记）。

如果您的法人使用发票匹配，您可以在**产品收据数量匹配**列中查看数量匹配的结果。 您还可以使用**检查**选项卡上的**匹配详细信息**菜单命令查看数量匹配的结果。

## <a name="adding-a-line-that-wasnt-on-the-purchase-order"></a>添加不在采购订单上的行
您可以将不在采购订单上的行添加到供应商发票。 您必须选择物料编号或采购类别。 您可以向该行添加数量、价格和金额。 该行将仅包括在发票合计的匹配政策中。

## <a name="submitting-a-vendor-invoice-for-review"></a>提交供应商发票，以供审核
您的组织可以使用工作流来管理供应商发票的审核流程。 可能需要对发票抬头、发票行或两者进行工作流审核。 工作流控件适用于抬头或行，具体取决于单击该控件时焦点的位置。 您将看到的不是**过帐**按钮，而是**提交**按钮，您可以使用它来通过审核流程发送供应商发票。

## <a name="matching-vendor-invoices-to-product-receipts"></a>将供应商发票与产品收据匹配
您可以输入和保存供应商发票的信息，您还可以将发票行匹配产品收据行。 如果需要，还可以匹配行的部分数量。 

您可以创建基于迄今已接收的产品收据行物料的供应商发票，即使尚未接收特定采购订单的所有物料。 例如，如果供应商每个月发送一张支票，该供应商支票涵盖您在该月中发运的所有交货，则可以使用此选项。 每个产品收据都表示该采购订单上物料的部分或全部交货。 

在您过帐该发票时，每个物料的**未开票数量**都用来自所选产品收据的已收货数量的总数更新。 如果采购订单上所有物料的**未开票数量**和**剩余交货量**均为 0（零），则该采购订单的状态将更改为**已开票**。 如果**未开票数量**不为 0，则该采购订单的状态将不更改，并且可为其输入其他发票。

此选项假定为该采购订单至少过帐了一个产品收据。 供应商发票基于这些产品收据并反映来自这些装箱单的数量。 该发票的财务信息基于在您过帐该发票时输入的信息。

有关详细信息，请参阅[记录供应商发票和匹配接收的数量](../accounts-receivable/tasks/record-vendor-invoice-match-against-received-quantity.md)。

## <a name="working-with-multiple-invoices"></a>使用多个发票

您可以同时处理多张发票以及同时全部过帐。 如果您必须创建多个发票，请使用**待定供应商发票**页。 如果您必须过帐和打印多个供应商发票，请使用发票审核日记帐页。 如果您使用发票审核日记帐，则必须针对该采购订单过帐至少一个产品收据，并且在发票登记簿中必须过帐该采购订单的发票。 该发票的财务信息来自在该发票登记簿中已过帐的发票。


有关详细信息，请参阅: 

 - [设置供应商发票策略](../accounts-receivable/tasks/set-up-vendor-invoice-policies.md) 

 - [使用供应商发票将发票数据键入应付账款](tasks/key-invoice-data-ap-system-vendor-invoice.md)

 - [使用审核日记帐将发票数据键入应付帐款](tasks/key-invoice-data-into-ap-system-approval-journal.md)

 - [使用发票池将发票数据键入 AP 系统](tasks/key-invoice-data-into-ap-system-invoice-pool.md)

 - [在发票日记帐中记录供应商发票](tasks/record-vendor-invoice-invoice-journal.md)

