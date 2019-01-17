---
title: 销售点 (POS) 中的产品搜索和客户搜索
description: 此主题概述 Microsoft Dynamics 365 for Retail 中的产品和客户搜索的增强功能。
author: ShalabhjainMSFT
manager: AnnBe
ms.date: 03/28/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-365-retail
ms.technology: ''
audience: Application user
ms.reviewer: josaw
ms.search.scope: Core, Operations, Retail
ms.custom: 141393
ms.assetid: ''
ms.search.region: Global
ms.search.industry: Retail
ms.author: shajain
ms.search.validFrom: 2017-06-30
ms.dyn365.ops.version: Retail April 2017 update
ms.openlocfilehash: a8279db6c46206658a90bf66f9d906d1af7087d1
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54774"
---
# <a name="product-search-and-customer-search-in-the-point-of-sale-pos"></a>销售点 (POS) 中的产品搜索和客户搜索

[!include [banner](includes/banner.md)]

现代销售点 (MPOS) 和云销售点 (CPOS) 提供易于使用的搜索功能，便于搜索产品和客户。 由于搜索栏始终显示在 MPOS 和 CPOS 窗口顶部，因此员工可以快速搜索产品和客户。

员工可以在与当前商店关联的分类和目录中搜索产品。 还可以在与公司其他任何商店关联的分类和目录中搜索。 因此，出纳可以销售和退回商店分类以外的产品。 同样，员工可以搜索与当前商店或公司中的任何其他商店关联的客户。 此外，员工可以搜索与父组织中的不同公司关联的客户。

## <a name="product-search"></a>产品搜索

默认情况下，对商店分类执行产品搜索。 此类搜索被称为*本地产品搜索*。 但是，员工可以轻松切换到与当前商店关联的任何目录，或在不同商店中进行搜索。 此类搜索被称为*远程产品搜索*。 若要更改目录，请选择页面左侧的**类别**按钮。 在显示的窗格顶部，选择**更改目录**按钮，然后选择一个可用的目录进行浏览。 系统将在选定目录中搜索产品。

在**更改目录**页上，员工可以轻松选择任何商店，或者可以跨所有商店搜索产品。

![更改目录](./media/Changecatalog.png "更改目录")
 
本地产品搜索在以下产品属性中进行搜索：

- 产品编号
- 产品名称
- 说明
- 维度
- 条码
- 搜索名称

### <a name="enhancements-to-local-product-searches"></a>本地产品搜索增强功能

本地产品搜索的体验现在对用户更加方便。 我们实现了以下增强功能：

- 在搜索栏中添加了产品和客户下拉菜单，使员工在执行搜索前可以选择**产品**或**客户**。 默认情况下，选择**产品**，如下图中所示。
- 对于多个关键字搜索（即使用搜索词的搜索），零售商可以配置搜索结果是否包括匹配*任何*搜索词的结果或仅包括匹配*所有*搜索词的结果。 此设置在 POS 功能配置文件中命名为**产品搜索**的新组中可用。 默认设置为**匹配任何搜索词**。 此设置也是建议的设置。 如果使用**匹配任何搜索词**设置，将把完全或部分匹配一个或多个搜索词的所有产品作为结果返回。 这些结果将自动按照关键字匹配项（完全或部分）最多的产品的升序排序。

    **匹配所有搜索词**设置仅返回（完全或部分）匹配所有搜索词的产品。 当产品名称较长，且员工只想查看搜索结果中的有限产品时，此设置有用。 但是，该搜索类型有两个限制：

    - 对单独的产品属性进行搜索。 例如，仅返回在至少一个产品属性中具有所有搜索关键字的产品。
    - 不搜索维度。

- 零售商现在可以将产品搜索配置为当用户键入产品名称时显示搜索建议。 此功能的新设置在 POS 功能配置文件中命名为**产品搜索**的组中可用。 设置命名为**在键入时显示搜索建议**。 此功能使员工无需手动键入全部名称，因此可以帮助员工快速查找其搜索的产品。
- 产品搜索算法现在可以搜索在产品的**搜索名称**属性中搜索的词语。

![产品建议](./media/Productsuggestions.png "产品建议")

## <a name="customer-search"></a>客户搜索

客户搜索用于根据不同目的查找客户。 例如，出纳可能想要查看客户的愿望列表或购买历史记录，或将客户添加到交易记录。 在多个关键字搜索的情况下，客户搜索算法返回与任何搜索的关键字匹配的所有客户。 但是，匹配最多关键字的客户显示在结果的顶部。 此行为与其他搜索引擎显示结果的方式类似。 先显示匹配最多搜索词的结果，然后显示部分匹配搜索关键字的结果。 出现出纳使用多个关键字进行搜索，但其中一个关键字拼写错误的情况下，此行为有用。

默认情况下，客户搜索在与商店关联的客户通讯簿中执行。 此类搜索被称为*本地客户搜索*。 但是，员工也可以搜索全局客户。 换而言之，他们可以跨公司及所有其他法人的商店进行搜索。 此类搜索被称为*远程客户搜索*。

要执行全局搜索，员工可以选择页面底部的**筛选结果**按钮，然后选择**搜索所有商店**选项，如下图中所示。 在这种情况下，不止返回客户。 也返回属于总部中的任何通讯簿的所有类型的相关方。 这些相关方包括工作人员、供应商、联系人和竞争对手。

> [!NOTE]
> 远程客户搜索中必须输入至少四个字符才能返回结果。

在远程客户搜索中，不显示来自其他法人的客户的客户 ID，因为没有在当前公司为这些相关方创建客户 ID。 但是，如果员工打开客户详细信息页，系统将自动为相关方生成一个客户 ID，且将商店的客户通讯簿与该客户相关联。 因此，该客户将在以后执行的本地商店搜索中可见。

![全局客户搜索](./media/Globalcustomersearch.png "全局客户搜索")

### <a name="enhancements-to-local-customer-search"></a>本地客户搜索增强功能

已简化了基于电话号码的搜索。 此类搜索现在忽略创建客户时可能添加的特殊字符，如空格、连字符和括号。 因此，收银员在进行搜索时无需担心电话号码格式。 也可以通过键入部分电话号码搜索客户。 如果电话号码中包含特殊字符，也可以通过搜索特殊字符后显示的数字查找。 例如，如果输入的客户电话号码为 **123-456-7890**，则收银员可以通过键入 **123**、**456**、**7890** 或 **1234567890** 来搜索客户，也可以通过输入电话号码的前几个数字来搜索客户。

传统的客户搜索可能很费时间，因为要在多个字段中进行搜索。 不过，收银员现在可在单个自定义属性（如姓名、电子邮件地址或电话号码）中进行搜索。 客户搜索算法使用的属性统称为*客户搜索条件*。 系统管理员可以轻松地将一个或多个条件配置为 POS 中显示的快捷方式。 因为搜索限制为单个条件，所以将仅显示相关搜索结果，而性能则比标准客户搜索的性能好得多。 下图显示 POS 中的客户搜索快捷方式。

![客户搜索快捷方式](./media/SearchShortcutsPOS.png "客户搜索快捷方式")

若要设置搜索条件快捷方式，管理员必须在 Microsoft Dynamics 365 for Finance and Operations 中打开**零售参数**页，然后在 **POS 搜索条件**选项卡上选择所有应显示为快捷方式的条件。

![配置搜索快捷方式](./media/ConfigureShortcutsAX.png "配置搜索快捷方式")

> [!NOTE]
> 如果添加的快捷方式过多，POS 中搜索栏上的下拉菜单将变得杂乱不堪，从而可能影响员工的搜索体验。 建议仅根据需要添加快捷方式。

**显示顺序**字段确定快捷方式在 POS 中的显示顺序。 显示的条件是客户搜索算法用于搜索客户的自带属性。 但是，合作伙伴可以添加自定义属性作为搜索快捷方式。 若要将自定义属性添加为搜索快捷方式，系统管理员必须扩展用于客户搜索条件的可扩展枚举，然后将合作伙伴的自定义属性标记为快捷方式。 合作伙伴负责编写代码以在其自定义快捷方式用于搜索时查找结果。

> [!NOTE]
> 添加到枚举的自定义属性不影响标准客户搜索算法。 换言之，客户搜索算法不在自定义属性中进行搜索。 仅当自定义属性添加为快捷方式时或替代了默认搜索算法时，用户才能将该自定义属性用于搜索。