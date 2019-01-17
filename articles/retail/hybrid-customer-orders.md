---
title: 混合客户订单
description: 混合客户订单是一份订单，其中包含客户可以从店内自提的产品，以及以后将拣货或装运的产品。
author: josaw1
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 261164
ms.assetid: 9d99a5b9-4662-499a-bece-3ea1d6092934
ms.search.region: global
ms.search.industry: Retail
ms.author: anpurush
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: 126e4db266e9ecb7ded9028c7cf0674f28aa8f1c
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54378"
---
# <a name="hybrid-customer-orders"></a>混合客户订单

[!include [banner](includes/banner.md)]

混合客户订单是一份订单，其中包含客户可以从店内自提的产品，以及以后将拣货或装运的产品。

在 Microsoft Dynamics 365 for Retail 中，可以为客户订单选择自提所有产品，或自提选定产品。 创建订单后，自动为标记为自提的产品行开票，同样，创建订单后也会为待拣货的订单自动开票。 混合订单中的应付款金额通过添加带自提行金额的拣货和装运产品行中的保证金百分比确定。 对于混合订单，系统按照以下方式在客户订单模式与现金提货模式之间切换：

-   如果购物车中的所有产品设置为**自提交货**，将把订单作为现金提货交易记录处理。
-   如果购物车中的任何或所有行设置为**拣货**或**装运交货**，订单将作为客户订单交易记录处理。

如果某个购物车行已选中并选中了**领取所选项**、**装运所选产品**或**完成所选产品**，则仅使用该交货方法设置这个特定购物车行。 在这种情况下，工序的下游流程照常继续。 但是，如果选中了**领取所选项**、**装运所选产品**或**完成所选产品**但未选中购物车行，将打开一个新页面，其中列举所有购物车行。 在该屏幕上，可以一次选择多行以设置交货方法。 使用该方法选择行时，将覆盖已分配给该行的上述任何交货方法。

<a name="additional-resources"></a>其他资源
--------

[客户订单概览](customer-orders-overview.md)


