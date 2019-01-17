---
title: 中国的固定资产折旧法
description: 此主题描述为中国法人设置的折旧法。
author: ShylaThompson
manager: AnnBe
ms.date: 03/21/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: AssetParameters
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 265244
ms.search.region: China (PRC)
ms.author: shylaw
ms.search.validFrom: 2016-11-30
ms.dyn365.ops.version: Version 1611
ms.openlocfilehash: fa72ee85d00f6e7efca8200fef3ec3996a95331c
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54954"
---
# <a name="fixed-assets-depreciation-methods-for-china"></a>中国的固定资产折旧法

[!include [banner](../includes/banner.md)]

此主题描述为中国法人设置的折旧法。

The sum of the years' digits method of depreciation (SYD) is one of the accelerated depreciation techniques that is based on the assumption that assets are generally more productive when they are new and their productivity decreases as they become old. SYD 法的折旧计算公式为：

> *SYD Depreciation = Depreciable base × (Remaining useful life/Sum of the  years digits)*

To create a depreciation profile:

1. On the **Fixed assets parameters** page, select the **SYDM and DRBM** depreciation methods.
2. 创建一个新折旧模板。 使用**年数总和法**或**双倍余额递减法**。
3. Create a book for the depreciation method, use either **Sum year digits** or **Double reducing balance**.

有关详细信息，请参阅[设置固定资产折旧分摊](./tasks/fixed-asset-depreciation-allocation.md)。


