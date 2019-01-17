---
title: 定义 ER 配置与其他组件之间的依赖关系
description: 若要完成这些步骤，首先必须完成任务指南“ER 管理模型映射配置”中的步骤，还必须可以访问 Microsoft Dynamics Lifecycle Services (LCS)。
author: NickSelin
manager: AnnBe
ms.date: 06/23/2017
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
audience: Application User
ms.reviewer: kfend
ms.search.scope: Operations
ms.search.region: Global
ms.author: nselin
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 9284b705f362704da62e1583c140df95a9853cb9
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54113"
---
# <a name="define-the-dependency-of-er-configurations-on-other-components"></a>定义 ER 配置与其他组件之间的依赖关系

[!include [task guide banner](../../includes/task-guide-banner.md)]

若要完成这些步骤，首先必须完成任务指南“ER 管理模型映射配置”中的步骤，还必须可以访问 Microsoft Dynamics Lifecycle Services (LCS)。

此过程显示如何设计电子申报 (ER) 配置和指定其与其他软件组件之间的依赖关系，以便帮助确保将配置正确下载到特定 Microsoft Dynamics 365 for Finance and Operations 版本。 在此示例中，将为示例公司 Litware 公司创建所需 ER 配置。 

此过程针对向其分配了系统管理员角色或电子申报开发人员角色的用户。 这些步骤适用于所有公司，因为这些公司共享 ER 配置。 

1. 转到“组织管理”>“电子申报”>“配置”。
    * 确保配置树中包含“示例数据模型”配置和附属项。 否则，完成“ER 管理模型映射配置”这一任务指南中的步骤，然后再次启动此指南。   

## <a name="define-the-dependency-of-er-configurations-from-other-components"></a>定义 ER 配置与其他组件之间的依赖关系
1. 在树中，展开“示例数据模型”。
2. 在树中，选择“示例数据模型\示例映射“。
    * 我们选择了“示例映射”模型映射配置的草稿版本。 我们现在将定义其与其他软件组件之间的依赖关系。 此步骤被视为控制从 ER 存储库下载此配置的版本和进一步使用此版本的先决条件。   
3. 展开“先决条件”部分。
    * 请注意，此阶段已自动添加了“实施”先决条件组。 此组中包含引用数据模型配置的先决条件组件，并且已开启了实施标记。 此标记指示“示例映射”映射配置被视为“示例数据模型”数据模型的实施。 只要下载了“示例数据模型”模型配置，此组件都将强制 ER 从 ER 存储库下载“示例映射”映射配置。   
4. 单击“编辑”。
    * 可以通过使用软件组件的类型，以及组件版本或组件版本范围，定义配置的当前版本与该软件组件之间的单个依赖关系。  
    * 可以将所需依赖关系组合在一起。 如果选择了“所有”组类型，并且满足了此组和附属组的每个依赖关系条件，将视为满足了此组的依赖关系条件。 如果选择了“一个”组类型，并且满足了此组的至少一个依赖关系条件，将视为满足了此组的依赖关系条件。   
5. 单击“新建”。
6. 选择”产品必备项组件“。
7. 选择“Microsoft Dynamics 365 for Operations (1611)”。
8. 在”版本“字段中，键入”[7.1.1541.3036,8)“。
    * [7.1.1541.3036,8)  
    * 如果从任何 ER 存储库下载了此配置，将评估您输入的依赖关系。 如果“示例数据模型”配置的版本 1 已提前准备就绪或下载，将从 ER 存储库下载此配置版本。 如果提前下载，则必须在 Finance and Operations 中完成，其版本必须为 7.1.1541.3036 或更高，但是不得超过主要版本 8。   
9. 单击“保存”。
10. 关闭该页面。
11. 单击“更改状态”。
12. 单击“完成”。
13. 单击“确定”。
14. 在树中，选择“示例数据模型\示例映射(备用)“。
15. 单击“编辑”。
16. 单击“新建”。
17. 选择”产品必备项组件“。
18. 选择”Microsoft Dynamics AX 7.0 RTW“。
19. 在”版本“字段中，键入”[7.0.1265.3015,7.1)“。
    * [7.0.1265.3015,7.1)  
    * 如果从任何 ER 存储库下载了此配置，将评估依赖关系。 如果“示例数据模型”配置的版本 1 已提前准备就绪或下载，将从 ER 存储库下载此配置版本。 如果提前下载，则必须在 Microsoft Dynamics 365 for Finance and Operations Enterprise Edition 中完成，其版本必须为 7.0.1265.3015 或更高，但是不得超过次要版本 1。   
20. 单击“保存”。
21. 关闭该页面。
22. 单击“更改状态”。
23. 单击“完成”。
24. 单击“确定”。

## <a name="configure-the-er-repository"></a>配置 ER 存储库
1. 关闭该页面。
2. 转到“组织管理”>“工作区”>“电子申报”。
    * 打开当前 ER 提供商 Litware 公司的 ER 存储库列表。  
3. 在列表中，标记所选的行。
4. 单击“存储库”。
5. 单击“显示筛选器”。
6. 使用”包含“筛选器运算符在”类型名称“字段中输入筛选器值”LCS“。
    * 如果已经为当前 ER 提供商注册了 LCS 存储库，则可跳过此子任务中的其余步骤。 如果尚未注册 LCS 存储库，请完成其余步骤。   
7. 单击“添加”以打开下拉对话框。
8. 在“配置存储库类型”字段中，输入”LCS“。
9. 单击“创建存储库”。
10. 在“项目”字段中，输入或选择一个值。
    * 从“项目”字段的查找中选择所需 LCS 项目。  
11. 单击“确定”。
12. 关闭该页面。

## <a name="upload-configurations-to-lcs"></a>将配置上传到 LCS
1. 单击“申报配置”。
2. 在树中，选择“示例数据模型”。
3. 选择此配置的已完成版本。
4. 单击“更改状态”。
5. 单击“共享”。
6. 单击“确定”。
    * 已通过使用以前配置的 ER 存储库的 LCS 项目，将此模型配置的版本 1 上传到该 LCS。   
7. 在树中，展开“示例数据模型”。
8. 在树中，选择“示例数据模型\示例映射“。
9. 选择此配置的已完成版本。
10. 单击“更改状态”。
11. 单击“共享”。
12. 单击“确定”。
    * 已通过使用以前配置的 ER 存储库的 LCS 项目，将此模型映射配置的版本 1.1 上传到该 LCS。   
13. 在树中，选择“示例数据模型\示例映射(备用)“。
14. 选择此配置的已完成版本。
15. 单击“更改状态”。
16. 单击“共享”。
17. 单击“确定”。
    * 已通过使用以前配置的 ER 存储库的 LCS 项目，将此模型映射配置的版本 1.1 上传到该 LCS。   

## <a name="evaluate-er-configuration-dependencies"></a>评估 ER 配置依赖关系
    * 我们将从系统中删除创建的配置，然后将其从 LCS 存储库下载回来。  
1. 在树中，选择“示例数据模型\示例映射“。
2. 单击“删除”。
3. 单击“是”。
4. 在树中，选择“示例数据模型\示例映射(备用)“。
5. 单击“删除”。
6. 单击“是”。
7. 在树中，选择“示例数据模型\示例格式“。
8. 单击“删除”。
9. 单击“是”。
10. 在树中，选择“示例数据模型”。
11. 单击“删除”。
12. 单击“是”。
13. 关闭该页面。
    * 打开当前 ER 提供商 Litware 公司的 ER 存储库列表。  
14. 单击“存储库”。
15. 单击“显示筛选器”。
16. 使用”包含“筛选器运算符在”类型名称“字段中输入筛选器值”LCS“。
17. 单击“打开”。
18. 在树中，选择“示例数据模型”。
    * 请注意，您可以查看对是否已满足了当前存储库的 ER 配置各版本必备项的评估。 若要查看此评估，请单击“检查必备项”。   
19. 单击”检查必备项“。
20. 单击“导入”。
21. 单击“是”。
22. 关闭该页面。
23. 关闭该页面。
24. 关闭该页面。
25. 转到“组织管理”>“电子申报”>“配置”。
26. 在树中，展开“示例数据模型”。
    * 请注意，已下载了模型“示例映射”映射配置和所选数据模型配置。 一起下载这两个文件是因为已将“示例映射”定义为实施所选数据模型，并且其适用于 Finance and Operations。 尚未下载“示例映射（备用）”配置，因为未满足所需应用程序版本的条件。   
    * 如果登录 Dynamics 365 for Finance and Operations Enterprise edition，注册相同提供程序，访问相同 LCS 项目，然后下载相同数据模型配置，将下载“示例映射（备用）”配置，但跳过“示例映射”配置。  
