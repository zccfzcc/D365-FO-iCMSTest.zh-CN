---
title: 使用任务录制创建文档或培训
description: 此主题介绍任务录制器和任务指南是什么，如何创建任务录制，以及如何自定义 Microsoft 任务指南和将其加入帮助中。
author: josaw1
manager: AnnBe
ms.date: 10/24/2017
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-platform
ms.technology: ''
ms.search.form: SysHelpSetup
audience: Application User, IT Pro
ms.reviewer: josaw
ms.search.scope: Core, Operations
ms.custom: 25391
ms.assetid: 59bf39f8-1464-441e-8b23-9a856c73471b
ms.search.region: Global
ms.author: josaw
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: daaa8f3c033c2285300a5c383a57b1939ed21f80
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54500"
---
# <a name="create-documentation-or-training-by-using-task-recordings"></a>使用任务录制创建文档或培训

[!include [banner](../includes/banner.md)]

此主题介绍任务录制器和任务指南是什么，如何创建任务录制，以及如何自定义 Microsoft 任务指南和将其加入帮助中。

> [!IMPORTANT]
> 您可以录制自己的 Dynamics 365 for Talent 任务指南，但暂时不能将其保存到业务流程建模器 (BPM) 库或从“帮助”窗格中打开它。 您可以将其保存到本地或网络位置，然后使用任务录制器打开并播放。 

<a name="learn-about-task-recorder"></a>了解任务录制器
-------------------------

任务录制器是一种可用来记录您在产品用户界面 (UI) 上执行的操作的工具。 当您使用任务录制器时，将捕获您在 UI 中对服务器执行的所有事件（包括添加值、更改设置、删除数据）。 您记录的步骤统称为*任务录制*。 可通过多种方式使用任务录制：

-   **任务录制可作为任务指南播放。** 任务指南是帮助体验的一个组成部分。 A task guide is a controlled, guided, interactive experience through the steps of a business process. 系统将通过弹出提示（或“气泡”）方式指示用户完成每个步骤，这将跨 UI 创建动画效果并指向用户应与之交互的 UI 元素。 The "bubble" also provides information about how to interact with the element, such as “Click here” or “In this field, enter a value.” A task guide runs against the user’s current data set and the data that is entered is saved in the user’s environment.
-   **任务录制可作为操作步骤显示在“帮助”窗格中。** 您可以使用“帮助”窗格搜索和显示任务录制。 您可以通过单击顶部导航栏中的 **?** 图标访问“帮助”窗格， 也可以使用快捷键组合  **Ctrl+Shift+?**。 您可以阅读“帮助”窗格中的任务录制步骤，也可以选择以任务指南方式播放录制以便其指导您完成 UI。
-   **任务录制可保存到 BPM。** You can save your task recording to a line of a hierarchy in a BPM library in Lifecycle Services (LCS). 将从录制中生成一个步骤列表和一个业务流程图表。 已保存到 BPM 库中的任务录制可显示为帮助。
-   **任务录制可另存为 Word 文档。** 这将允许您轻松地生成可打印的培训指南。

您可以创建自己的任务录制、播放 Microsoft 提供的任务录制或修改 Microsoft 提供的任务录制以反映您的配置。 For more information about Task recorder, see [Task recorder](task-recorder.md).

## <a name="plan-your-task-recording"></a>计划您的任务录制
无论您要创建新的任务录制还是基于 Microsoft 任务录制创建您的录制，请记住以下信息。

-   计划您的录制，就像计划视频一样。 提前制定您的所有决策。
-   在不录制业务流程的情况下演练业务流程一次或两次以了解步骤。
-   当您在录制前演练业务流程时，记下使用快捷键或 **Enter** 键的位置，以避免在实际录制期间使用它们。
-   确定以下内容：
    -   是否要将步骤分成多个子任务？ 子任务以直观方式使流程的各个部分分离。 例如，如果您为“创建和发布产品”创建录制，则可能需要将创建产品所需的步骤组合在一起，然后将发布产品所需的步骤组合在一起。 子任务还使得较长的流程更易读取。
    -   是否要添加批注，如果添加，该添加在何处？ 请参阅下面的“了解不同类型的批注”以了解更多信息。
    -   在您完成业务流程的步骤时，将在各个字段中添加什么值？ 最好是了解在您继续时将选择或输入的内容，以便您在录制时不会追踪或修复错误。

**提前编写描述和批注**

-   在每个任务录制开始时，将显示一个描述字段，该字段允许您输入对录制的介绍。 最好是提前在一个单独的文档中编写并保存描述，以便在录制时将其复制并粘贴到任务录制中。 这样一来，当您未处于录制过程中时，可花时间精炼文本。 剪切并粘贴文本将使录制流程变得更快且更平稳。
-   对于任务录制中的每个步骤，您可以创建批注。 播放任务指南期间，批注作为注释显示在步骤文本的上方或下方的“气泡”中。 When viewed as text in the Help pane, annotations appear as text inline in the step. 正如描述一样，最好是在一个单独的文档中编写和保存您的批注。 当您录制任务录制时，从该文档中剪切并粘贴批注。

**了解不同类型的批注** 所有批注均可选。 仅在批注向用户提供有用信息时添加批注。

-   **标题：** 标题批注将显示在任务录制器自动生成的步骤文本的前面。 In the task guide, the title annotation appears above the automatically generated text. 使用这种类型的批注可说明用户执行步骤的原因或提供附加上下文。

这是您在创建录制的同时添加批注时显示的编辑窗格。 在**标题**框中输入标题注释。 

[![屏幕 1](./media/screen1.png)](./media/screen1.png) 

这是标题注释在任务指南中的“气泡”中的样子。 

[![屏幕 2](./media/screen2.png)](./media/screen2.png)

-   **注意：** 注释批注将显示在任务录制器自动生成的步骤文本的后面。 在任务指南中，批注仅在用户单击任务指南气泡中的**显示更多**链接时可见。 使用此类批注可描述用户完成步骤所需了解的所有内容。

这是您在创建录制的同时添加批注时显示的编辑窗格。 在**附注**框中输入标题注释。 

[![屏幕 3](./media/screen3.png)](./media/screen3.png) 

这是附注注释在任务指南中的“气泡”中的样子。

[![屏幕 4](./media/screen4.png)](./media/screen4.png)

-   **Info step**: These annotations are created by right clicking on a control or anywhere on a form &lt; **Task recorder** &lt; **Add info step. **Info steps appear as a numbered step at whatever point you insert it, even though no action was recorded in the UI. 您可以添加窗体级别信息步骤或与控件关联的信息步骤。 当信息步骤与窗体关联时，任务指南“气泡”将在播放任务指南时显示在窗体的某个位置（无指针）。 当信息步骤与控件关联时，任务指南“气泡”将在播放任务指南时指向控件。 In the Help pane, an info step annotation will appear as a numbered step with whatever text you entered. 使用信息步骤可准备用户以执行后续步骤、描述需在 Microsoft Dynamics 365 for Finance and Operations 外部完成的步骤或引用其他录制（尽管您无法在批注中创建超链接）。

**确定创建录制所需的时长**

-   通常，用户将自始至终读取或播放录制，因此不要组合更适合单独执行的步骤或任务。
-   尽量不要录制跨多个子流程的长方案。 例如，“在商店内客户服务台运行”太广泛，将它拆分为多个小型任务，如“接收退货”和“添加到礼品卡”。
-   如果某个任务可作为多个不同的业务流程的一部分执行，请为它创建一个单独的录制，这样您就可以在其他录制中引用它。
-   如果该流程涉及人员可能马上全部完成的多个任务，您可以将这些任务保留在一个录制中，例如“设置和分配功能配置文件”。
-   如果人员可一次性完成某个任务（如配置），然后完成可随后立即执行但可能重复执行的另一任务，则将这些任务拆分为两个任务录制。

**决定在 UI 中开始录制的位置** 您在开始录制任务录制时所在的页面会影响为其显示任务指南的页面。 For example, if you want your task recording to be listed in the Help pane when a user clicks Help on the General ledger parameters page, you must start your recording on the General ledger parameters page. **将录制另存为 .axtr 文件** 当您创建或编辑完任务录制时，系统将为您显示有关如何下载或保存录制的多个选项。 您可以将文件作为任务录制包 (.axtr)、原始录制文件 (.xml) 或 Word 文档下载或将文件保存到 LCS 库。 最好是始终将您的任务录制另存为任务录制包文件 (.axtr)。 如果稍后需要更改过程或批注，这将帮助更轻松地维护文件。 如果您需要将文件作为 Word 文档下载，也将其另存为任务录制包文件。

## <a name="create-your-task-recording"></a>创建您的任务录制
For detailed walk-through steps, see [How to create a task recording](task-recorder.md).

## <a name="copy-and-customize-microsofts-task-recordings"></a>复制和自定义 Microsoft 的任务录制
您可以下载和编辑 Microsoft 的任务录制以将其用于您自己的帮助文档或培训材料。 要下载 Microsoft 任务录制，请执行以下步骤：

1.  打开任务录制器。 任务录制器位于**设置**菜单中。
2.  在任务录制器窗格中，单击**维护录制**。
3.  在**录制位于何处**下，单击**它在 LCS 库中**。
4.  单击**选择 LCS 库**。
5.  选择 Microsoft 全局库。
6.  在树中，选择与任务录制关联的业务流程库节点。
7.  单击**OK**。
8.  单击**开始**。
9.  At this point, step through the recording, changing any steps as you go to re-record it. **Note**: If you only need to change the text of a recording, you can open the recording in **Edit a recording's annotations** mode, and then save it.
10. 在播放完录制后，单击屏幕顶部的任务录制器栏中的**停止**。
11. 选择您希望用来保存任务录制的方式。

## <a name="include-your-task-recordings-in-the-help-pane"></a>将您的任务录制包含在“帮助”窗格中
要在“帮助”窗格中显示您自己的自定义任务录制以便它们可作为任务指南播放或作为文本查看，您必须将任务录制保存到自己的 BPM 库，然后更新帮助系统参数以指向您的 BPM 库。 有关更多信息，请参阅[连接帮助系统](../../fin-and-ops/get-started/help-connect.md)。

<a name="additional-resources"></a>其他资源
--------

[帮助概览](../../fin-and-ops/get-started/help-overview.md)

[连接帮助](../../fin-and-ops/get-started/help-connect.md)

[任务录制器](task-recorder.md)

[使用任务录制器创建丰富的帮助主题（外部链接）](https://mbspartner.microsoft.com/AX/Videos/970)
