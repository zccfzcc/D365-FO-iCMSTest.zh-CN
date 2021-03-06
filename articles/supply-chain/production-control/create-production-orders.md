---
title: 创建生产订单
description: 在创建生产订单时，将发起开始生产物料的请求。 生产订单包含与将生产的产品、生产数量和计划完工日期有关的信息。 它还包含要消耗的物料以及要用于生产物料的流程的信息。
author: johanhoffmann
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ProdTable, ProdTableCreate
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 19741
ms.assetid: bbb6e69d-479c-45fc-a0a8-66da5df16c7f
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: johanho
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 4989d5141ad983652ca4b3a047450dac33d7a85f
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "53430"
---
# <a name="create-production-orders"></a>创建生产订单

[!include [banner](../includes/banner.md)]

在创建生产订单时，将发起开始生产物料的请求。 生产订单包含与将生产的产品、生产数量和计划完工日期有关的信息。 它还包含要消耗的物料以及要用于生产物料的流程的信息。

生产订单在生产生命周期的各个阶段中传递。 在创建一个订单后，会将状态**已创建**分配给该订单。 在完成一个订单后，会将状态**已结束**分配给该订单。 每个阶段中的参数设置允许用户配置每个步骤。 可以为单个用户或为所有用户指定该设置。

生产物料清单和生产工艺路线是生产订单的主要实体。 它们基于要生产的选定物料和数量复制到生产订单。 在启动生产订单之前，生产物料清单和工艺路线是可以编辑的。

在以下情况下可以创建生产订单：

-   由主规划执行基于物料需求创建。
-   从销售订单行直接创建，或在创建和估计更高级别的生产订单（限定供应）时创建。
-   手动创建。




