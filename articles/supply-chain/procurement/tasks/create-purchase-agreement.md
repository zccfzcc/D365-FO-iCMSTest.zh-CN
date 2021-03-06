---
title: 创建采购协议
description: 该过程会从头至尾指导您创建一份采购协议。
author: mkirknel
manager: AnnBe
ms.date: 08/29/2018
ms.topic: business-process
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: PurchAgreement, PurchAgreementCreate, InventItemIdLookupSimple, AgreementConfirmRunForm, PurchAgreementHistory
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.search.region: Global
ms.author: mkirknel
ms.search.validFrom: 2016-06-30
ms.dyn365.ops.version: Version 7.0.0
ms.openlocfilehash: c86024de6012dbfa10bafe53fd33029c096ab253
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "56421"
---
# <a name="create-a-purchase-agreement"></a>创建采购协议

[!include [task guide banner](../../includes/task-guide-banner.md)]

该过程会从头至尾指导您创建一份采购协议。 这通常由采购经理完成。 您可以使用演示数据公司 USMF，也可使用您自己的数据运行该过程。 在您开始之前，您需要设置采购协议分类。 一旦创建完协议，您可以在创建采购订单时使用该协议，并且这会将采购协议条件复制到受该协议影响的订单的标题和任何行。


## <a name="create-a-new-purchase-agreement"></a>新建采购协议
1. 转到“采购”>“采购协议”>“采购协议”。
2. 单击“新建”。
3. 在“供应商帐户”字段中，单击下拉按钮以打开查找。
4. 在列表中，找到并选择所需记录。
5. 在列表中，单击所选行中的链接。
6. 在“采购协议分类”字段中，单击下拉按钮以打开查找。
7. 在列表中，找到并选择所需记录。
8. 在列表中，单击所选行中的链接。
9. 展开“常规”部分。
10. 在“到期日期”字段中，输入一个日期。
    * 此到期日期将是所有承诺行的默认设置，并将确定每个特定承诺的有效期有多长。  
11. 在“文件标题”字段中，键入您的采购协议的名称。
    * 将“默认承诺”字段设置为“产品数量承诺”（或者进行更改，如果未设置为产品数量承诺）。  
    * 默认承诺值可确定您在协议行上的选项。 如果在创建协议行时，您需要新的承诺类型，则您需要更改标题上的默认承诺。  共有 4 种类型的承诺：产品数量承诺 - 适用于特定数量的产品；产品价值承诺 - 适用于特定币种金额的产品；产品类别价值承诺 - 适用于特定币种金额的采购类别，其中金额可以是某一目录物料或非目录物料的金额；价值承诺 - 适用于可由任何产品或任何采购类别实现的特定币种金额。  
12. 单击“确定”。

## <a name="add-a-commitment"></a>添加承诺
1. 单击“添加行”。
2. 在列表中，标记所选的行。
3. 在“物料编号”字段中，单击下拉按钮以打开查找。
4. 选择您想为其添加承诺的产品。
5. 在列表中，单击所选行中的链接。
6. 在“数量”字段中，输入一个数字。
    * 这是您同意从供应商采购的总数量。  
7. 在“单位价格”字段中，输入一个数字。
8. 展开“行明细”部分。
9. 将“最大值”强制选项设置为“是”。
    * “最大值”是强制执行的选项，以限制承诺的使用。 您只能最多购买“数量”字段中规定的该行的数量。  
10. 收起“行详情”部分。

## <a name="add-header-conditions"></a>添加标题条件
1. 在“操作窗格”上，单击“选项”。
2. 单击“更改”视图。
3. 单击“标题”视图。
4. 展开“条款”部分。
5. 在“付款方式”字段中，单击下拉按钮以打开查找。
    * 供应商帐户的付款条件会默认显示在此。       
6. 在列表中，找到并选择所需记录。
7. 在列表中，单击所选行中的链接。
8. 在“交货方式”字段中，单击下拉按钮以打开查找。
9. 在列表中，单击所选行中的链接。
10. 在“交货条款”字段中，单击下拉按钮以打开查找。
11. 在列表中，单击所选行中的链接。

## <a name="confirm-and-activate-the-agreement"></a>确认并激活协议
1. 在“操作窗格”上单击“采购协议”。
2. 单击“确认”。
    * 将“标记协议为有效选项”设置为“是”。  
3. 单击“确定”。
4. 在“操作窗格”上单击“采购协议”。
5. 单击“采购协议确认”。
    * “预览/打印”选项允许您生成一份采购协议文件，然后您可以打印或发送给供应商。 如果您随后更新并再次确认该协议，则会在此显示两个版本的协议。  
6. 关闭该页面。

