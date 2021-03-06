---
title: 设置销售税申报代码
description: 销售税报表代码指销售税报表上的字段编号。
author: twheeloc
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: TaxReportCollection
audience: Application User
ms.reviewer: twheeloc
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: vstehman
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: 05e30ee70d37af57fe5e4c67bca4a419ba4ced54
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56138"
---
# <a name="set-up-sales-tax-reporting-codes"></a>设置销售税申报代码

[!include [task guide banner](../../includes/task-guide-banner.md)]

销售税报表代码指销售税报表上的字段编号。 这些代码在国家特定的报表版式上使用，并且根据代码识别的销售税付款按照申报代码，申报打印一定结算期间内的销售税金额。 在创建销售税申报代码后，您可以在销售税代码页面的“报告设置”快速选项卡中引用这些代码。 

此记录使用 DEMF 公司演示。



1. 转到“纳税”>“设置”>“销售税”>“销售税申报代码”。
2. 单击“新建”。
3. 选择申报代码所属的报表版式。
    * 此版式用于筛选销售税代码的可用申报代码。 每个销售税代码属于使用报表版式的销售税主管机构的结算期间。  
4. 输入引用销售税报表中的字段的编号。
5. 在“报表文本”字段中，输入在报表中显示的描述。
6. 在“简单描述”字段中，输入用于内部的描述。
7. 单击“保存”。

