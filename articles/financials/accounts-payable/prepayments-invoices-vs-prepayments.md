---
title: 预付款发票与预付款
description: 本主题介绍和对比组织可以用于预付款（预先付款）的两种方法。 在一种方法中，您创建与采购订单相关联的预付款发票。 在另一种方法中，您通过创建日志条目并将它们标记为预付款日志凭证来创建预付款日志凭证。
author: ShivamPandey-msft
manager: AnnBe
ms.date: 10/26/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: LedgerJournalTransVendPaym, PurchTable
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 15871
ms.assetid: a0bb5220-73d4-48ae-84d0-46a171c224fa
ms.search.region: Global
ms.author: shpandey
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 51a24e68b10e1654017a2034cbf9ac8ffbfee2ae
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54277"
---
# <a name="prepayment-invoices-vs-prepayments"></a>预付款发票与预付款

[!include [banner](../includes/banner.md)]

本主题介绍和对比组织可以用于预付款（预先付款）的两种方法。 在一种方法中，您创建与采购订单相关联的预付款发票。 在另一种方法中，您通过创建日志条目并将它们标记为预付款日志凭证来创建预付款日志凭证。

组织可能向货物或服务的供应商发布预付款（在满足这些货物或服务之前）。 两种方法可用于向供应商发布预付款。 若要将风险最小化，您可以通过跟踪采购订单上的预付款跟踪这些预付款。 对于此方法，您必须创建与采购订单相关联的预付款发票。 此方法称为预付款开票。 不想那么紧密跟踪预付款或不从供应商那里接收预付款发票的组织可以使用预付款日记帐凭证，而不是预付款开票方法。 您可以通过创建日志条目并将它们标记为预付款日志凭证来创建预付款日志凭证。 对于此方法，您不能跟踪根据那个采购订单对供应商进行哪种预付款。 但是，您可以比对采购订单标记要进行结算的过帐预付款。

## <a name="when-to-use-prepayment-invoicing-vs-prepayments"></a>什么时候使用预付款开票与预付款

| 预付款开票                                                                | 预付款                                                              |
|-------------------------------------------------------------------------------------|--------------------------------------------------------------------------|
| 在采购订单上定义预付款值。                                    | 在采购订单上未定义预付款值。                    |
| 键：必须过帐预付款发票和最终发票。                       | 不必过帐预付款发票。                                    |
| 预付款的义务保留在预付款帐户中，不在 AP 帐户中。 | 预付款的义务保留在 AP 帐户中。                  |
| 供应商余额不反映整个流程中的预付款值。     | 供应商余额反映整个流程中的预付款值。 |
| 预付款开票只可用于应付账款。                         | 预付款可用于应付账款和应收账款。    |

## <a name="overview-of-the-prepayment-process"></a>预付款流程的概览
许多国家/地区中的会计实务都要求来自某一客户或向某一供应商的预付款（提前付款）不过帐到该客户或供应商的日常汇总科目中。 这些预付款而是过帐到用于预付款的特殊会计科目中。 当创建销售订单或采购订单时，向客户或从供应商签发发票。 当支付发票时，冲销预付款会计科目上的预付款和销售税预付款凭证，发票金额将自动过帐到日常汇总科目上。 遵循这些步骤创建预付款。

1.  设置预付款的过帐模板。
2.  在应收账款参数和应付账款参数中，在**分类帐和销售税**下，使用**具有预付款的付款日记帐的过帐模板**参数选择新的过帐模板。
3.  创建一个付款日记帐，然后创建新的付款。
4.  您可以将付款标记为预付款。 If a payment is flagged as a prepayment, the payment is posted to the ledger accounts that are defined on the posting profile that you set up in steps 1 and 2. 此外，如果付款标记为预付款，则会计算税金。 某些政府需要在记录预付款时支付税金，即使没有发票也是。
5.  过帐预付款。
6.  Optional: You can settle the prepayment against the purchase order or sales order before you create the invoice. On the sales order or purchase order page, on the Action Pane, use **Settle transactions**.
7.  在供应商提供货物或服务之后，应记录发票。 如果您在第 6 步中已比对采购订单或销售订单结算预付款，则会自动比对您创建的发票来结算预付款。 如果您未比对采购订单或销售订单结算预付款，则可以通过使用客户或供应商页上的 **“结算交易记录”** 来手动结算它。 然后，预付款金额将暂时冲销到 AP/AR 会计科目之外。 此外，如果计算税金，它们将被冲销，因为发票具有实际税金。

## <a name="overview-of-the-prepayment-invoicing-process"></a>预付款开票流程的概览
预付款发票是一个常见业务实践。 在履行采购订单前，供应商会签发预付款发票以要求为采购存款。 例如，某些供应商要求客户货物或服务的预付款。 如果供应商签发一个请求预付款的发票，您可以使用预付款开票功能。 预付款值可以在采购订单上定义，预付款发票会被记录并支付，然后预付款应用于最终发票。 遵循这些步骤创建预付款。

1.  采购代理创建、确认，然后提交供应商已请求预付款的采购订单。 预付款值是在采购订单上定义的，作为协议的一部分。
2.  供应商提交了一个预付款发票。
3.  应付账款协调员记录了针对采购订单的预付款发票，然后支付预付款发票。
4.  在供应商交付了货物或服务并已接收相关供应商发票后，应付账款协调员将应用针对该发票已支付的预付款金额。
5.  应付账款协调员支付并结算了该发票的剩余金额。




