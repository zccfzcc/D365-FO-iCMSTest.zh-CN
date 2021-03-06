---
title: 在现金折扣期间之外执行现金折扣
description: 本文提供显示即使在现金折扣期间外进行付款时也可以执行的现金折扣的两种情况。
author: ShivamPandey-msft
manager: AnnBe
ms.date: 08/22/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerJournalTransVendPaym, VendOpenTrans
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 14301
ms.assetid: bad10b7f-e550-4742-9261-8a094c9c624d
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: cf5700c9adb3dad0bc64fc706f761fbb2ee71403
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54827"
---
# <a name="take-a-cash-discount-outside-the-cash-discount-period"></a>在现金折扣期间之外执行现金折扣

[!include [banner](../includes/banner.md)]

本文提供显示即使在现金折扣期间外进行付款时也可以执行的现金折扣的两种情况。

6 月 28 日，April 为供应商 3052 创建 2,000.00 的发票。 如果在 14 天内支付该发票，则发票的现金折扣为 1%。

## <a name="use-cash-discount-option--always"></a>使用现金折扣选项 = 始终
April 在 7 月 1 日（折扣日期之后）创建付款。 April 打开**结算交易记录**页查看可以结算的交易记录。 

April 标记付款的发票。 不会执行现金折扣，因为付款在折扣日期之后。 但是，供应商已赋予 April 始终执行现金折扣的审核权。 因此，April 更改**使用现金折扣**字段中的值为**始终**。

| 标记     | 使用现金折扣 | 凭证   | 帐户 | 现金折扣日期 | 到期日期  | 开票 | 交易记录币种金额 | 货币 | 要结算的金额 |
|----------|-------------------|-----------|---------|--------------------|-----------|---------|--------------------------------|----------|------------------|
| 已选择 | 始终            | Inv-10030 | 3052    | 6/28/2015          | 7/12/2015 | 10030   | -2,000.00                      | 美元      | -1,980.00        |

折扣信息显示在**结算交易记录**页的底部。

|                              |           |
|------------------------------|-----------|
| 现金折扣日期           | 7/12/2015 |
| 现金折扣金额         | -20.00    |
| 使用现金折扣            | 始终    |
| 提取了现金折扣          | 0.00      |
| 要提取的现金折扣金额 | -20.00    |

## <a name="date-to-use-for-calculating-discounts--selected-date"></a>用于计算折扣的日期 = 所选日期
如果发票和付款均已过帐，仍可以在**结算交易记录**页面结算交易记录时执行现金折扣。 April 将**用于计算折扣的日期**字段中的值更改为**所选日期**。 然后她输入日期 6 月 28 日，该日期在发票的现金折扣期间内。 该日期用于计算交易记录的现金折扣。 在**结算未结交易记录**页上，April 看到，默认情况下，显示完整折扣 20.00。 发票行显示要结算的金额为 1,980.00。

| 标记                     | 使用现金折扣 | 凭证   | 帐户 | 现金折扣日期 | 到期日期  | 开票 | 交易记录币种金额 | 货币 | 要结算的金额 |
|--------------------------|-------------------|-----------|---------|--------------------|-----------|---------|--------------------------------|----------|------------------|
| 已选择和突出显示 | 标准            | Inv-10030 | 3052    | 6/28/2015          | 7/12/2015 | 10030   | -2,000.00                      | 美元      | -1,980.00        |
| 选定                 | 标准            | APP-10030 | 3052    | 7/15/2015          | 7/15/2015 |         | 500.00                         | 美元      | 500.00           |

折扣信息显示在**结算未结交易记录**页的底部。 执行的折扣金额是 20.00，因此，要结算的发票金额为默认金额 1,980.00。

|                              |           |
|------------------------------|-----------|
| 现金折扣日期           | 7/12/2015 |
| 现金折扣金额         | -20.00    |
| 使用现金折扣            | 标准    |
| 提取了现金折扣          | 0.00      |
| 要提取的现金折扣金额 | -20.00    |

April 将**要结算的金额**字段中的值更新为 **500.00**。 **要提取的现金折扣金额**字段中的值计算为 **5.05**。

| 标记                     | 使用现金折扣 | 凭证   | 帐户 | 日期      | 到期日期  | 开票 | 交易记录币种金额 | 货币 | 要结算的金额 |
|--------------------------|-------------------|-----------|---------|-----------|-----------|---------|--------------------------------|----------|------------------|
| 已选择和突出显示 | 标准            | Inv-10030 | 3052    | 6/28/2015 | 7/12/2015 | 10030   | 2,000.00                       | 美元      | -500.00          |
| 选定                 | 标准            | APP-10030 | 3052    | 7/15/2015 | 7/15/2015 |         | 500.00                         | 美元      | 500.00           |

折扣信息显示在**结算未结交易记录**页的底部。 **要提取的现金折扣金额**字段中的值为 **5.05**，因为要结算的发票金额更改为了付款金额 500.00。

|                              |           |
|------------------------------|-----------|
| 现金折扣日期           | 7/12/2015 |
| 现金折扣金额         | -20.00    |
| 使用现金折扣            | 标准    |
| 提取了现金折扣          | 0.00      |
| 要提取的现金折扣金额 | -5.05     |





