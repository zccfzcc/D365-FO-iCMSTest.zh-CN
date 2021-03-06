---
title: 导出信用证
description: 这个流程帮助了解导出信用证的整个过程。
author: kweekley
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: CustTable, CustBankAccounts, DefaultDashboard, SalesTableListPage, SalesCreateOrder, SalesTable, BankLCExport, SalesEditLines,  LedgerJournalTable, LedgerJournalTransCustPaym, CustOpenTrans
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: kweekley
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: e730413a52c73e5e0e0312916564ec124e651d5e
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54442"
---
# <a name="export-letter-of-credit"></a>导出信用证

[!include [task guide banner](../../includes/task-guide-banner.md)]

这个流程帮助了解导出信用证的整个过程。

信用证是银行签发的协议，在信用证中银行同意代表买家确认付款（如果满足了买家和卖家间的协议条款）。



在运行该过程之前，先运行“设置银行融资和过帐模板”和”信用证创建银行融资协议”过程。 请选择 USMF 演示公司以成功运行该过程。




## <a name="create-sales-order-for-export-letter-of-credit"></a>创建“导出信用证销售订单”
1. 转到应收帐项目>订单>所有销售订单。
2. 单击“新建”。
3. 在“客户帐户”字段中，单击下拉按钮以打开查找。
4. 在列表中，找到并选择所需记录。
5. 在列表中，单击所选行中的链接。
6. 展开或收起“常规”部分。
7. 在“位置”字段中，单击下拉按钮打开查询。
    * 选择进货物料的装运“站点”。  
8. 在列表中，单击所选行中的链接。
9. 在“仓库”字段，单击下拉按钮以打开查找。
    * 选择进货物料的装运“仓库”。  
10. 在列表中，单击所选行中的链接。
    * 说明：此“银行单据编号”字段应选择相关值“信用证”。  
11. 在“银行单据类型”字段中，选择“信用证”。
12. 展开或折叠“交货”部分。
    * 选择“交货日期管理 = 无”。  
13. 在“请求收货日期”字段中，输入一个日期。
14. 单击“确定”。
15. 在“物料编号”字段中，单击下拉按钮以打开查找。
    * 选择所需的“装运/售出”物料。  
16. 在列表中，找到并选择所需记录。
17. 在列表中，单击所选行中的链接。
18. 在“单价”字段中，输入一个数字。
19. 展开或折叠“行详细信息”部分。
20. 单击“交货”选项卡。
21. 在“请求装运日期”字段中，输入一个日期。
22. 在“确认装运日期”字段中，输入一个日期。
23. 在“操作窗格”上单击“管理”。
24. 单击“信用证”。
25. 在“银行单据编号”字段中，键入一个值。
26. 在“到期日期”字段中，输入日期和时间。
27. 展开或折叠“银行详细信息”部分。
28. 在“开证银行”字段中，单击下拉按钮打开查找。
29. 在列表中，单击所选行中的链接。
30. 在“通知银行”字段中，单击下拉按钮打开查找。
31. 在列表中，找到并选择所需记录。
32. 在列表中，单击所选行中的链接。
33. 单击“提取订单装运”。
34. 单击“开证银行单据”。
35. 关闭该页面。

## <a name="post-packing-slip"></a>过帐“装箱单”
1. 在操作窗格中，单击“领料和装箱”。
2. 单击“将装箱单过帐”。
3. 展开或收起“参数”部分。
4. 在“数量”字段中，选择“所有”。
5. 展开或折叠“设置”部分。
6. 在“装箱单日期”字段中，输入一个日期。
7. 选择“装运数”。
8. 在列表中，单击所选行中的链接。
9. 单击“确定”。
10. 单击“确定”。

## <a name="post-sales-invoice"></a>过帐销售发票
1. 在操作窗格上，单击“发票”。
2. 单击“发票”。
3. 展开或折叠“概述”部分。
4. 选择“装运数”。
5. 在列表中，单击所选行中的链接。
6. 展开或折叠“设置”部分。
7. 在“发票日期”字段中，输入日期。
8. 单击“确定”。
9. 单击“确定”。

## <a name="shipment-document-submitted-status"></a>装运单据的提交状态
1. 在“操作窗格”上单击“管理”。
2. 单击“信用证”。
3. 展开或折叠“行”部分。
    * 说明：“文件提交”字段应设置为“是”。  

## <a name="verify-export-letter-of-credit"></a>核实“导出信用证”
1. 转到现金和银行管理>信用证>导出信用证和导入催款
2. 在列表中，找到并选择所需记录。
3. 在列表中，单击所选行中的链接。
    * 核实“导出信用证”的装运状态为“已开发票”。  

## <a name="customer-payment"></a>客户 - 付款
1. 转到“应收账款”>“付款”>“付款日记帐”。
2. 单击“新建”。
3. 在列表中，标记所选的行。
4. 在“名称”字段中，单击下拉按钮以打开查找。
5. 在列表中，单击所选行中的链接。
6. 单击“行”。
7. 在“日期”字段中，输入一个日期。
8. 在“帐户”字段中，指定所需值。
9. 单击“结算”。
10. 选择“总计”标题上的复选框。
    * 说明：设置“显示”字段为“信用证”。  
11. 在列表中，找到并选择所需记录。
12. 选中或取消选择“标记”复选框。
13. 单击“确定”。
14. 单击“付款”选项卡。
    * 核实“银行单据编号”和“装运数量”的详细信息  
15. 单击“过帐”。

## <a name="verify-export-letter-of-credit-after-payment"></a>在付款后核实“导出信用证”
1. 转到现金和银行管理>信用证>导出信用证和导入催款
2. 在列表中，找到并选择所需记录。
3. 在列表中，单击所选行中的链接。
    * 核实装运状态 = 已收到付款和余额 = 0.00。  

