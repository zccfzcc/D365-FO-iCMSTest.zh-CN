---
title: 创建在线渠道和定义渠道属性
description: 此程序会逐步演示如何创建新的在线渠道，然后将其添加到组织层次结构。
author: jashanno
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: RetailSPOnlineStoreDetailPage, SysLookupMultiSelectGrid, DimensionLookup, OMHierarchyManager, HierarchyDesigner, OMNodeSelection, HierarchyPublishAndCloseForm
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.search.industry: Retail
ms.author: jashanno
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 967048ef90072c3ee9aafe1fc657a6aa32550a3e
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56077"
---
# <a name="create-online-channel-and-define-channel-attributes"></a>创建在线渠道和定义渠道属性

[!include[task guide banner](../includes/task-guide-banner.md)]

此程序会逐步演示如何创建新的在线渠道，然后将其添加到组织层次结构。 在创建新的在线渠道之前，您必须创建组织层次结构。 此程序使用 USRT 演示数据公司。


## <a name="create-a-new-online-channel"></a>创建新的在线渠道
1. 转至“零售和商业”>“渠道”>“在线商店”。
2. 单击“新建”。
3. 在“名称”字段中，键入一个值。
4. 在“仓库”字段中，输入或选择一个值。
5. 在“商店时区”字段中，选择一个选项。
6. 在“默认客户”字段中，输入或选择一个值。
7. 在“客户通讯簿”字段中，输入或选择一个值。
8. 在“付款条款”字段中，输入或选择一个值。
9. 在“付款方式”字段中，输入或选择一个值。
10. 在“电子邮件通知配置文件”字段中，输入或选择一个值。
11. 扩展财务维度区段。
12. 在“业务单位”字段中，输入或选择一个值。
    * 同样设置所有其他默认维度的值。  
13. 单击“保存”。

## <a name="add-the-online-channel-to-organization-hierarchy"></a>将在线渠道添加到组织层次结构
1. 关闭该页面。
2. 转到“组织管理”>“组织”>“组织层次结构”。
3. 在列表中，找到并选择所需记录。
4. 单击“查看”。
5. 单击“编辑”。
    * 您可以选择您想要在其项下插入新渠道的任何层次结构节点。  
6. 单击“插入”。
7. 单击“零售渠道”。
8. 单击“确定”。
9. 单击“发布”以打开下拉对话框。
10. 在“有效日期”字段中输入日期和时间。
11. 单击“发布”。

