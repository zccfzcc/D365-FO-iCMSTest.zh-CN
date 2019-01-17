---
title: 调整现有库存量成本价值
description: 使用”现有库存量调整“页调整库存结转流程运行后的现有库存量数量的成本价值。
author: AndersGirke
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: InventAdjInventOnHand
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 53231
ms.assetid: bc1fde9f-5ad9-4339-8ae8-e2839b792eb2
ms.search.region: Global
ms.search.industry: Manufacturing
ms.author: aevengir
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: b310ea3b05db19e0c9388337c2d1304be755d0ee
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55760"
---
# <a name="adjust-on-hand-inventory-cost-values"></a>调整现有库存量成本价值

[!include [banner](../includes/banner.md)]

使用”现有库存量调整“页调整库存结转流程运行后的现有库存量数量的成本价值。

您可以使用**现有库存量调整**页调整库存结转流程运行后的现有库存量数量的成本价值。 **Note:** To open the **Adjustment of on-hand inventory** page, on the **Closing and adjustment** page, select the record of a completed inventory close process, and then click **Adjustment** &gt; **On-hand**. **示例：** 您在 2 月份具有以下交易记录：

-   2 月 1 日：以 10.00 美元的成本有数量为 2 的库存财务收货
-   2 月 5 日：以 13.00 美元的成本有数量为 1 的库存财务收货
-   2 月 19 日：以 11.00 美元的移动平均成本有数量为 1 的库存财务发货

此物料以先进先出 (FIFO) 库存模型设置，并在 2 月 28 日结转库存。 11.00 美元的财务发货交易记录将对照 2 月 1 日的财务收货结算，并将做 1.00 美元的调整。 以下库存收货将包含未结库存数量：

-   2 月 1 日：成本为 10 美元的数量 1
-   2 月 5 日：成本为 13.00 美元的数量 1

若要将这两个物料的成本设置为 USD 15.00，请使用现有量调整选项来调整截至最后库存结转期间的未结现有数量。 **注意：** 现有量调整交易记录的过帐日期将是上一次库存结转的日期。 不能修改此日期。