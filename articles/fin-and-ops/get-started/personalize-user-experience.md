---
title: 打造个性化的用户体验
description: 本主题说明如何个性化 Microsoft Dynamics 365 for Finance and Operations。
author: TLeforMicrosoft
manager: AnnBe
ms.date: 09/28/2018
ms.topic: article
ms.prod: ''
ms.service: dynamics-ax-applications
ms.technology: ''
ms.search.form: SysUserSetup, DefaultDashboard
audience: Application User, IT Pro
ms.reviewer: sericks
ms.search.scope: Core, Operations
ms.custom: 62363
ms.assetid: 57b445d7-3e9e-4228-8728-f63b9dbd77a3
ms.search.region: Global
ms.author: tlefor
ms.search.validFrom: 2016-02-28
ms.dyn365.ops.version: AX 7.0.0
ms.openlocfilehash: feae12df709fcc5e39006d7689ea110494de2208
ms.sourcegitcommit: 73e10192fb6318dee5bb1129591120199de6a487
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "54725"
---
# <a name="personalize-the-user-experience"></a>打造个性化的用户体验

[!include [banner](../includes/banner.md)]

本主题说明如何个性化 Microsoft Dynamics 365 for Finance and Operations。

Finance and Operations. 中有三类基本的个性化设置。 
- 设置页执行的个性化设置。 例如，主题颜色和时区。
- 与页面使用情况有关的个性化设置，称为*隐式*个性化设置。 例如，Finance and Operations 跟踪网格列的宽度（如果您调节它们）或快速选项卡的展开/折叠状态。 
- 用户为了修改页面的外观通过更改元素在页面中的显示方式或操作方式执行的个性化设置，通常是通过交互式个性化模式进行的。 此类个性化设置称为*显式*个性化设置。 例如，用户可以在页面中添加、隐藏元素或为元素重新排序。

用户在 Finance and Operations 中所进行的每项个性化设置都仅针对该用户，与个性化类型或用户当前交互的公司无关。 一位用户对页面所做的更改不会影响系统中的其他用户。

## <a name="system-wide-options-for-the-current-user"></a>当前用户的系统范围选项
**用户选项**页中包含若干针对当前用户的系统级设置。 若要打开**用户选项**页，请选择导航栏上的**设置**菜单（齿轮符号），然后选择**用户选项**。 **用户选项**页有四个选项卡，其中包含各项用户设置：

- **可视化** - 用于选择颜色主题和页面上的元素的默认尺寸。
- **首选项** – 用于选择每次打开 Finance and Operations 时使用的默认值。 这些值包括公司、初始页和默认查看/编辑模式。 （查看/编辑模式确定页面在每次打开时为锁定供查看，还是打开供编辑。）此选项卡中还有语言，时区及日期、时间和数字格式选项。 最后，此选项卡中包含若干杂项首选项，具体由版本决定。
- **帐户** – 用于调整用户名和其他与帐户有关的选项。
- **工作流** – 用于选择与工作流有关的选项。

## <a name="implicit-personalizations"></a>隐式个性化设置
隐式个性化设置是只需通过与“记得”其当前可视化状态的控件互动即可执行的个性化设置。

- **网格列** - 您可以选中列标题左侧或右侧的大小调整列，然后将其向左或向右滑动到所需列宽，从而调整网格中列的宽度。 Finance and Operations 将存储您为列设置的宽度。 然后每次打开包含该网格的页时，都将把该列调整为此宽度。
- **快速选项卡** – 某些页面具有可扩展的分区，称为*快速选项卡*。 Finance and Operations 将存储有关您已展开和折叠的快速选项卡的信息。 然后，每次您回到此页时，都将根据您上次与此页的交互展开或折叠相同快速选项卡。 在某些情况下，可以通过折叠某个快速选项卡帮助提高性能，因为在该快速选项卡被展开之前，Finance and Operations 不必检索有关该快速选项卡的信息。 本主题后文将说明，您也可以更改页面上的快速选项卡顺序。
- **速见表**  – 某些页面有一个称为*速见表窗格*的部分。 此窗格包含与该页面的当前主题相关的只读信息。 速见表窗格中的每个部分称为一个*速见表*。 可以隐藏或显示整个速见表窗格，也可以展开或折叠单个速见表。 Finance and Operations 将存储您的首选项。 然后，每次回到该页时，都将根据您上次与该页的交互还原速见表窗格和单个速见表的状态。 在某些情况下，可以通过折叠某个速见表帮助提高性能，因为在该速见表被展开之前，Finance and Operations 不必检索有关该速见表的信息。
- **操作窗格** – 大多数页面顶部会显示一个*操作窗格*。 操作窗格中包含可在当前页面中执行的大量操作的按钮。 这些按钮通常组织在选项卡上。 可固定打开整个操作窗格，也可以默认折叠。 然后，下次打开该页时，Finance and Operations 将还原操作窗格的固定状态。 如果操作窗格已固定打开，Finance and Operations 还将显示您上次使用的操作的选项卡。
- **快速筛选器** – 许多网格上方会显示*快速筛选器*。 快速筛选器根据您选择的列筛选网格。 Finance and Operations 将存储您筛选的列。 然后，下次打开包含该网格的页面时，将对同一列筛选该网格。 但是，可以对其他列筛选该网格。
- **列标题筛选器** – 使用*列标题筛选器*筛选网格时，可根据需要更改筛选器运算符，以便查找所需数据。 例如，可以将运算符从**开头为**更改为**正好是**。 每次使用列标题筛选器并修改筛选器运算符时，Finance and Operations 都将存储更改。 下次对该列进行筛选时，将还原筛选器运算符。
- **导航窗格** – 可通过选择任何页面左窗格中的**菜单**按钮打开*导航窗格*。 （**菜单**按钮有时称为*汉堡包*、*汉堡包菜单*或*汉堡包按钮*。）可将导航窗格固定打开，也可以让其默认保持折叠。 固定打开导航窗格后，Finance and Operations 将使其保持打开，直到您折叠为止。

## <a name="explicit-personalizations"></a>显式个性化设置
不同人和不同公司对哪些数据对其最重要或哪些数据对其开展业务来说不需要的认知不同。 在 Finance and Operations 中，可调整信息的排序和交互方式。 也可以指定应隐藏某些信息。 这些功能是个性化高效体验的关键，也是显式个性化设置的典范。 显式个性化设置是您为了更改元素或页面的外观或行为，显式执行的个性化设置。

### <a name="shortcut-menu-options"></a>快捷菜单选项
可通过快捷菜单使用一些方法显式更改页面，以更好地满足您或公司的需要。 （快捷菜单也称为*右键单击菜单*或*上下文菜单*。）

可对页面执行的某些最典型、最重要的更改直接以快捷菜单中的选项的形式提供。 例如，从平台更新 17 开始，如果要在网格中添加或隐藏列，只需右键单击网格列标题，然后选择**添加列**或**隐藏此列**。

此外，大多数最基本的显式个性化设置可以通过右键单击元素再选择**个性化**来执行。 （注意，并非您页面上的所有元素都能可行化。）当您使用这种个性化设置方法时，将显示元素的属性窗口。

[![个性化元素的属性](./media/personalization-element-properties.jpg)](./media/personalization-element-properties.jpg)

可使用属性窗口通过下面的方法对元素进行个性化设置：

- 更改元素的标签。
- 隐藏元素，使其不在页面中显示。 不会删除或修改字段中的数据。 不过是信息不再在页面中显示而已。
- 将信息包含在快速选项卡摘要部分中（如果元素位于快速选项卡上）。
- 按 Tab 键在页面中的字段之间切换时跳过该字段。
- 禁止编辑该字段中的数据（适用于所有记录）。

属性窗口中可能包含其他个性化设置功能，具体取决于元素。 例如，磁贴的属性窗口可能允许您将该磁贴升级为仪表板，而仪表板的属性窗口可能允许您在该仪表板中新建工作区。

### <a name="the-personalization-toolbar"></a>个性化设置工具栏
如果要对页面进行多项更改或要进行的更改不能通过其他机制（如为元素进行重新排序）进行，则可使用**个性化设置**工具栏。 若要打开**个性化设置**工具栏，请在元素的属性窗口中选择**个性化设置此窗体**。 也可以在各页面的操作窗格的**选项**选项卡上**个性化**组中选择**个性化设置此窗体**。

[![个性化设置工具栏](./media/personalization-personalizationtoolbar.jpg)](./media/personalization-personalizationtoolbar.jpg)

#### <a name="navigating-the-page"></a>导航页面 
**个性化设置工具栏**打开后是否可导航页面取决于运行的平台版本。 

- 在平台更新 19 之前的版本中，**个性化设置**工具栏打开后，页面为只读（不能输入任何内容）且不可交互（只能对页面中的可视元素进行更改）。 如果要对折叠部分中的元素或其他选项卡上的元素进行更改，需要关闭**个性化设置**工具栏，展开部分或切换到所需选项卡，然后重新打开**个性化设置**工具栏。  

- 从平台更新 19 开始，如果**个性化设置**工具栏已打开，页面仍然为只读，但是交互性更高。 特别是，可以在**个性化设置**工具栏处于打开状态时展开或折叠速见表窗格，切换选项卡和展开或折叠部分，就像通常在页面中进行导航一样。 要对可折叠部分或选项卡应用个性化设置更高（如隐藏速见表），请在可折叠部分或选项卡获得了键盘焦点或您将光标悬停在其上方时，触发该部门或选项卡旁边显示的按钮。  

#### <a name="personalization-tools"></a>个性化设置工具
**个性化设置**工具栏上提供了以下工具：

- 可使用**选择**工具选择和更改元素的属性。 选择**选择**工具，然后选择要修改其属性的元素。 如果您选择了某个元素，将显示该元素的属性窗口，您可以修改该元素的任意属性。 您可以对该页中可个性化设置的其他元素重复此流程。 但是，由于某些元素的使用方式的原因，Finance and Operations 不允许更改这些元素的一些属性。 因此，选择元素时，可能会发现不能更改该元素的某些属性。 例如，不能隐藏必填字段。

- 可使用**移动**工具将元素移动到当前元素组中的其他位置。 （不能将元素移到其父组之外）。 选择**移动**工具，然后选择要移动的元素。 在您选择元素后，Finance and Operations 将扫描页面以确定可将该元素移到哪里。 然后创建一组“拖放区域”。 当您在当前组内拖动元素时，每个“拖放区域”在可放置该元素的区域旁边显示为彩色粗线。

- 可使用**隐藏**工具在页面中隐藏元素。 选择**隐藏**工具，然后选择要隐藏的元素。 如果选择**隐藏**工具，当前隐藏的所有元素都将可视并在阴影容器中显示。 然后可取消隐藏这些元素。 通过选择**选择**工具，可查看隐藏所选元素后页面的外观。
    - 从平台更新 18 开始，可隐藏必填字段和包含必填字段的部分。 这样就可以通过不显示缺省采用业务逻辑提供的值的字段来简化体验。 如果保存时隐藏的必填字段为空，也可以暂时将其显示。 

- 如果希望某个元素在快速选项卡摘要部分中显示，可使用**摘要**工具。 “摘要”工具将仅适用于快速选项卡部分中的字段。 如果选择**摘要**工具，已作为摘要字段选择的所有字段都将在阴影容器中显示。 可以通过选择字段以交互方式将其添加到快速选项卡摘要中，也可以通过这种方法将其从快速选项卡摘要中移除。

- 可使用**跳过**工具从页面的键盘 Tab 序列中删除元素。 如果选择**跳过**工具，当前跳过的所有元素都将在阴影容器中显示。 然后可将其重新添加到 Tab 序列中。

- 可使用**编辑**根据将元素标记为可编辑或不可编辑。 如果选择**编辑**工具，当前不可编辑的所有元素都将在阴影容器中显示。 然后可将其重新设置为可编辑。 请注意，某些字段是必填字段，不能设置为不可编辑。 这些字段旁边将显示一个挂锁符号。

- 可使用**插入**按钮查看页面上可插入元素的列表。
    - 可选择**插入**下的**字段** 工具向页面添加字段。 使用**字段**工具时，只能添加页面定义中包含，但页面中当前不显示的字段。 有关如何新建当前页面定义中不包含的字段的信息，请参阅[自定义字段](user-defined-fields.md)。 选择**字段**工具之后，首先必须选择要在其中添加字段的组或区域。 一个对话框显示与所选组或区域相关的字段的列表。 在该对话框中，选择一个或多个要添加的字段，然后选择**插入**。 若要删除以前添加的字段，请重复该过程，但在对话框中清除选择字段。
    - 选择**插入**下的 **PowerApp** 工具可将通过使用 Microsoft PowerApps 创建的应用程序插入页面中。 有关如何将 PowerApps 应用程序嵌入页面中的详细信息，请参阅[嵌入 PowerApps](embed-power-apps.md)。

- 选择**管理**按钮可查看与当前页面的所有个性化设置相关的管理选项的列表。
    - 选择**清除**可将页面重置为其默认安装状态。 将清除当前页面上的所有个性化设置。 此操作不可撤消。 因此，仅当确信要重置页面，才使用此选项。
    - 选择**导入**可从您或其他人之前为此页面创建的文件加载个性化设置。 将把您对该页面执行的所有当前个性化设置替换为所选文件中的个性化设置。
    - 可选择**导出**将页面的个性化设置保存到文件。 可将个性化设置与其他用户共享。 这些用户只需导入包含您对页面执行的个性化设置的文件。

- 选择**关闭**按钮可关闭**个性化设置**工具栏并使页面恢复为之前的交互式状态。

如果使用**个性化设置**工具栏，则保存操作隐式执行。 个性化设置将在执行后立即生效，您不需要选择**保存**按钮。 在某些情况下，选择工具后时，元素旁边将显示一个挂锁符号。 此符号指示您不能修改与所选工具有关的元素属性，因为更改这些属性将导致页面异常工作。

### <a name="adding-a-tile-list-or-link-to-a-workspace"></a>向工作区添加磁贴、列表或链接
对于某些包含列表的页面，还有一项个性化设置功能。 可通过操作窗格**选项**选项卡上**个性化设置**组中的**添加到工作区**按钮在特定工作区中显示当前列表内的信息。 可在该工作区中显示经过筛选和排序的信息视图，也可以显示默认视图。 还可以指定信息在工作区中显示为列表、可显示列表中的项数的汇总磁贴还是链接。

[![添加到工作区](./media/personalization-addtoworkspace.png)](./media/personalization-addtoworkspace.png)

- 若要向工作区添加列表，请首先在页面中对列表排序或筛选，以便将信息按照您希望在工作区中显示的方式显示。 然后选择 **添加到工作区**。 选择一个工作区，然后在**展示**字段中选择**列表**。 选择**配置**之后，将显示一个对话框，可在其中选择应在工作区中的列表内显示的列。 还可以指定要用于工作区中的列表的标签。
- 若要向工作区添加磁贴，首先请在页面中对列表进行筛选，使其显示要汇总或快速访问的数据。 然后选择 **添加到工作区**。 选择一个工作区，然后在**展示**字段中选择**磁贴**。 选择**配置**之后，将显示一个对话框，可在其中指定要在工作区中用于磁贴的标签。 也可以指定磁贴是否应显示计数。 将磁贴添加到工作区之后，可选择该磁贴以从工作区打开当前页面，然后查看与该磁贴关联且经过筛选的列表。
- 若要向工作区添加链接，请首先在页面中筛选列表，以使其显示您感兴趣的数据。 然后选择 **添加到工作区**。 选择一个工作区，然后在**展示**字段中选择**链接**。 选择**配置**之后，将显示一个对话框，可在其中指定要用于链接的标签。 也可以选择为将包含此链接的新部分指定标签。

列表、磁贴或链接添加到工作区之后，可打开该工作区并按照您的意愿在其中显示元素。

### <a name="adding-a-summary-from-a-workspace-to-a-dashboard"></a>将摘要从工作区添加到仪表板
某些工作区中包含计数磁贴（即磁贴上有数字），您可能希望在仪表板中也显示这些磁贴。 在工作区中，右键单击计数磁贴，然后选择**个性化**。 然后在磁贴的属性窗口中选择**固定到仪表板**。 下次打开（和刷新）所选仪表板时，将在该工作区的导航磁贴下方显示计数。 可选择该计数以直接转到其表示的数据。

### <a name="personalizing-your-dashboard"></a>个性化设置仪表板
通常，仪表板是您打开 Finance and Operations 时看到的第一页。 可个性化设置仪表板，使其仅显示要查看的工作区磁贴。 也可以重新排列磁贴以使其按照您喜爱的查看顺序排列，重命名工作区导航磁贴，或添加全新的工作区磁贴。

若要个性化设置仪表板，请右键单击任何磁贴，然后选择**个性化**以打开磁贴的属性窗口。

- 如果要隐藏或重命名所选磁贴，可直接在属性窗口中进行相应更改。
- 若要为工作区磁贴重新排序，请在属性窗口中选择**个性化设置此窗体**以打开**个性化设置**工具栏。 然后，您可以使用**移动**工具按照自己的意愿来排列磁贴。
- 若要新建工作区磁贴，请在属性窗口中选择**添加工作区**。 将在仪表板底部创建一个新工作区。 可按照您的意愿为这个新工作区命名。 也可以按照本主题中的[向工作区添加列表、磁贴或链接](personalize-user-experience.md#adding-a-tile-list-or-link-to-a-workspace)部分中的介绍向工作区添加列表、磁贴或链接。

## <a name="administration-of-personalization"></a>管理个性化设置
在页面个性化后，可以通过导出个性化的页面与其他用户共享您的个性化设置。 然后可以请其他用户打开个性化的页面并导入您创建的个性化文件。 也可以将您的个性化设置提供给具有管理员权限的用户。 然后，该用户可将您的个性化设置文件同时应用于大量用户。

具有管理员权限的用户也可以在**个性化设置**页面中为其他用户管理个性化设置。 此页有四个选项卡：

- **应用** –您可以导入或选择一个或多个用户的个性化设置。 若要将个性化设置应用于一位或多位用户，请首先选择一个角色和具有该角色的用户。 然后选择要为所选用户应用的现有个性化设置，或导入个性化设置文件。 将验证该个性化设置，并在所选用户下一次打开所选页面时应用。
- **清除** – 您可以清除一个或多个用户的页面或工作区的所有个性化设置。 首先访问页面或工作区以查看已对其执行了个性化设置的用户的列表。 然后，选择应该清除该页面或工作区的个性化设置的用户，再选择**清除**。 将删除所选用户已应用于所选页面或工作区的所有个性化设置。 此操作无法撤消。 但是，如果为页面或工作区保存了个性化设置，则可以重新导入该个性化设置。
- **按用户管理** – 选择一个用户查看其已个性化的页面的列表。 随后您可以选择启用或禁用所选用户为特定页面或为整个系统使用个性化设置的权限。 您还可以导入、导出或清除所选用户的个性化设置。
- **系统** - 您可以在此临时禁用系统中所有用户的全部个性化设置。 在这种情况下，将删除个性化设置。 所有页面仅重置为针对全部用户的默认状态。 如果您在以后重新启用个性化设置，所有个性化设置将重新应用。 您还可以永久删除系统中所有用户的全部个性化设置。 不能恢复已删除的个性化设置。 因此，在执行此任务之前，请务必导出以后可能需要的任何个性化设置。

## <a name="personalization-of-inventory-dimensions"></a>库存维度的个性化

个性化页面中的库存维度设置时，请注意已通过使用**显示维度**选项创建的设置。 例如，您使用个性化设置隐藏批次编号库存维度的一个列，但下次打开该页时显示这列。 发生此行为是因为**维度显示**设置控制显示的库存维度列。

**维度显示**设置应用于所有页，并覆盖单个页中的库存维度字段的所有个性化设置。

因此，在前面的示例中，如果不希望批次编号库存维度的列显示，必须在表的**显示维度**选项中清除该维度。 此项更改最终不仅在一个特定页上应用，还将在所有页中应用。
