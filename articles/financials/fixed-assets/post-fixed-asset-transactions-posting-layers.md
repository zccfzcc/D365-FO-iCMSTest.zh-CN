---
title: 将固定资产交易记录过帐到过帐层
description: 本文提供固定资产交易记录的过帐层功能的概览。
author: ShylaThompson
manager: AnnBe
ms.date: 04/25/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: AssetBookTable, LedgerJournalTransAsset
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 3001
ms.assetid: 7dabde57-0843-47c3-85ef-f36b6f472e30
ms.search.region: Global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 135cfd24d4605407fea846940f0d84e9eda9a081
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54339"
---
# <a name="post-fixed-asset-transactions-to-posting-layers"></a>将固定资产交易记录过帐到过帐层

[!include [banner](../includes/banner.md)]

本文提供固定资产交易记录的过帐层功能的概览。

通常，出于不同的目的会采用不同的方法对固定资产进行折旧。 出于纳税目的，将根据当前的纳税规则计算折旧，以实现尽可能高的税前折旧；但出于报告目的，将根据会计法和标准计算折旧。 各种折旧都分别在过帐层进行计算和记录。

附加到固定资产的每个帐簿都是针对具有整体折旧目标的特定过帐层设置的。 有十个过帐层：当前、工序、纳税和七个自定义层。 您还可以通过将“过帐到总帐”字段设置为“否”，为帐簿禁用过帐到总帐。 “过帐层”字段将自动设置为“无”。 不过帐到总帐的帐簿通常用于报税用途。 这样您的灵活性更高，可以删除资产帐簿的历史交易信息，因为这些信息尚未提交给总帐。

固定资产日记帐通过“日记帐名称”页面上的总帐 >日记帐设置 >日记帐名称进行定义。 可以将折旧过帐到其中的每个日志都只能由其日志名称为一个过帐层定义。 日记帐中的过帐层无法更改。 此限制有助于保障每个过帐层的交易记录都单独存放。 因此，必须为每个过帐层至少创建一个日志名称。 如果您在使用不过帐到总帐的帐簿，则还必须创建过帐层设置为“无”的日记帐。

您可以在“固定资产过帐模板”页指定固定资产交易记录的会计科目。 对于每个过帐模板，都必须选择相关的交易记录类型和帐簿，然后指定会计科目。 设置要过帐到总帐的每个帐簿的过帐模板记录。

> [!NOTE] 
> 使用衍生帐簿，可以将交易记录同时过帐到不同的过帐层。 可以在过帐层对应于帐簿过帐层的日记帐中创建主帐簿的交易记录。 在过帐期间，衍生帐簿交易记录将过帐到相应的过帐层。

有关详细信息，请参阅[衍生帐簿](derived-books.md)和[使用衍生帐簿过帐](post-derived-value-models.md)。



