---
title: 使用 ISO20022 付款格式创建和导出供应商付款
description: 此过程显示如何在供应商付款日记帐中创建付款行，并使用 ISO2022 贷方转帐示例生成供应商付款文件。
author: mrolecki
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerJournalTable, LedgerJournalTransVendPaym, SysQueryForm, VendPaymProposalEdit, BankAccountTableLookUp
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mrolecki
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 7f616c0de5b7f5cf0651766639b45d443606b8f6
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56213"
---
# <a name="create-and-export-vendor-payments-using-iso20022-payment-format"></a>使用 ISO20022 付款格式创建和导出供应商付款

[!include [task guide banner](../../includes/task-guide-banner.md)]

此过程显示如何在供应商付款日记帐中创建付款行，并使用 ISO2022 贷方转帐示例生成供应商付款文件。 

用于创建此过程的演示数据公司是 DEMF。

这是五个用于演示使用电子申报配置的供应商付款流程的流程中的第五个。 此过程针对 Dynamics 365 for Operations 版本 1611 中增加的一项功能。


## <a name="create-payment-lines"></a>创建付款行
1. 转至“应付账款”>“付款”>“付款日记帐”。
2. 单击“新建”。
3. 在列表中，标记所选的行。
4. 在“名称”字段中，输入或选择一个值。
5. 单击“行”。
6. 单击“付款方案”。
7. 单击”创建付款方案“。
8. 扩展“要包括的记录”部分。
9. 单击“筛选器”。
10. 在列表中，选择“供应商”表和“供应商帐户”字段的行。
11. 在“标准”字段中，输入或选择一个值。
    * 您可以为选择要付款的供应商交易应用任何条件，此示例中则是将 DE-001 用作供应商帐户。  
12. 单击“确定”。
13. 单击“确定”。
14. 单击”创建付款“。

## <a name="generate-an-iso20022-payment-file"></a>生成 ISO20022 付款文件

