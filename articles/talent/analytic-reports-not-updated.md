---
title: 分析报告未更新
description: 本主题说明如果客户的数据更改不出现在任何客户的工作区时该怎么做。
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
ms.openlocfilehash: 35dd7722ce550bfcd2270352843e6d7e981afc92
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "60274"
---
# <a name="analytic-reports-are-not-updated"></a>分析报告未更新

[!include [banner](includes/banner.md)]

**发货**

客户的数据更改不出现在任何客户的工作区的**分析**选项卡。

**原因**

默认情况下，Microsoft Power BI 报表根据部署度量批处理作业的计划每四小时刷新一次。

**分辨率**

此问题可能只是时间问题。 请执行以下步骤开始批处理作业并更新分析工作区。

1. 在**系统管理 \> 链接 \> 批处理作业 \> 批处理作业**打开**批处理作业**页。 或者，使用“搜索”，输入**批处理作业**。
1. 在列表中查找**部署度量**作业。
1. 选择该页顶部的**编辑**，将计划的开始日期/时间设置为将刷新更接近当前时间的分析的值。

![批处理作业](media/batch-jobs.png)
