---
title: 处理数据库备份的方式
description: 本主题将帮助要了解 SQL 备份的客户。
author: Darinkramer
manager: AnnBe
ms.date: 11/02/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-talent
ms.technology: ''
audience: Application User
ms.reviewer: josaw
ms.search.scope: Talent
ms.custom: ''
ms.assetid: ''
ms.search.region: Global
ms.author: dkrame
ms.search.validFrom: 2018-11-02
ms.dyn365.ops.version: Talent
ms.openlocfilehash: c74b2caa63c3044f9c260246acc8639da0d3d211
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "60295"
---
# <a name="how-database-backups-are-handled"></a>处理数据库备份的方式

[!include [banner](includes/banner.md)]

**环境详细信息**

通过 Microsoft Dynamics Lifecycle Services (LCS) 设置的生产环境

**发货**

- 客户想要了解 Microsoft Dynamics 365 for Talent 的 SQL 备份计划。
- 客户想要还原生产环境的 SQL 备份。
- 客户希望将数据库从生产环境移至测试环境。

**解决方案**

- Talent 使用标准 Microsoft Azure SQL 数据库库存单位 (SKU)。 有关备份的详细信息，请参阅[了解自动 SQL 数据库备份](https://docs.microsoft.com/en-us/azure/sql-database/sql-database-automated-backups)。
- 就地生产环境备份的还原是应被视为昂贵的 Development Operations (DevOps) 操作。 实际上，对备份的还原程度是有限制的。 由于代码包几乎每周升级，我们不希望还原与代码包的当前版本兼容的备份。 因此，我们必须根据实际情况具体考虑最佳方法。
- 目前，将数据库从生产环境移至测试环境是一项 DevOps 操作。 Microsoft 当前不提供在 LCS 体验中移动或复制数据库的途径。 此功能已经请求，但尚未完成。 我们建议您使用数据实体包在环境之间导出/导入。

**长期解决方案**

作为我们长期未来计划的一部分，我们计划添加将生产数据库复制到测试环境的选项。
