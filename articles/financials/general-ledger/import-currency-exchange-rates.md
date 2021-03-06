---
title: 导入币种汇率。
description: 如果法人收到外币发票，则必须将外币转换为本币。 这意味着需要不同币种的最新汇率。 本主题提供导入欧洲央行和俄罗斯央行等汇率提供方通过 Internet 发布的参考汇率所需设置和处理的概览。
author: EvgenyPopovMBS
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ExchangeRateProviderConfiguration
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 261374
ms.assetid: b2b22868-de68-439f-914c-78c6930b7340
ms.search.region: Global
ms.author: epopov
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: f1134c9ccf6ef6faf248a1f59f2c4fd7f3aaad85
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56028"
---
# <a name="import-currency-exchange-rates"></a>导入币种汇率。

[!include [banner](../includes/banner.md)]

如果法人收到外币发票，则必须将外币转换为本币。 这意味着需要不同币种的最新汇率。 本主题提供导入欧洲央行和俄罗斯央行等汇率提供方通过 Internet 发布的参考汇率所需设置和处理的概览。

以下章节介绍用于设置和处理汇率导入的信息流。

## <a name="configure-an-exchange-rate-provider"></a>配置汇率提供方
必须先设置提供汇率的提供方所需信息，才能导入汇率。 请使用**配置汇率提供方**页选择汇率提供方。 Microsoft Dynamics 365 for Finance and Operations 中的演示数据随附了一些汇率提供方。 下表描述此页中的各个控件。

|           |                                                                                                                                                                                                                             |
|-----------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **字段** | **描述**                                                                                                                                                                                                             |
| **名称**  | 汇率提供方的名称。                                                                                                                                                                                     |
| **键**   | 提供方所需的每条配置信息的唯一标识符。 此信息为单击**添加**按钮时添加的每个汇率提供方自动添加。 |
| **值** | 每个参数的信息。 此信息为单击**添加**按钮时添加的每个汇率提供方添加。                                                                                         |

## <a name="import-currency-exchange-rates"></a>导入币种汇率。
可以从汇率提供方源导入汇率，然后在**汇率**页面中设置导入的汇率。 可使用**导入汇率**页导入汇率。 下表介绍成功完成导入过程所需字段。

|                                        |                                                                                                                                                                                                                                                                                                                                                                             |
|----------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **字段**                              | **描述**                                                                                                                                                                                                                                                                                                                                                             |
| **汇率类型**                 | 汇率类型。                                                                                                                                                                                                                                                                                                                                                      |
| **汇率提供方**             | 汇率提供方。                                                                                                                                                                                                                                                                                                                                                  |
| **导入起始日期**                       | 此参数管理导入当天汇率还是某个日期范围的汇率。 如果要使用日期范围，请输入或选择开始日期和结束日期。                                                                                                                                                                                                                |
| **创建必需的币种对**    | 如果导入的币种对不存在，此复选框管理币种对的自动创建。 此选项可能对某些提供方不可用。                                                                                                                                                                                               |
| **重写现有汇率**   | 已存在特定日期的汇率时，此复选框管理汇率对的现有汇率更新。 如果不选中此复选框，则已存在另一个汇率时，不导入指定日期的汇率。                                                                                       |
| **禁止在法定假日导入** | 此复选框管理假日的汇率导入。 例如，如果选中此复选框并使用欧洲央行作为汇率提供方，系统将不更新与当前法人有关的假日的汇率。 此选项可能对某些提供方不可用。 |





