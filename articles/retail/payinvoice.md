---
title: 设置付款发票方案
description: 本主题将介绍如何配置 Dynamics 365 for Retail 以支持与发票付款相关的各种方案。
author: josaw1
manager: AnnBe
ms.date: 11/14/2018
ms.topic: index-page
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: ''
ms.assetid: ed0f77f7-3609-4330-bebd-ca3134575216
ms.search.region: global
ms.search.industry: Retail
ms.author: josaw
ms.search.validFrom: 2018-11-15
ms.dyn365.ops.version: ''
ms.openlocfilehash: 543804a02f381b38cb8a8dc52d9eb0e20a3ae867
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "71222"
---
# <a name="set-up-pay-invoice-scenarios"></a><span data-ttu-id="51b09-103">设置付款发票方案</span><span class="sxs-lookup"><span data-stu-id="51b09-103">Set up pay invoice scenarios</span></span>

[!include [banner](includes/banner.md)]

<span data-ttu-id="51b09-104">Dynamics 365 for Retail 中的“付款发票”功能已扩展为支持：</span><span class="sxs-lookup"><span data-stu-id="51b09-104">The Pay invoice functionality in Dynamics 365 for Retail has been expanded to support:</span></span>
- <span data-ttu-id="51b09-105">单一 POS 交易中多个销售订单发票的结算。</span><span class="sxs-lookup"><span data-stu-id="51b09-105">Payoff of multiple sales order invoices in a single POS transaction.</span></span>
- <span data-ttu-id="51b09-106">各种客户发票类型的支付，包括普通发票、基于项目的发票和贷方通知单。</span><span class="sxs-lookup"><span data-stu-id="51b09-106">Payment of various customer invoice types including free text invoices, project-based invoices, and credit notes.</span></span>

<span data-ttu-id="51b09-107">要启用这些方案，必须按如下所述配置商店的功能配置文件。</span><span class="sxs-lookup"><span data-stu-id="51b09-107">To enable these scenarios, the functionality profile for stores must be configured as outlined in below.</span></span>  

1. <span data-ttu-id="51b09-108">转到 **Retail > 渠道设置 > POS 设置 > POS 配置文件 > 功能配置文件**，然后选择与您要更改的商店相链接的配置文件。</span><span class="sxs-lookup"><span data-stu-id="51b09-108">Go to **Retail > Channel setup > POS setup > POS profiles > Functionality profiles** and select a profile that's linked to the stores that you want to make the changes for.</span></span>

1. <span data-ttu-id="51b09-109">在**功能**选项卡上，根据需要配置以下参数。</span><span class="sxs-lookup"><span data-stu-id="51b09-109">On the **Functions** tab, configure the following parameters as needed.</span></span>

    - <span data-ttu-id="51b09-110">**销售订单发票** - 选择**是**以允许用户在单一 POS 交易中支付一个或多个基于销售订单的发票。</span><span class="sxs-lookup"><span data-stu-id="51b09-110">**Sales order invoice** - Select **Yes** to allow users to pay one or more sales order-based invoices in a single POS transaction.</span></span>

    - <span data-ttu-id="51b09-111">**普通发票** - 选择**是**以允许用户在单一 POS 交易中支付一个或多个普通发票。</span><span class="sxs-lookup"><span data-stu-id="51b09-111">**Free text invoice** - Select **Yes** to allow users to pay one or more free text-based invoices in a single POS transaction.</span></span>

    - <span data-ttu-id="51b09-112">**项目发票** - 选择**是**以允许用户在单一 POS 交易中支付一个或多个基于项目的发票。</span><span class="sxs-lookup"><span data-stu-id="51b09-112">**Project invoice** - Select **Yes** to allow users to pay one or more project-based invoices in a single POS transaction.</span></span>

    - <span data-ttu-id="51b09-113">**销售订单贷方通知单** - 选择**是**以允许用户针对未结发票结算多个基于销售订单的贷方通知单，或者向未结贷方通知单的客户处理退款。</span><span class="sxs-lookup"><span data-stu-id="51b09-113">**Sales order credit note** - Select **Yes** to allow users to settle multiple sales order-based credit notes against open invoices or process a refund to the customer for an open credit note.</span></span>

> [!NOTE]
> <span data-ttu-id="51b09-114">尚不支持对部分金额进行支付或结算。</span><span class="sxs-lookup"><span data-stu-id="51b09-114">Payment or settlement of partial amounts is not yet supported.</span></span>
