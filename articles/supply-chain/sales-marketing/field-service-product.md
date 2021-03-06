---
title: 将 Finance and Operations 中的产品同步到 Field Service 中的产品
description: 本主题讨论用于将来自 Microsoft Dynamics 365 for Finance and Operations 的产品同步到 Microsoft Dynamics 365 for Field Service 的模板和基础任务。
author: ChristianRytt
manager: AnnBe
ms.date: 04/09/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: ''
audience: Application User, IT Pro
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: ''
ms.assetid: ''
ms.search.region: global
ms.search.industry: ''
ms.author: crytt
ms.dyn365.ops.version: July 2017 update
ms.search.validFrom: 2017-07-8
ms.openlocfilehash: c1cc7d8e081f140cd1b3662163afaf988cc5eedf
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "53339"
---
# <a name="synchronize-products-in-finance-and-operations-to-products-in-field-service"></a>将 Finance and Operations 中的产品同步到 Field Service 中的产品

[!include[banner](../includes/banner.md)]

本主题讨论用于将来自 Microsoft Dynamics 365 for Finance and Operations 的产品同步到 Microsoft Dynamics 365 for Field Service 的模板和基础任务。

使用的 **Field Service 产品（Fin and Ops 到 Field Service）** 模板基于“从目标客户到现金”中的**产品（Fin and Ops 到Sales）– 直接**模板。 有关详细信息，请参阅[产品（Fin and Ops 到Sales）– 直接](https://docs.microsoft.com/en-us/dynamics365/unified-operations/supply-chain/sales-marketing/products-template-mapping-direct)。

本主题仅介绍 **Field Service 产品（Fin and Ops 到 Field Service）** 与**产品（Fin and Ops 到Sales）– 直接**模板之间的差异。

## <a name="templates-and-tasks"></a>模板和任务

**数据集成中的模板名称：**

- Field Service 产品（Fin and Ops 到 Field Service）

**数据集成项目中的任务名称：**

- 产品 - 产品

**Field Service 产品（Fin and Ops 到 Field Service）** 模板中包含**产品（Fin and Ops 到Sales）– 直接**模板中没有的一个映射。 此映射确保正确设置所需的 Field Service 特定的 **Field Service 产品类型**。

```
FIELDSERVICEPRODUCTTYPE        Fn        msdyn_fieldserciveproducttype
```

使用以下值映射。

```
inventory     :  690970000
nonInventory  :  690970001 
service       :  690970002 
```

在 Finance and Operations 中，**适售的已发布产品**数据实体的 **Field Service 产品类型**值的计算方法如下：

- **库存：** 产品类型 = 产品和物料模型组，贮存的产品 = True
- **非库存：** 产品类型 = 产品和物料模型组，贮存的产品 = False
- **服务：** 产品类型 = 服务

## <a name="template-mapping-in-data-integration"></a>数据集成中的模板映射

下图显示了数据集成中的模板映射。

### <a name="field-service-products-fin-and-ops-to-field-service-products---products"></a>Field Service 产品（Fin and Ops 到 Field Service）：产品 - 产品

[![数据集成中的模板映射](./media/FSProduct.png)](./media/FSProduct.png)
