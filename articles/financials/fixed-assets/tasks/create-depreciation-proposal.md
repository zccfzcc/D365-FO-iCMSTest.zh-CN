---
title: 创建折旧方案
description: 本程序描述了批处理折旧方案的工作原理，并说明了如何为固定资产建议折旧方案。
author: abruer
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerJournalTable, LedgerJournalTransAsset
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: abruer
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 4bc923c4b0c0903e221ee9483eb179fcfbb460ed
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56044"
---
# <a name="create-depreciation-proposal"></a>创建折旧方案

[!include [task guide banner](../../includes/task-guide-banner.md)]

本程序描述了批处理折旧方案的工作原理，并说明了如何为固定资产建议折旧方案。 此任务使用 USMF 演示公司和会计角色。


## <a name="create-depreciation-proposal"></a>创建折旧方案
1. 转到“固定资产”>“日记帐条目”>“创建折旧方案”。
2. 在“日记帐名称”字段中，单击下拉按钮以打开查找。
3. 在列表中，单击所选行中的链接。
4. 在“结束日期”字段中输入日期。
    * 选择“汇总折旧”选项，将按月折旧汇总到一个日记帐行。  
    * 例如，如果“结束日期”值为 2015 年 3 月 31 日，则会生成以下描述：“自 2015 年 1 月 31 日起折旧”。 建议日记帐行的“日期”字段随后将设置为 2015 年 3 月 31 日。  
    * 使用“筛选”选项，按资产、资产组或其他条件筛选折旧方案。  
    * 如果您为固定资产表格使用“创建购置或折旧方案”，可以批处理折旧方案。 对于使用较多系统资源的较大方案，建议使用此方案。 如果选择批处理选项，您仍可以在该期间完成其他任务。 在您这样建议折旧时，则为固定资产价值模型计算折旧。  
5. 单击“创建日记帐”。

## <a name="review-depreciation-entries"></a>查看折旧条目
1. 转到固定资产>流水输入项>固定资产流水。
2. 在列表中，找到并选择所需记录。
3. 单击“行”。
4. 单击“过帐”。

