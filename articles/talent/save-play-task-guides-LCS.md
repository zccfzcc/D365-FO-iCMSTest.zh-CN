---
title: 将任务指南保存到 LCS 并重新播放它们
description: 本主题说明如何将任务指南保存到 Microsoft Dynamics Lifecycle Services (LCS) 然后重新播放它们。
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
ms.openlocfilehash: f54751629a6ead46c8e2d1c60ba0d9ebced325bb
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "60200"
---
# <a name="save-task-guides-to-lcs-and-replay-them"></a>将任务指南保存到 LCS 并重新播放它们

[!include [banner](includes/banner.md)]

**环境详细信息** 

Microsoft Dynamics 365 for Talent 通过 Microsoft Dynamics Lifecycle Services (LCS) 部署

**发货**

客户希望将新任务录制保存到其 LCS 项目，然后重新播放保存的任务指南。

**分辨率**

请执行以下步骤将任务录制保存到 LCS。

1. 登录到 LCS，并选择项目。
2. 选择**业务流程建模器**磁贴。
3. 在“更新的 BPM 体验”中查看此页面。
4. 选择库，然后选择**复制**。
5. 为业务流程建模器 (BPM) 模型输入一个名称。
6. 从 LCS 登录 Talent。
7. 在**搜索**字段中，输入**帮助**。 Lifecycle Services 帮助将打开。
8. 选择 Lifecycle Services 帮助配置的**刷新**按钮。

    您的新 BPM 库应会出现，它应是活动的。

9. 关闭该页面。
10. 创建任务录制。
11. 当您完成时，选择**保存到 Lifecycle Services**。

    ![保存到 Lifecycle Services](media/task-guides.png)

12. 选择要保存任务录制的 BPM 库和节点。

执行以下步骤从 LCS 重新播放任务指南。

1. 启动任务录制器
2. 选择**从 LCS 打开**。
3. 选择包含保存的任务指南的库和 BPM 节点。
4. 打开任务指南。
