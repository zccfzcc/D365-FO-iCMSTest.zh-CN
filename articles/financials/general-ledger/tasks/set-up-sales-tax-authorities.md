---
title: 设置增值税主管机构
description: 销售税主管机构是收缴需要申报和缴纳的销售税的实体。
author: twheeloc
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TaxAuthority
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: vstehman
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: b3e7e9952de8a04e2d72b1393dd52e6c4421f785
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54085"
---
# <a name="set-up-sales-tax-authorities"></a>设置增值税主管机构

[!include [task guide banner](../../includes/task-guide-banner.md)]

销售税主管机构是收缴需要申报和缴纳的销售税的实体。 您可以直接向销售税主管机构支付销售税，也可以通过为销售税主管机构创建的供应商帐户支付。 如果您这样做，公司可以使用其日常付款程序及时向增值税主管机构付款。 如果您没有将增值税主管机构设置为供应商，则某个人必须在相应的到期日期时准备向增值税主管机构手动付款。 本任务使用 USMF 公司进行演示。

1. 转到“纳税”>“间接税”>“销售税”>“销售税主管机构”。
2. 单击“新建”。
3. 在“主管机构”字段中，输入一个值。
4. 在“名称”字段中，键入一个值。
5. 在“供应商帐户”字段中，单击下拉按钮以打开查找。
6. 在列表中，找到并选择所需记录。
7. 在列表中，单击所选行中的链接。
8. 为您的国家/地区选择报表版式（如果有）。 如果报表版式不对应于销售税主管机构的要求，请使用默认版式。
9. 在舍入表格和“舍入”字段中输入数字，以指定支付的总税额如何舍入。 所有舍入差额将过帐到总帐中设置的自动交易记录的帐户。
10. 在“舍入”字段中，输入一个数字。
11. 单击“保存”。

