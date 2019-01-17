---
title: 确定叠加折扣的最佳组合
description: 折扣叠加时，必须确定将产生最低交易记录总额或最高折扣总额的叠加折扣组合。 当折扣金额根据购买的产品价格变化时（如常见的“第二件打折”(BOGO) 零售折扣），此过程就成为了组合优化问题。
author: kfend
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
ms.search.form: RetailParameters, RetailPeriodicDiscount,
audience: Application User, IT Pro
ms.reviewer: kfend
ms.search.scope: Core, Operations, Retail
ms.custom: 89643
ms.assetid: 09843c9a-3e19-4e4a-a8ce-80650f2095f9
ms.search.region: global
ms.search.industry: Retail
ms.author: kfend
ms.search.validFrom: 2016-05-31
ms.dyn365.ops.version: AX 7.0.1
ms.openlocfilehash: 7a2ff7cafd630f70c9e7913faba9b02c61dd0ce5
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "53606"
---
# <a name="determine-the-optimal-combination-of-overlapping-discounts"></a>确定叠加折扣的最佳组合

[!include [banner](includes/banner.md)]

折扣叠加时，必须确定将产生最低交易记录总额或最高折扣总额的叠加折扣组合。 当折扣金额根据购买的产品价格变化时（如常见的“第二件打折 (BOGO) 零售折扣），此过程就成为了组合优化问题。

本文适用于带 KB 3105973 的 Microsoft Dynamics AX 2012 R3（发布日期为 2015 年 11 月 2 日），以及 Microsoft Dynamics 365 for Retail。 要确定要及时应用的叠加折扣组合，我们引入了一种应用叠加折扣的方法。 我们把这种方法称为**临界值分级**。 当评估叠加折扣的可行组合所需时间超过了可在**零售参数**页面上配置的阈值时，使用临界值方法。 在临界值分级方法中，将通过使用共享产品的折扣值，计算各叠加折扣的值。 然后将叠加折扣从最高相对值应用于最低相对值。 有关这种新方法的详细信息，请参阅本文后面的“临界值”部分。 产品的折扣金额不受交易记录中的其他产品影响时，不使用临界值分级。 例如，此方法不用于两个简单折扣，也不用于一个简单折扣加单一产品数量折扣。

## <a name="discount-examples"></a>折扣示例
您可为一组普通产品创建数量不受限制的零售折扣。 但是，由于没有限制，所以尝试计算应对多种产品使用的折扣时，可能发生性能问题。 以下示例更详细地说明此问题。 在示例 1 中，首先是两件产品和两个叠加折扣。 然后在示例 2 中，我们显示随着添加更多产品，问题如何发展。

### <a name="example-1-two-products-and-two-discounts"></a>示例 1：两件产品和两种折扣

在此示例中，需要两件产品都符合各折扣的资格，并且折扣不能组合。 此示例中的折扣为**最优价格**折扣。 两件产品都符合两种折扣的资格。 这里是两种折扣。
![叠加折扣组合 01](./media/overlapping-discount-combo-01.jpg)

对于任意两件产品，这两个折扣中更优惠的取决于这两件产品的价格。 两件产品的价格相等或几乎相等时，折扣 1 更优惠。 当一件产品的价格比另一件产品的价格低得多时，折扣 2 更优惠。 下面是针对彼此评估这两个折扣的数学规则：![叠加折扣组合 02](./media/overlapping-discount-combo-02.jpg)

**注意：** 产品 1 的价格等于产品 2 价格的三分之二时，这两个折扣相等。 在此示例中，折扣 1 的有效折扣百分比多种多样，从较小百分比（当两件产品的价格相差很大时）到最大 25%（当两件产品价格相同时）。 折扣 2 的有效折扣百分比是固定值。 始终为 20%。 因为折扣 1 的有效折扣百分比的范围可以大于或小于折扣 2，所以最优折扣取决于必须打折的两件产品的价格。 在此示例中，计算的完成速度很快，因为仅对两件产品应用两个折扣。 只能有两种组合：一折扣 1 应用一次，折扣 2 应用一次。 没有要计算的序列。 每个折扣的值通过同时使用两件产品计算，并使用最优折扣。

### <a name="example-2-four-products-and-two-discounts"></a>示例 2：四件产品和两种折扣

接下来，我们将使用四件产品和同样的两种折扣。 所有四件产品都符合两种折扣的资格。 可以有 12 种组合。 最后，将通过以下三种组合之一为交易记录应用两种折扣：折扣 1 应用两次，折扣 2 应用两次，或者折扣 1 应用一次，折扣 2 应用一次。 为了演示可行组合，我们将查看具有不同价格的四件产品的两个不同组合：

-   所有四件产品的价格都相同，为 15.00 美元。 在这种情况下，最优折扣组合为折扣 1 应用两次。 两件产品为全价，两件为五折。 交易记录的折扣后总额为 45 美元 (15 + 15 + 7.50 + 7.50)，其中的 15 美元 (25%) 是正价 60 美元的折扣。 折扣 2 为仅 12 美元 (20%)。
-   两件产品分别 20 美元，一件产品 15 美元，一件产品 5 美元。 在这种情况下，最优折扣组合为折扣 2 应用一次，折扣 1 应用一次。 下面的表演示这些折扣。

要理解这些表，请使用一行中的一件产品和一列中的一件产品。 例如，在折扣 1 的表中，组合两个 20 美元的产品时，折扣为 10 美元。 在折扣 2 的表中，组合 15 美元的产品和 5 美元的产品时，折扣为 4 美元。
![叠加折扣组合 03](./media/overlapping-discount-combo-03.jpg)

首先，我们通过使用其中一种折扣找到任意两件产品的最大可行折扣。 两个表显示两件产品所有组合的折扣金额。 表的阴影部分表示产品与自身配对的情况（这种情况无法实现），或者产生相同折扣金额并且可以忽略的两件产品交换配对。 通过查看表，可以发现两件 20 美元物料的折扣 1 是所有四件产品其中一种折扣的最大可行折扣。 （此折扣在第一个表中以绿色突出显示。）这样仅保留 15 美元的产品和 5 美元的产品。 通过再次查看这两个表，可以发现对于这两件产品，折扣 1 的折扣为 2.50 美元，而折扣 2 的折扣为 4 美元。 因此，我们选择折扣 2。 折扣总额为 14 美元。 要使此折扣更容易可视化，下面还有两个表，其中显示折扣 1 和 折扣 2 所有两个可行产品组合的有效折扣百分比。 仅包括组合列表中的一半，因为对于这两种折扣，这两种产品的折扣顺序没有影响。 最高有效折扣 (25%) 以绿色突出显示，而最低有效折扣 (10%) 以红色突出显示。 

![叠加折扣组合 04](./media/overlapping-discount-combo-04.jpg)

**注意：** 价格多种多样，并且两种或多种折扣竞争时，只能通过评估和比较折扣才能确保最优折扣组合。

## <a name="total-possible-combinations"></a>可行组合总数
本部分继续使用上一部分的示例。 我们将增加更多产品和一种折扣，并了解必须计算和比较多少种组合。 下表显示随着产品数量增加产生的可行折扣组合数量。 此表显示有两种叠加折扣（如上一个示例中）和有三种叠加折扣时的结果。 必须评估的可行折扣组合数量很快超过其计算和比较性能足以让零售交易记录接受的快速计算机的承受能力。

![叠加折扣组合 05](./media/overlapping-discount-combo-05.jpg)

应用甚至更大的数量或更多叠加折扣时，可行折扣组合总数很快将变为百万级，并且快速评估和选择最优可行组合所需时间将变得引人瞩目。 已经在零售价格引擎中执行了一些优化，以便减少必须评估的组合的总数。 但是，因为交易记录中的叠加折扣数量和产品数量不受限制，所以只要存在叠加折扣，就必须评估大量组合。 临界值方法可以解决这个问题。

## <a name="marginal-value-method"></a>临界值方法
若要解决必须评估的组合数量呈指数增长这一问题，可以通过优化来计算可应用两种或多种折扣的产品集的每个折扣的共享产品的值。 我们将该值称为共享产品的折扣的**临界值**。 临界值是在每种折扣中计算共享产品时，折扣总额中每个产品增长的平均值。 临界值的计算方法是，采用折扣总额 (DTotal),，减去不含共享产品的折扣金额 (DMinus\\ Shared)，然后将差除以共享产品数量 (ProductsShared)。 
![叠加折扣组合 06](./media/overlapping-discount-combo-06.jpg)

计算了一组共享产品的每种折扣的临界值之后，将按照从最高临界值到最低临界值的顺序，依次将折扣详尽地应用于共享产品。 对于此方法，应用了一种折扣的单个实例之后，不会每次都比较其余可行折扣。 而是比较一次叠加折扣，然后依次应用这些折扣。 无需再执行任何比较。 可以在**零售参数**页面的**折扣**选项卡上配置阈值以切换到临界值方法。 零售行业中计算折扣总额所用可接受时间多种多样。 但是，此时间的范围通常为几十毫秒到一秒。


