---
title: 合并的批次订单
description: 本文介绍合并的批次订单的概念。
author: ShylaThompson
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: PmfAddToConsOrder, PmfBulkItemConv, PmfBulkPackOnHand, PmfConsOrderListPage
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 19291
ms.assetid: e97f1d3d-1306-4c42-b2bc-d1755fe574d5
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: shylaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 1a78c407980187c9f516f3d57455dc0890ffc489
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55655"
---
# <a name="consolidated-batch-orders"></a>合并的批次订单

[!include [banner](../includes/banner.md)]

本文介绍合并的批次订单的概念。

生产的散装物料被视为父物料，而包装的物料被视为子物料。 散装物料和包装物料之间的关系以散装物料转换表示。 此散装物料转换在散装物料本身上定义。  

包装的物料可包装到被视为一个单位的单个大小或多个大小的容器中。 通过合并散装物料的订单，您可以在单个视图中查看所有相关的批次订单，这些订单可帮助您确定任何必须完成的剩余工作。  

合并的批次订单可以包含以下订单的任意组合：

-   单个散装物料订单和多个包装物料订单
-   多个散装物料订单和多个包装物料订单
-   多个散装物料订单和单个包装物料订单
-   仅包装物料订单




