---
title: CN-00016 按中国工作规则的用户操作日志
description: 此过程演示如何创建用户操作日志。
author: ShylaThompson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysDatabaseLogSetup, SysDatabaseLogWizard, BankAccountTable, ComplianceUserOperationLogConfig_CN
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: China (PRC)
ms.author: shylaw
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: b6c442a2bdb67a6d4252b1eb3070df5a8c53a359
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "55990"
---
# <a name="cn-00016-user-operation-log-by-china-working-rule"></a>CN-00016 按中国工作规则的用户操作日志

[!include [task guide banner](../../includes/task-guide-banner.md)]

此过程演示如何创建用户操作日志。 必须先设置数据库日志，才能生成用户操作日志。  

根据您指定的条件跟踪用户操作并记录在日志中，包括操作类型、用户名，以及时间和日期。 此过程逐步演示如何为跟踪银行帐户的创建设置条件，为演示目的创建银行帐户，然后生成用户日志。

此程序使用 CNMF 演示数据。 此过程针对 Dynamics 365 for Operations 版本 1611 中增加的一项功能。


## <a name="set-up-the-database-log"></a>设置数据库日志
1. 转到“系统管理”>“设置”>“数据库日志配置”。
2. 单击“新建”。
3. 单击“下一步”。
4. 在树中，展开“银行”。
5. 在树中，检查“银行\银行帐户”。
    * 对于此演示，我们希望跟踪谁创建银行帐户，但是您可能希望跟踪其他用户操作。  
6. 单击“下一步”。
7. 选中“跟踪新交易记录”复选框。
8. 选中“更新”复选框。
9. 选中“删除”复选框。
10. 单击“下一步”。
11. 单击“完成”。

## <a name="create-a-new-bank-account-for-demonstration-purposes"></a>出于演示目的新建银行帐户
1. 转至“现金和银行管理”>“银行对账单对帐”>“银行帐户”。
2. 单击“新建”。
3. 在“银行帐户”字段中，键入一个值。
4. 在“银行帐号”字段中，输入一个值。
5. 在“主科目”字段中，指定所需值。
6. 单击“保存”。

## <a name="print-the-user-operation-log-report"></a>打印用户操作日志报告
1. 转到“系统管理”>“查询”>“用户操作日志查询”。
2. 在树中，展开“银行”。
3. 在树中，检查“银行\银行帐户”。
4. 展开“按用户”部分。
5. 在“用户”字段中，输入或选择一个值。
    * 对于此示例，如果您在上一个子任务中创建了银行帐户，请选择您的用户名。 否则选择最近创建了银行帐户的其他用户。  
6. 展开“按日期”部分。
7. 在“开始日期”字段中输入日期。
8. 在“结束日期”字段中输入日期。
9. 单击“确定”。
10. 单击“确定”。

