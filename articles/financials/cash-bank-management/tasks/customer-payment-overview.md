---
title: 客户付款概览
description: 本任务指南逐步介绍用于输入客户付款的各种方法。
author: kweekley
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerJournalTable, CustPaymEntry, CustTableLookup, LedgerJournalTransCustPaym, CustOpenTrans, BankAccountTableLookUp
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: kweekley
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 59487f50974c3035c3a4d2d41ccbd740850e440d
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "53491"
---
# <a name="customer-payment-overview"></a>客户付款概览

[!include [task guide banner](../../includes/task-guide-banner.md)]

本任务指南逐步介绍用于输入客户付款的各种方法。 本任务使用 USMF 公司进行演示。

1. 转到“应收账款”>“付款”>“付款日记帐”。
2. 单击“新建”。
3. 选择将保存客户付款的付款日记帐。
4. 选择或手动输入日记帐。
5. 单击“输入客户付款”。
    * 输入客户付款用于一次记录一项客户付款。 您在顶部输入付款信息，然后标记该付款支付的发票，全部在同一个页面操作。  
6. 输入您接收其付款的客户。
    * 如果您不知道客户，但是知道已付款的交易，则可以使用“交易记录”字段输入付款。 在“交易记录”字段中输入或选择发票。 在选择交易后，客户将自动默认填充。  
7. 在“付款参考”字段中，输入付款参考。
    * 付款参考可以是客户的支票编号或客户的电子付款参考。 仅当您标记为在存款单上包括付款时才需要付款参考。  
8. 选择是否在存款单中加入付款。 
9. 输入客户付款金额。
    * 付款金额不会默认填充。 必须手动输入。  
10. 标记客户已支付的发票。
    * 如果付款为预付款，您无需为结算标记任何发票。 付款仍可以保存和过帐。 发票结算可在稍后进行。  
11. 输入应结算以标记发票的付款的金额。 
    * 此字段可在付款为部分付款时使用。 如果您不输入金额，系统将自动为您确定要结算的金额。  
12. 单击“保存在日记帐中”。
    * 在将付款保存到日记帐前，请确保已定义对方科目。 使用“保存在日记帐中”将保存付款并将其移动到日记帐中。 然后，您可以继续输入下一笔付款。  
13. 关闭该页面。
14. 单击“行”。
    * 在打开“行”时，您将看到您在“输入客户付款”页面记录并保存到日记帐的所有付款。 您还可以使用此页输入新的客户付款，或在现有客户付款过帐前对其进行编辑。  
15. 单击“新建”创建另一项付款。 
16. 选择您接收其付款的客户。
    * 如果您不知道客户，但知道付款支付的发票，则使用“发票”字段手动输入或选择发票。 选择发票后，客户将默认填充。  
17. 单击“结算交易记录”标记已支付的发票。
    * 您无需将付款结算到任何发票。 如果是预付款，或您不知道已支付的发票，您可以输入并过帐付款。 付款可以稍后结算到发票。  
18. 标记付款已支付的发票。 
19. 输入将结算以标记发票的付款金额。
20. 单击“确定”。
21. 在“付款参考”字段中，输入付款参考。 。
    * 仅当您标记为在存款单上包括付款时才需要付款参考。  
22. 过帐客户付款。 
