---
title: 过帐期间日记帐
description: 定期日记帐有时称作循环日记帐，因为这些数额、文本和其他信息每次均会在检索定期日记帐时重复出现。
author: aprilolson
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerJournalTable, LedgerJournalTransPeriodic, LedgerJournalTransDaily
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: aolson
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 023689f8fb03091c213e96bdbd04c06cff63ce82
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56463"
---
# <a name="post-periodic-journals"></a>过帐期间日记帐

[!include [task guide banner](../../includes/task-guide-banner.md)]

定期日记帐有时称作循环日记帐，因为这些数额、文本和其他信息每次均会在检索定期日记帐时重复出现。 当您创建定期日记帐时，您需要指定循环的间隔周期，如天或月。 此任务指南将创建一个以月为周期的定期日记帐。



1. 转到总分类记账>周期性任务 >周期账簿。
2. 单击“新建”。
3. 在“名称”字段中，输入或选择一个值。
4. 在列表中，单击所选行中的链接。
5. 在“描述”字段中，键入一个值。
    * 日后检索时，该描述将为期间日记帐的名称，因此请确保指定一个相关名称。  
6. 单击“行”。
    * 期间日记帐一般包含多个日记帐行。 但是此任务向导只能添加一行。  
7. 在“日期”字段中，输入一个日期。
    * “日期”字段包含下次转移到日常记帐中的过帐日期。 对于每个月均将检索的日记帐，建议过帐时采用当月日期，一般是期间的开始或结束日期。 也可以将“日期”字段留空，并在检索日记帐时通过“空白日期”字段指定一个日期。    检索交易记录时，该字段会自动更新为下一轮日期。  
8. 在“帐户”字段中，指定所需值。
9. 在“描述”字段中，键入一个值。
10. 关闭该页面。
11. 在“借方”字段中，输入一个数值。
12. 在“抵销帐户”字段中，指定所需值。
13. 在“单位”字段中，选择“月”。
14. 在“单位标号”字段中，输入“1”。
15. 在“最后日期”字段中，输入一个日期。
    * 在上一个期间输入结束日期会避免在错误的开始期间错误地创建循环日记帐。 最后日期将会在每次检索期间日记帐之后得到更新。  
16. 单击“保存”。
17. 转到“默认仪表板”。
18. 转到“总帐”>“日记帐条目”>“普通日记帐”。
19. 单击“新建”。
20. 在“名称”字段中，输入或选择一个值。
21. 在列表中，找到并选择所需记录。
22. 在列表中，单击所选行中的链接。
23. 在“描述”字段中，键入一个值。
24. 单击“行”。
25. 单击“定期日记帐”。
26. 单击“检索日记帐”。
27. 在“结束日期”字段中输入日期。
    * “结束日期”是指周期凭证行的截止日期。 基于周期设置，同一行的“最后日期”和“结束日期”可能会多次出现在结果日记帐中。 结束日期将会根据定期行转移到日记帐的最后会话日期进行自动更新。  
28. 在“定期日记帐编号”字段中，输入或选择一个值。
29. 在列表中，单击所选行中的链接。
30. 单击“确定”。
    * 定期日记帐可以根据需求和设置进行检查、审核或过帐。  

