---
title: 查看和导出字段描述
description: 本文介绍了如何查看字段描述以及如何使用字段描述页导出描述。
author: rschloma
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: FieldDescriptions
audience: Application User, Developer, IT Pro
ms.reviewer: rschloma
ms.search.scope: Core, Operations
ms.custom: 11534
ms.assetid: e2795f51-a8a7-4c74-bdb9-b1be93bdd358
ms.search.region: Global
ms.author: rschloma
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 17f6e65f6ffa6534288f00edbeef8e4721babfcd
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54271"
---
# <a name="view-and-export-field-descriptions"></a>查看和导出字段描述

[!include [banner](../includes/banner.md)]

本文介绍了如何查看字段描述以及如何使用字段描述页导出描述。

Microsoft Dynamics 365 for Finance and Operations 具有某些较为复杂的字段的描述。 在您将鼠标悬停在某个字段时，这些描述将显示。 您还可以在**字段描述**页查看和导出描述。 

并非所有页都有字段描述。 我们只为较为复杂的字段提供描述，不为用法明显的字段提供。 因此，某些页没有任何字段描述，某些页有一些描述，而一些较复杂的页面（如很多参数页）有很多描述。 

如果您有权访问 Finance and Operations 开发环境，则可添加新字段描述并自定义现有描述。 例如，您可以添加特定于公司的信息到字段描述。 有关详细信息，请参阅[自定义字段帮助](../../dev-itpro/user-interface/customize-field-help.md)。

## <a name="see-field-descriptions-in-the-user-interface"></a>参阅用户界面的字段描述
您可以通过将鼠标悬停到字段上查看字段描述。 如果没有提供描述，当您将鼠标悬停在字段上时将看到字段名。 （注意：在版本 Dynamics AX 7.0（2016 年 2 月）中，仅可在**字段描述**页上查看字段描述。）下面的插图显示将鼠标悬停在**盘点期间锁定物料**字段上时将显示的字段描述。 

[![字段描述的示例](./media/field-description.png)](./media/field-description.png)

## <a name="use-the-field-descriptions-page-to-view-and-export-field-help"></a>使用字段说明页查看和导出字段帮助
**字段描述**页允许查看和导出字段描述。 您可以一次查看一页的可用描述。

### <a name="view-the-descriptions-for-a-page"></a>查看页的描述

要查看页的描述，请按以下步骤操作。

-   在**选择页面**字段中，键入页面的名称。 或者，单击箭头打开所有页的列表，然后浏览或筛选列表。

您可以使用在用户界面 (UI) 显示的页面名称（例如，**客户**），或在右键单击页面时出现的代码名称（AOT 名称）（例如，**CustTable**）。 

有关筛选页面列表的各种方式的信息，请参阅本文下文的“搜索页面”部分。 

如果设置**包含字段，但不带描述**选项为**是**，页面中的所有字段都将显示，即使它们没有字段描述。

### <a name="export-the-descriptions-for-a-page"></a>导出页的描述

要导出页的描述，请按以下步骤操作。

1.  在**选择页面**字段中，选择一个页面。
2.  单击右上角的**在 Microsoft Office 中打开**按钮，然后单击 **FieldDescriptionTmp**。

### <a name="searching-for-a-page"></a>搜索页

可通过多种方法在**选择页面**字段中搜索页。 在许多情况下，必须单击**选择页面**字段中的箭头才能打开下拉列表，然后在筛选后的页列表中进行选择。

-   键入名称的一部分，然后打开下拉列表以从筛选后的页列表中进行选择。
-   打开下拉列表，然后单击列表顶部的**页面名称**标题，或**页面 AOT 名称**标题。 这将出现一个对话框，供您使用高级筛选选项，如**页面名称开始于**。
-   键入页面的全名。 如果使用此选项，最好打开下拉列表，看看列表中的其他选项，即使显示了字段描述。
    -   如果名称只有一个精确匹配项，将显示该页的字段描述。
    -   如果有多个精确匹配，则不显示描述。 您必须打开下拉列表并选择所需的网页。
    -   如果您键入的名称是另一个页面的名称的一部分，您会看到您的页面的描述。 但是，如果打开下拉列表，您将看到包含该名称的其他页面。

例如，当您在*<strong><em>选择页面</em></strong>* 字段键入<strong>盘点</strong>时，将不显示描述。 您打开下拉列表，将看到具有名称<strong>盘点</strong>的两个页面，以及名称中包含字词“盘点”的若干页面。 如果选择 AOT 名称为 <strong>InventJournalCount</strong> 的页，将显示该页的字段描述。 但是，如果再次打开下拉列表，将看到列表中现在包含 AOT 名中包含“InventJournalCount”的所有页。

## <a name="troubleshooting"></a>疑难解答
此部分提供的信息帮助您解决使用字段描述页时可能遇到的问题。

### <a name="i-cant-find-a-field-description"></a>我找不到字段描述

我们正在为较为复杂的字段添加描述。 如果您需要有关特定字段的帮助，请通过评论此主题告知我们。

### <a name="the-field-description-isnt-helpful"></a>此字段描述没有帮助

请通过评论此主题告知我们。 如果可能，请描述所需的其他信息。

### <a name="i-cant-find-a-field-on-the-field-descriptions-page"></a>我在字段描述页上找不到字段

要显示某页中的所有字段，请将**包含字段，但不带描述**选项设置为**是**。 单击**选择页面**字段，以确认选择了正确的页面。 如果您键入的名称是另一个字段名称的一部分，您可能已经选择了具有更长名称的页面。

### <a name="i-cant-find-a-page-on-the-field-descriptions-page"></a>我在字段描述页上找不到页面

有关查找页面的各种方式的信息，请参阅本文先前部分的“搜索页面”部分。 如果已键入了页的精确名称，但是多页同名，可能不显示字段描述。 单击**选择页面**字段中的箭头打开筛选后的可用页列表。

<a name="additional-resources"></a>其他资源
--------

[自定义字段帮助](../../dev-itpro/user-interface/customize-field-help.md)




