---
title: 创建和关联收银机
description: 此过程演示如何创建销售点 (POS) 收银机。
author: rubencdelgado
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: RetailTerminalTable
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Retail
ms.author: rubendel
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 2ac5135d0606ffc9816c841637aa032826f87e28
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "53753"
---
# <a name="create-and-associate-registers"></a>创建和关联收银机

[!include[task guide banner](../includes/task-guide-banner.md)]

此过程演示如何创建销售点 (POS) 收银机。 此过程使用了演示数据公司 USRT。

1. 转至“零售和商业”>“渠道设置”>“POS 设置”>“收银机”。
2. 单击“新建”。
3. 在“收银机编号”字段中，键入新收银机的编号。
    * 收银机 ID 中通常包含有助于将收银机映射到其所属商店的代码，以及商店内的位置。  
4. 在“名称”字段中，键入收银机的描述性名称。
5. 在“商店编号”字段中，输入或选择一个值。
6. 在“硬件配置文件”字段中，输入或选择一个值。
    * 硬件配置文件用于指定将连接到收银机的零售外设，如银箱和收据打印机。  
7. 在“可视化配置文件”字段中，输入或选择一个值。
    * 可视化配置文件用于指定 POS 背景和登录页中使用的图像，以及 POS 的主题。  
8. 在“EFT POS 收银机编号”字段中，输入一个值。
    * EFT POS 收银机编号用于通知付款处理器哪个终端在发送授权请求。 该值通常称为“终端 ID”或“TID”。 TID 通常位于付款设备上的贴纸中。  
9. 单击“保存”。

