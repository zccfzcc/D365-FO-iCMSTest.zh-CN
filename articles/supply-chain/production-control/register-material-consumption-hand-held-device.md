---
title: 使用移动设备登记物料消耗量
description: 此主题介绍允许使用手持设备登记生产中的原材料消耗量的工作流。
author: johanhoffmann
manager: AnnBe
ms.date: 06/20/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: WHSRFMenuItem
audience: Application User
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 1706093
ms.assetid: 75ee68e0-4b9f-4f4d-b286-f498e0eb73fa
ms.search.region: Global
ms.author: johanho
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: 6e04e943e6f4a4ede80b2d2c211fc71e153f39f9
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "53167"
---
# <a name="register-material-consumption-using-a-mobile-device"></a>使用移动设备登记物料消耗量

[!include [banner](../includes/banner.md)]

此主题介绍允许使用手持设备登记生产中的原材料消耗量的工作流。

<a name="introduction"></a>简介
------------

This workflow is relevant if there is a strict requirement for material traceability. 在这些情况下，为了维护物料的可追踪性，必须申报消耗量的准确时间和数量。 此流程可能被视为与预先耗用或反向耗用工序（登记时间与发生实际消耗的时间之间存在偏移）相反。 这解释了为什么自动消耗策略无法用于具有可追踪性要求的一些物料。 Let’s look at a simple scenario that explains how to set up a workflow to enable registration of raw material consumption in production by using a handheld device. [![set up a workflow to enable registration of raw material consumption by using a handheld device](./media/scenario3.png)](./media/scenario3.png)

### <a name="scenario-details"></a>方案详细信息

A continuous production process (5) consumes the batch-controlled raw material RM-100. 物料是牌照 PL-1 上的库位 Bulk-001 (1) 上的现有物料，具有两个批次，B1 和 B2，数量均为 100 磅。 仓库工作 (2) 为 RM-100 进行发布和处理，且物料从 Bulk-001 领取到被定义为非牌照控制的生产输入库位 PIL-01 (3)。 机器操作员从生产输入库位 (3) 称出物料并将重量和批处理号登记为已使用 (4)。 从生产输入库位，部分物料在定义的时间间隔内被手动添加到生产流程。 在机器操作员添加物料时，物料在秤上称重，并登记批号。

## <a name="set-up-theworkflow-to-register-consumption-using-a-handheld-device"></a>Set up the workflow to register consumption using a handheld device
Create a finished-good product, FG-100, with a bill of material that has the batch-controlled raw material RM-100. Add two batches, B1 and B2, of RM-100 in a quantity of 100 to location: Bulk-001 on license plate: PL-1. RM-100 在物料清单行上的耗用原则设置为**手动**。 Set  the production input location to PIL-01. 为此，您可以选择此库位作为仓库 51 上的默认生产输入库位。

1.  创建新的移动设备菜单项： 

-    **Menu item name** - Register material consumption. 
-    **标题** - 登记物料消耗量。 
-    **模式** - 间接。 
-    **Activity code** - Register material consumption.

2.  Add the menu item to the **Production Mobile** device menu.
3.  创建成品的生产订单： 

-    **Item number** - FG-100 
-    **Site** - 5 
-    **Warehouse** - 51 
-    **Quantity** - 150

生产订单为**估计**和**已发布**，并创建仓库工作。

4.  使用用于手持设备的原材料领料工作流完成工作。

这将把物料从堆放库位移到生产输入库位 PIL-01。 After the work is completed, the material has the status **Picked on the production input location**. 工作处理后的状态可能为**已领料**或**实际预留**。 这使用参数**置于仓库后的发货状态窗体**进行配置。

5.  使用**生产开始**菜单项从客户端或从手持设备开始生产订单。

在开始执行生产订单后，您可以使用用于手持设备的工作流登记物料消耗量。 Let's start by registering consumption of 25 lbs of batch B1.

6.  Select the **Register material** **consumption** menu item in the menu for the hand held device, enter the following details: 

-    生产订单编号。 
-    要消耗物料的库位，在此例中为 PIL-01。 
-    物料编号 RM-100。 
-    批处理号 B1。 
-    A quantity of 25.

7.  选择**确定**。

Note that the message "Journal line is created" appears on the display. 在生产订单上有一个针对物料编号 RM-100 和批处理号 B1 的**生产领料单**类型的未结日记帐。 

您现在可以选择继续登记，例如在批处理号 B2 上，且每一次选择**确定**，都会在未结日记帐上添加新的日记帐行。 

After you have finished your registration, select **Done** to post the journal and end the workflow.

### <a name="additional-comments"></a>其他注释 

-   If a user cancels the workflow after a journal line is created, the journal is in an unposted state but if the user at a later point uses the workflow for the same production order, then the lines will be added to the open journal rather than to a new journal.
-   The new workflow also supports the registration of serial numbers.
-   只能登记在所选生产订单或批次订单的物料清单或配方中定义的物料编号。
-   物料可以过度消耗。 例如，如果物料的估计消耗数量为 100 磅，则可以过度消耗，例如数量 105 磅。


