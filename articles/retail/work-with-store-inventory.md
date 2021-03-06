---
title: 商店库存管理
description: 本文描述可用于管理库存的文档类型。
author: rubencdelgado
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 21391
ms.assetid: bfef3717-d0e0-491d-8466-d8a9c995177d
ms.search.region: global
ms.search.industry: Retail
ms.author: rubendel
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0, Retail July 2017 update
ms.openlocfilehash: dd31a19be4b1874837832b7bb59453fec4b0819f
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54924"
---
# <a name="store-inventory-management"></a>商店库存管理

[!include [banner](includes/banner.md)]

本文描述可用于管理库存的文档类型。

您可以使用以下文档的类型管理您的组织的库存。

## <a name="purchase-orders"></a>采购订单
采购订单在总部创建。 如果零售仓库包括在采购订单头中，通过使用 Microsoft Dynamics 365 for Retail 中的 Modern POS (MPOS) 或 Cloud POS 订货可以在商店接收。 在商店输入已接收数量后，可以保存本地以供附加修改。 或者，数量可承诺和发送给总部。 在总部，在商店接收的数量将显示在 Dynamics 365 for Retail 中的采购订单的**当前接收量**字段中。

## <a name="transfer-orders"></a>转移单
转移单可指定特定商店为可用于装运物料的位置。 在这种情况下，转移单在商店中显示为 MPOS 或 Cloud POS 内的拣货请求。 在请求的领料数量后，它们承诺和发送总部。 在总部，在商店领取的数量将显示在 Dynamics 365 for Retail 中的转移单的**当前装运量**字段中。 转移单可以指定该物料可以装运到的位置的特定商店。 在这种情况下，转移单在商店中显示为 MPOS 或 Cloud POS 中的接收请求。 在商店输入已接收数量后，可以保存本地以供附加修改。 或者，数量可承诺和发送给总部。 在总部，在商店接收的数量将显示在 Dynamics 365 for Retail 中的转移单的**当前接收量**字段中。

## <a name="stock-counts"></a>存货盘点
存货盘点可以是计划或不定期的。 存货盘点在总部启动，总部指定必须盘点的物料。 总部会创建盘点文档，并将商店接收，将实际的现有存货数量输入 MPOS 或 Cloud POS.。 计划外存货盘点在商店启动，在 MPOS 或 Cloud POS. 中更新实际的现有存货数量。 与周期盘点不同，计划外存货盘点没有物料的预定义列表。 在存货盘点类型为已完工入库时，它承诺和发送给总部。 在总部，将验证和过帐盘点。

## <a name="inventory-lookup"></a>库存查找
在库存查找页可以查看多个商店和仓库的当前现有产品数量。 除了当前现有数量以外，还可以查看各个商店的未来可承诺 (ATP) 数量。 为此，选择你要查看 ATP 的商店，然后单击**查看商店可用性**。




