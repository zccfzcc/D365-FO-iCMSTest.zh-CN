---
title: 无法在 PowerApps 管理中心创建环境
description: 本主题说明如果管理员无法在 Microsoft PowerApps 管理中心创建环境该做什么。
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
ms.openlocfilehash: 5bee2be99b4f70db9ba75cd1e040c445c47ef9f8
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "60168"
---
# <a name="cant-create-an-environment-in-the-powerapps-admin-center"></a>无法在 PowerApps 管理中心创建环境

[!include [banner](includes/banner.md)]

**发货**

- 租户/环境管理员无法在 Microsoft PowerApps 管理中心创建环境。
- 授予用户执行环境创建步骤权限的许可证未直接分配给执行该步骤的用户。

**解决方案**

确保租户管理员已将有效的 PowerApps P2 许可证直接分配给将执行环境创建步骤的用户。 这里是提供该权限的 Microsoft Dynamics 服务计划。

| 整个产品库存单位 (SKU)       | PowerApps P2 服务计划  |
|------------------------------------------------|----------------------------|
| Microsoft Dynamics 365 for Operations          | PowerApps for Dynamics 365 |
| Microsoft Dynamics 365 计划 Enterprise Edition | PowerApps for Dynamics 365 |

请注意，各个 Microsoft Office SKU 也提供权限，以及独立的 PowerApps 计划 2 SKU。 重点是这些 SKU 中的一个必须存在。

1. 转到 [https://preview.admin.powerapps.com/environments](https://preview.admin.powerapps.com/environments)。
2. 按照[配置 Talent](https://docs.microsoft.com/en-us/dynamics365/unified-operations/talent/provisioning-talent) 中的说明创建环境。
