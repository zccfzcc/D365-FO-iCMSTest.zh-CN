---
title: 审核特定产品的供应商
description: 此过程显示如何审核特定产品的供应商。
author: mkirknel
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: EcoResProductDetailsExtended, PdsApprovedVendorList, VendTable
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mkirknel
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: aa240f29668452d3006be4e939a51504f539fcf7
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55598"
---
# <a name="approve-vendors-for-specific-products"></a>审核特定产品的供应商

[!include [task guide banner](../../includes/task-guide-banner.md)]

此过程显示如何审核特定产品的供应商。 这允许您控制使在产品添加到采购订单时可以使用哪个供应商。 您可以使用演示数据公司 USMF 或您自己的数据使用该程序。 此任务通常由采购经理完成。

1. 转到“产品信息管理”>“产品”>“已发布产品”。
2. 在列表中，找到并选择所需记录。
3. 在列表中，单击所选行中的链接。
4. 展开“采购”部分。
    * 如果在“供应商”字段中显示主供应商，则您需要在以下步骤中添加此供应商为核准供应商。 如果显示了供应商编号，请记下该编号。  
5. 在操作窗格上，单击“采购”。
6. 单击“设置”。
7. 单击“添加”。
8. 在“供应商”字段中，输入或选择一个值。
    * 选择核准供应商。 如果在产品记录中有一个供应商，至少有一个行必须是主供应商。 如果您之前记录了供应商编号，请在此处选择它。  
9. 在“截止日期”字段，输入日期。
    * 选择数月前的日期。  
10. 单击“添加”。
11. 在“供应商”字段中，输入或选择一个值。
12. 在“截止日期”字段，输入日期。
    * 选择与以前的到期日期不同的日期。  
13. 关闭该页面。
14. 单击“核准供应商”。
15. 在“截止日期”字段，输入日期。
    * 此日期用作筛选器，这样您可以看到直到某一日期谁是核准供应商。  
16. 关闭该页面。
17. 单击“有效期”。
18. 在“显示供应商到期日期”字段中输入日期。
    * 您可以使用此页来标识审核状态将在某一日期之后到期的供应商。  
19. 关闭该页面。
20. 单击“编辑”。
21. 然后在“核准供应商检查方法”字段中选择选项。
    * 如果产品添加到供应商不是核准供应商的采购订单行，此字段可为应发生的情况选择策略。  
22. 单击“保存”。
23. 关闭该页面。
24. 关闭该页面。
25. 转到“采购”>“供应商”>“供应商/物料关系”>“按物料显示的核准供应商列表”。
    * 此页为您提供所有产品和核准供应商的概览。  
26. 关闭该页面。
27. 转到“采购”>“供应商”>“所有供应商”。
    * 您还可以从供应商开始，然后转到该供应商帐户的已审核产品的列表。  
28. 在列表中，找到并选择所需记录。
29. 在“操作”窗格上，单击“采购”。
30. 单击“按供应商显示的核准供应商列表”。
31. 关闭该页面。
32. 关闭该页面。

