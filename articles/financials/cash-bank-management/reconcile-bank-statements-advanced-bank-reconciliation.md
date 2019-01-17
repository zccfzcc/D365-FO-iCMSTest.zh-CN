---
title: 使用高级银行对帐对银行对账单进行对帐
description: 高级银行对帐功能让您可以导入电子银行对帐单，并可以将其与 Microsoft Dynamics 365 for Finance and Operations 中的银行交易记录自动对帐。 本主题说明对帐流程。
author: saraschi2
manager: AnnBe
ms.date: 01/11/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: BankReconciliationWorksheet
audience: Application User
ms.reviewer: shylaw
ms.search.scope: Core, Operations
ms.custom: 98243
ms.assetid: 9df13adf-aa9d-4f6b-bde6-25a214611692
ms.search.region: global
ms.author: saraschi
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: a3283a607e63086fb9acbd7de1c761e525591fbe
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54084"
---
# <a name="reconcile-bank-statements-by-using-advanced-bank-reconciliation"></a>使用高级银行对帐对银行对帐单进行对帐

[!include [banner](../includes/banner.md)]

高级银行对帐功能让您可以导入电子银行对帐单，并可以将其与 Microsoft Dynamics 365 for Finance and Operations 中的银行交易记录自动对帐。 本主题说明对帐流程。  

<a name="import-an-electronic-bank-statement"></a>导入电子银行对帐单
-----------------------------------

通过使用**银行对账单**页的**导入对账单**操作导入银行对账单。 在银行对账单上，银行帐户通过银行帐户详细信息中设置的值的组合识别。 这些值包括银行名称、银行帐号、路由号码、国际银行金融电信协会 (SWIFT) 代码和国际银行帐号 (IBAN)。 

您可以上传包含一个帐户或多个帐户的信息的银行对账单。 如果存在多个帐户，这些帐户可以使用不同的法人。

-   若要导入单个帐户的单个银行对账单文件，设置**导入所有法人的多个银行帐户的对账单**选项为**否**，并选择与该对账单关联的银行帐户。 单击**浏览**以选择相关联的银行对账单文件，然后单击**上载**。
-   若要导入多个帐户单个银行对账单文件，设置**导入所有法人的多个银行帐户的对账单**选项为**是**。 单击**浏览**以选择相关联的银行对账单文件，然后单击**上载**。

如果电子文件中的任何对账单无法通过使用标识字段与银行帐户相关联，则不会导入。 但是可以导入文件中的其他对账单。 随后用户将收到消息，指出特定银行帐户的银行对帐单导入不成功。 注意导入银行对账单文件的用户必须具有访问法人以导入该法人银行帐户对账单的权限。 

您可以使用 zip 文件在一个流程中将多个对账单文件上载到 Finance and Operations。 要导入多个帐户的多个银行对账单文件，将所有银行对账单文件合并到一个 zip 文件。 在**导入银行对账单**对话框中，将**导入所有法人的多个银行帐户的对账单**选项设为**是**。 单击**浏览**以选择包含银行对账单文件的 zip 文件，然后单击**上载**。 导入流程将识别 zip 文件并上载包含在其中的每一个对账单，无论银行帐户的法人。 

**在导入后对帐**选项可用。 将此选项设置为**是**时，系统自动验证银行对账单，创建一个新的银行对帐和工作表，并在上载银行对账单时运行默认匹配规则集。 此功能自动将流程运行到必须手动匹配交易记录的阶段。

## <a name="validate-the-bank-statement"></a>验证银行对账单
若要验证对账单，请单击**银行对账单**页面上的**验证**。 银行对账单必须先进行验证才能对帐。 如果在导入时将**在导入后对帐**选项设置为**是**，此步骤将自动完成。 

银行对账单验证验证以下详细信息︰

-   银行对账单与所选的银行帐户相匹配。
-   银行对账单货币与银行帐户货币相匹配。
-   对账单的期初余额等于银行帐户上一对账单的期末余额。
-   日期不重叠同一个银行帐户不同银行对账单的日期。
-   银行帐户对账单的日期没有间断。
-   对账单行上的日期在银行对账单的开始日期和结束日期之间。
-   期初余额和汇总的行金额等于期末余额。

完成验证后，将银行对账单的状态更新为**已验证**。 银行对账单必须先进行验证才能对帐。

## <a name="reconcile-the-bank-statement"></a>对银行对账单进行对帐
在**银行对账单**页导入电子银行对账单并验证对账单后，您可以使用**银行对帐**和**银行对帐工作表**页对银行对账单进行对帐。 

在**银行对帐**页，单击**新建**创建新对帐，然后选择导入的对账单的银行帐户。 银行帐户只能有一个未结银行对帐。 截止日期确定对帐工作表中包括的银行对帐交易记录和 Operations 银行交易记录。 默认情况下，当前系统日期用作截止日期，但您可以更改对帐的截止日期。 其余标头信息从对账单自动获取。 如果在导入时将**在导入后对帐**选项设置为**是**，此步骤将自动完成。 

在**银行对帐**页，单击**工作表**打开**银行对帐工作表**页。 如果**在导入后对帐**选项设置为**是**，将为对帐自动运行默认匹配规则集。 若要手动运行匹配规则，单击**运行匹配规则**选择要对银行交易记录运行的匹配规则集或匹配规则。 如果您有很多交易记录要处理，您可以作为批处理流程完成此步骤。 

**银行对帐工作表**页具有四个包含交易记录的网格。 两上上部网格显示尚未匹配的银行对账单和 Operations 的交易记录。 两个下部网格显示匹配的交易记录。 **银行对账单交易记录详细信息**选项卡显示在上部网格选择的未匹配的银行对账单交易记录的详细信息。 

有三种方法可以匹配或对帐银行对账单交易记录：

-   将交易记录与 Operations 银行交易记录匹配。
-   将交易记录与冲销银行对账单交易记录匹配。
-   将交易记录标记为**新**，以使其稍后能够在 Finance and Operations 中作为银行交易记录过帐。

若要手动匹配交易记录，在**银行对账单交易记录**网格中选择交易记录，在 **Operations 银行交易记录**网格中选择对应的交易记录，然后单击**匹配**。 所选交易记录从未匹配交易记录的上部网格移至匹配交易记录的下部网格。 而且，匹配和未匹配的总额将更新。 您可以进行一对一、多对一和多对多交易记录匹配。 匹配必须遵守允许的日期差异和交易记录类型映射规则。 这些规则在**现金和银行管理参数**页设置。

对帐中可能发生尾差。 如果尾差在银行帐户的**允许尾差**字段中定义的容差金额内，您可以匹配单个银行对账单交易记录和具有尾差的 Operations 银行交易记录。 金额显示在匹配的 Operations 银行交易记录上的**冲销金额**字段中。 银行对帐标记为已对帐后，使用在相关联的银行交易记录类型上定义的主科目自动过帐更正。 **支票**和**存款**单据类型不支持更正。 

银行对账单交易记录冲销使用对帐工作表匹配。 如果金额相反，且其中一个交易记录标记为冲销，可以匹配两个对账单行。 您还可以为**清算冲销对账单行**操作设置匹配规则。

冲销 Operations 银行交易记录必须使用**Operations 银行交易记录**页对帐。 如果单据具有相同的银行帐户、单据类型和付款参考，且它们具有相反金额，您可以同时对帐两个 Operations 银行交易记录。 您还可以对账单个取消的支票以阻止这些交易出现在对帐工作表中。 

如果有新的银行发起的不在 Finance and Operations 中的交易，如利息、费用和收费，您可以将这些交易添加到与所选银行对账单对帐关联的日记帐中。 在未匹配交易记录的**银行对账单交易记录**网格中选择银行对账单交易记录，然后单击**标记为新交易记录**。 交易记录的状态将设置为**新**，且交易记录将移至匹配交易记录的**银行对账单交易记录**网格。 稍后，您将从**银行对账单**页过帐标记为**新**的交易记录。 

您可以取消匹配未正确匹配的交易记录。 选择匹配的银行对账单交易记录，然后单击**取消匹配**。 所有相关交易记录将移回未匹配交易记录的上部网格，匹配和未匹配总额将更新。 

完成对帐流程后，您应该将银行对帐工作表标记为已对帐。  该流程将自动使用**银行交易记录类型**页上设置的科目过帐更正金额。  对账单的银行对帐可随时标记为已对帐，即使有尚未匹配的银行对账单行。  未匹配的交易记录将作为待对帐的未匹配的银行对账单交易记录自动移到下一个对帐工作表。  请注意，将银行对账单对帐标记为已对帐后，不能取消。  对帐将不可再编辑，且您将无法再对该对帐进行更新。

## <a name="post-new-transactions-that-are-associated-with-the-reconciliation"></a>过帐与对帐关联的新交易记录
在对帐工作表中标记为**新**的银行对账单交易记录在**银行对账单**页过帐。 在**银行对账单**页，选择要查看对账单详细信息的对账单 ID。 在**会计**菜单上，您可以使用**查看分配**和**查看会计**选项查看新交易记录和相关分类帐条目后面的详细信息。 选择**过帐**选项将标记为**新**的银行对账单行过帐到总帐。 请注意，每个银行对账单只能完成一次过帐。


