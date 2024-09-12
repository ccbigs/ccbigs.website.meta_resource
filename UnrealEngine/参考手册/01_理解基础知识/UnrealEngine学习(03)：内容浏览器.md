# UnrealEngine学习(03)：内容浏览器

**内容浏览器（Content Browser）** 是虚幻编辑器的主要区域，用于在虚幻项目中创建、导入、整理、查看和修改内容资产。你还可以使用它管理内容文件夹，并执行专有资产操作，例如：

- 前往浏览项目中的所有资产并与之交互。
- 使用文本筛选器查找资产，你可以选择将其与更高级的筛选功能结合使用。
- 将资产整理到私有、本地或共享集合中。
- 识别可能存在问题的资产。
- 在内容文件夹之间迁移资产，或迁移到不同的项目。

要了解有关每项操作的更多信息，请参阅此页面上的内容浏览器主题（Content Browser Topics）小节。

**访问内容浏览器：**

1. 使用顶部菜单栏中的 **窗口（Window）** 菜单。![image-20240827075146643](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\image-20240827075146643.png)

2. 使用主工具栏（Main Toolbar）上的 **创建（Create）** 菜单。

   ![image-20240827075208506](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\image-20240827075208506.png)

3. 点击编辑器底部工具栏上的 **内容侧滑菜单（Content Drawer）** 按钮。这会打开临时的内容浏览器（Content Browser），然后你可以停靠到编辑器窗口。要了解更多信息，请参阅此页面上的内容侧滑菜单（Content Drawer）小节。![image-20240827075223598](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\image-20240827075223598.png)

你可以同时打开最多四个内容浏览器实例。例如，如果你要执行以下操作，这很有用：

- 在不同的内容浏览器（Content Browser）中筛选不同的资产类型，例如一个只显示静态网格体，另一个只显示材质。
- 在项目的不同文件夹之间迁移资产。

默认情况下， **内容浏览器（Content Browser）** 停放在虚幻编辑器（Unreal Editor）窗口的底部。你可以点击并拖动，将其重新停靠在编辑器中的任何位置，或使其成为浮动窗口。你还可以右键点击内容浏览器（Content Browser）选项卡，并选择 **移至侧边栏（Move to Sidebar）** ，这样内容浏览器（Content Browser）会折叠到虚幻编辑器（Unreal Editor）窗口左侧边栏中的可点击选项卡。

---

**内容侧滑菜单：**

**内容侧滑菜单（Content Drawer）** 是内容浏览器的特殊实例，其行为略有不同。要打开它，请执行以下任一操作：

- 点击编辑器底部栏上的 **内容侧滑菜单（Content Drawer）** 按钮。
- 使用键盘快捷键 **Ctrl + 空格键（Ctrl + Space Bar）** （Windows）或 **Cmd + 空格键（Cmd + Space Bar）**（macOS）。

内容侧滑菜单（Content Drawer）在失焦（即，当你点击离开它时）时会自动最小化。要使其保持打开状态，请点击 **停靠在布局中（Dock in Layout）** 按钮。这会创建内容浏览器的新实例，但你仍然可以打开新的内容侧滑菜单（Content Drawer）。

![image-20240827075611199](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\image-20240827075611199.png)



## 1.内容浏览器界面

**内容浏览器（Content Browser）** 分为以下几个区域：
![Areas of the Content Browser window](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\ue5_1-content-browser-areas.png)

| **编号** | **名称**                    |
| -------- | --------------------------- |
| 1        | 导航栏（Navigation Bar）    |
| 2        | 源面板（Sources Panel）     |
| 3        | 集合（Collections）         |
| 4        | 筛选器（Filters）           |
| 5        | 搜索栏（Search Bar）        |
| 6        | 资产视图（Asset View）      |
| 7        | 设置按钮（Settings Button） |

### 1.01.导航栏

**导航栏（Navigation Bar）** 包含用于处理资产、在文件夹路径之间来回浏览的功能按钮，并显示当前打开的文件夹浏览记录路径。![image-20240827080220323](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\image-20240827080220323.png)

![内容浏览器中的导航栏](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\content-browser-navigation-bar.png)

| **编号** | **名称**                                                     | **说明**                                                     |
| -------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| 1        | **资产控制按钮（Asset Control Buttons）**                    | 这些按钮具有以下功能：**添加（Add）** ：点击此按钮，可以将现有资产添加到你的项目或创建新资产。**导入（Import）** ：点击此按钮，可以打开文件浏览器，并选择一个或多个资产，添加到你的项目中。**保存全部（Save All）** ：点击此按钮，保存未保存更改的全部资产。要了解有关将资产导入项目的更多信息，请参阅[直接导入资产](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/importing-assets-directly-into-unreal-engine)页面。 |
| 2        | **历史记录后退和前进按钮（History Back and Forward Buttons）** | 这些按钮的功能类似于Web浏览器中的后退（Back）和前进（Forward）按钮。使用它们在最近的文件路径之间来回浏览。 |
| 3        | **浏览记录路径（Breadcrumb Trail Path）**                    | 此分段显示当前文件夹路径。点击任何文件夹，快速找到它。       |

### 1.02.源面板

**源（Sources）** 面板包含虚幻引擎项目中所有文件夹的列表。

![内容浏览器中的源面板](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\content-browser-sources-panel.png)

| **编号** | **名称**                          | **说明**                                                     |
| -------- | --------------------------------- | ------------------------------------------------------------ |
| 1        | **收藏夹面板（Favorites Panel）** | 此面板包含对你已添加到收藏夹中的资产的引用。                 |
| 2        | **项目名称（Project Name）**      | 这是当前打开项目的名称。点击项目名称旁边的箭头，可以折叠或展开文件夹列表。 |
| 3        | **搜索按钮（Search Buttons）**    | 点击此按钮可以打开搜索（Search）栏，使用该栏通过输入搜索条件，你可以缩小按钮关联面板中可用文件夹的列表范围。文件夹将被实时过滤，以将名字缩小至仅包括你所输入字符名称的文件夹。 |
| 4        | **资产树（Asset Tree）**          | 此层级列表显示了你的虚幻引擎项目中的所有文件夹。它的行为与Windows浏览器中的文件夹树或macOS中的访达（Finder）相同。要展开或折叠文件夹，请点击其名称旁边的箭头。在搜索文本前加上连字符（-），你可以从资产树中排除文件夹。例如，在搜索框中输入-anim会隐藏名称包含该字符串的任何文件夹，例如Animation或Animator。 |

有关源（Sources）面板的更多信息，请参阅[源面板参考](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/sources-panel-reference-in-unreal-engine)页面。

### 1.03.集合

**集合（Collections）** 面板显示你有权访问的所有集合（Collections）的列表。

![内容浏览器中的源面板](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\content-browser-collections.png)

| **编号** | **名称**                                      | **说明**                                                     |
| -------- | --------------------------------------------- | ------------------------------------------------------------ |
| 1        | **折叠/展开按钮（Collapse / Expand Button）** | 点击此按钮可以折叠或展开集合（Collections）区域。            |
| 2        | **添加集合按钮（Add Collections Button）**    | 点击此按钮可以创建新集合。                                   |
| 3        | **搜索按钮（Search Buttons）**                | 点击此按钮可打开搜索（Search）栏，使用该栏输入搜索条件，你可以缩小可用集合列表的范围。集合将被实时过滤，以将名字缩小至仅包括你所输入字符名称的集合。 |
| 4        | **集合列表（Collections List）**              | 此项目中所有集合按字母顺序排列的列表。                       |
| 5        | **资产计数（Asset Count）**                   | 显示每个集合中的资产数量。                                   |

有关集合及其用法的更多信息，请参阅[筛选器和集合](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/filters-and-collections-in-unreal-engine)页面。

### 1.04.筛选器

**筛选器（Search and Filters）** 栏提供了广泛的功能，可根据资产的名称和类型快速找到资产。**资产视图（Asset View）** 显示你在 **源（Sources）** 面板中选择的文件夹的内容，根据你在此处输入的参数动态更新。

![Filters column in the Content Browser](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\ue5_1-content-browser-filters.png)

关于筛选设置的更多信息，请参考[筛选和集合](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/filters-and-collections-in-unreal-engine)页面。

### 1.05.搜索栏

**搜索** 栏提供了许多功能，允许你根据名称和类型定位资产。**资产查看器（Asset View）** 会根据你在 **源** 面板中选中的目录来显示内容，并根据你输入如的参数动态更新。

![Search bar in the Content Browser](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\ue5_1-search-and-filters.png)

| **编号** | **名称**                                       | **说明**                                                     |
| -------- | ---------------------------------------------- | ------------------------------------------------------------ |
| 1        | **筛选器按钮（Filters Button）**               | 点击此按钮，可以打开筛选器（Filters）菜单，你可以使用该菜单自定义资产视图（Asset View）中显示的资产种类。有关使用筛选器的更多信息，请参阅[筛选器和集合](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/filters-and-collections-in-unreal-engine)页面。 |
| 2        | **搜索栏（Search Bar）**                       | 使用搜索栏按名称搜索资产。资产将被实时过滤，以将名字缩小至仅包括你所输入字符名称的资产。 |
| 3        | **保存搜索按钮（Save Search Button）**         | 点击此按钮可以将你当前的搜索保存为新集合。如果你要在以后再次运行相同的搜索，这将非常有用。 |
| 4        | **上一个搜索按钮（Previous Searches Button）** | Click this button to see a list of previous searches.        |

### 1.05.资产视图

**资产视图（Asset View）** 显示当前选定文件夹或集合中的所有可用资产。

在资产视图（Asset View）中，你可以：

- 将资产直接拖放到关卡中。
- 从你在资产视图（Asset View）中右键点击时打开的 **上下文菜单** ，创建和导入资产。
- 创建新文件夹。

![内容浏览器中的资产视图](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\content-browser-asset-viewer.png)

| **编号** | **名称**                    | **说明**                                                     |
| -------- | --------------------------- | ------------------------------------------------------------ |
| 1        | **视图区域（View Area）**   | 在应用所有筛选器和搜索条件后，这将显示当前选定文件夹或集合中的所有资产。 |
| 2        | **资产计数（Asset Count）** | 显示应用所有筛选器和搜索后显示资产的当前数量。               |

### 1.06.设置按钮

![内容浏览器中的设置按钮](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\content-browser-settings-button.png)

此按钮可以打开 **设置（Settings）** 菜单，你可以在其中调整内容浏览器的以下设置：

- 视图类型（资产的显示方式：图块、列表或列）。
- 搜索筛选器。
- 要包含或排除的内容。
- 搜索选项。



## 2.开发者文件夹

​	在 **内容浏览器（Content Browser）** 的 **开发者（Developers）** 文件夹中，可复制和处理资产，不必担心破坏项目中的内容。使用"开发者（Developers）"文件夹可尝试不同的操作，包括小规模资产修改，一直到项目级重构。

​	如果你与其他开发者在共享项目中进行协作，则每个开发者都会有自己的文件夹。

​	"开发者（Developers）"文件夹使用与Windows用户名相同的名称，但不包含虚幻引擎文件夹名称中不允许使用的字符，如句点或空格。

> 由于"开发者（Developers）"文件夹旨在用作沙盒环境，因此切勿在此文件夹之外的任何位置引用此文件夹中的资产。这样做可能会导致在烘焙项目时出错或导致烘焙失败。

### 2.01.启用开发者文件夹

如果在"内容浏览器（Content Browser）"中看不到"开发者（Developers）"文件夹，请按照以下步骤启用该文件夹：

1. 在 **内容浏览器（Content Browser）** 中，单击 **设置（Settings）**。
2. 在"设置（Settings）"菜单中，启用 **显示开发者内容（Show Developer Content）** 选项。

[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\ue5_1-enable-developers-folder.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/40643333-1d6d-4a1b-a3f1-2d56e409aa7e/ue5_1-enable-developers-folder.png)

### 2.02.与其他开发者协作

如果使用[源码控制系统](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/source-control-in-unreal-engine)，则可配置虚幻引擎以查看其他开发者的文件夹中的资产。请按照以下步骤执行此操作：

[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\ue5_1-other-developers-filter.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/86513fdb-247c-451a-a25a-54de4398d5db/ue5_1-other-developers-filter.png)

1. 在 **内容浏览器（Content Browser）** 中，单击 **过滤器（Filters）** 按钮。
2. 在"过滤器（Filters）"菜单中，选择 **其他过滤器（Other Filters）> 其他开发者（Other Developers）**。

### 2.03.从烘焙版本中排除开发者文件夹

如果要确保不会意外打包已损坏或正在处理的资产，可从烘焙版本中排除"开发者（Developers）"文件夹。请按照以下步骤执行此操作：

[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\ue5_1-directories-to-never-cook.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/076f8cc7-8590-4e3e-b17d-d525dcd862d8/ue5_1-directories-to-never-cook.png)

1. 在主菜单中，转到 **编辑（Edit）> 项目设置（Project Settings）**，然后搜索 **从不烘焙的目录（Directories to never cook）** 数组。

> 可使用该分段顶部的 **搜索（Search）** 框找到此数组。

2. 单击 **添加（+）（Add (+)）** 按钮向数组中添加新项目。

3. 单击 **…** 以打开项目中的文件夹列表。

4. 单击 **开发者（Developers）** 文件夹以将其选中。



## 3.源面板参考

​	**源（Sources）** 面板位于 **内容浏览器（Content Browser）** 左侧，包含虚幻引擎项目中的所有文件夹和集合的列表。你可以对其进行自定义，以包括其他类型的资产和资产整理功能，并将其用于启动一些常用编辑器操作。

​	当你从"源"面板选择一个或多个文件夹、集合或其他类型的资产组时，**资产视图（Asset View）** 面板将显示你的选项的内容。

![内容浏览器中的](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\ue5_1-sources-panel.png)

### 3.01.切换源面板

![image-20240827081259075](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\image-20240827081259075.png)

你可以在内容浏览器右上角的 **设置（Settings）** 菜单中启用或禁用 **显示源面板（Show Sources Panel）** 选项，以打开和关闭"源"面板。这样一来，你会有更多空间在 **资产视图（Asset View）** 中处理资产。

### 3.02.添加和删除源

![image-20240827081421483](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\image-20240827081421483.png)

默认情况下， **源（Sources）** 面板一开始显示两个资产源：

- 虚幻引擎项目中所有文件夹的层级列表，分组在 **项目名称** 下。
- 当前项目资产 **集合（Collections）** 的字母顺序列表。

你还可以添加一些资产源：

| **源**                                                       | **内容**                                                     | **如何添加**                                                 |
| ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **收藏夹（Favorites）**                                      | 你通过在资产视图中右键点击并从上下文菜单选择 **添加到收藏夹（Add To Favorites）** 而标记为收藏夹的资产。 | 从 **设置（Settings）** 菜单，启用 **显示收藏夹（Show Favorites）** 选项。 |
| **C++ Classes文件夹（C++ Classes folder）**                  | 虚幻引擎中所有C++类的可浏览层级。                            | 从 **设置（Settings）** 菜单，启用 **显示C++ 类（Show C++ Classes）** 选项。 |
| **Developers文件夹（Developers folder）**                    | 可用于在多用户项目上与其他开发人员协作的文件夹。             | 从 **设置（Settings）** 菜单，启用 **显示开发人员内容（Show Developers Content）** 选项。 |
| **Engine Content文件夹（Engine Content folder）**            | 带有各种内容和功能的现有资产集合。                           | 从 **设置（Settings）** 菜单，启用 **显示引擎内容（Show Engine Content）** 选项。 |
| **特定于插件的内容文件夹（Plugin-specific content folders）** | 各种虚幻引擎插件添加的内容文件夹。                           | 从 **设置（Settings）** 菜单，启用 **显示插件内容（Show Plugin Content）** 选项。 |
| **本地化内容（Localized content）**                          | `L10N/` 文件夹中的本地化内容。                               | 从 **设置（Settings）** 菜单，启用 **显示本地化内容（Show Localized Content）** 选项。 |

### 3.03.基于源的资产显示

**资产视图（Asset View）** 显示当前所选源中的资产。你可以使用搜索和筛选器进一步控制哪些资产显示在资产视图中。

要查看来自多个文件夹的资产，你必须选择想要搜索的所有文件夹。你可以使用以下鼠标和按键组合来选择多个文件夹。

- **左键点击** 可将当前所选项替换为你点击的文件夹。
- **Shift + 左键点击** 可选择开始和结束点之间的一系列文件夹。
- **Ctrl + 左键点击** 可选择或取消选择单个文件夹。

### 3.04.右键点击上下文菜单

如果你 **右键点击**"源"面板中的文件夹，将显示以下上下文菜单。

![image-20240827081536116](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\image-20240827081536116.png)

| **选项**                                                     | **说明**                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| **新建文件夹（New Folder）**                                 | 创建新文件夹作为当前所选文件夹的子文件夹。                   |
| **在新内容浏览器中显示（Show in New Content Browser）**      | 在新的"内容浏览器"窗口中打开此文件夹。 你可以同时打开最多四个内容浏览器实例，不包括内容侧滑菜单。 |
| 文件夹选项                                                   |                                                              |
| **添加/导入内容（Add/Import Content）**                      | 此子菜单提供与内容浏览器导航栏上的"添加（Add）"按钮相同的功能。使用它可在当前所选文件夹中导入或创建新资产。 |
| **在资源管理器(Windows)中显示（Show in Explorer (Windows)）** / **在访达中显示(macOS)（Show in Finder (macOS)）** | 在Windows资源管理器(Windows)或访达(macOS)中打开文件夹。      |
| **重命名（Rename）**                                         | 使文件夹名称可编辑，以便进行更改。按Enter键以保存更改，或按Esc键以取消重命名。 |
| **添加到收藏夹（Add to Favorites）**                         | 将文件夹添加到"收藏夹（Favorites）"分段。                    |
| **设置颜色（Set Color）**                                    | 设置所选文件夹的颜色以用于整理用途。                         |
| 批量操作                                                     |                                                              |
| **全部保存（Save All）**                                     | 保存当前文件夹中已修改的所有资产。                           |
| **全部重新保存（Resave All）**                               | 重新保存当前文件夹中的所有资产，无论它们是否已修改。         |
| **删除（Delete）**                                           | 删除当前文件夹及其所有内容。                                 |
| **修复文件夹中的重定向器（Fix Up Redirectors in Folder）**   | 查找所选文件夹中对所有重定向器的引用，并在可能的情况下将其重新保存，然后删除已修复其所有引用者的所有重定向器。 |
| **迁移（Migrate）**                                          | 将此文件夹中的资产及其依赖性复制到其他项目的 `Content` 文件夹。有关更多信息，请参阅[迁移资产](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/migrating-assets-in-unreal-engine)页面。 |
| **引用查看界面（Reference Viewer）**                         | 显示文件夹的引用图表。有关更多信息，请参阅[查找资产引用](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/reference-viewer-in-unreal-engine)页面。 |
| **大小贴图（Size Map）**                                     | 显示大致内存的交互式贴图，其所示为此文件夹中的资产及其引用内容所使用的内存。 |
| **审计资产（Audit Assets）**                                 | 打开"资产审计"窗口，其中显示有关当前文件夹中资产的详细信息。你可以使用筛选器进一步优化此窗口中显示的信息。 |
| **着色器烘焙统计数据（Shader Cook Statistics）**             | 显示与着色器烘焙相关的统计数据。                             |
| **验证文件夹中的资产（Validate Assets in Folder）**          | 验证文件夹中包含的资产并标记有问题的资产。                   |
| 源功能按钮                                                   |                                                              |
| **连接到源功能按钮（Connect to Source Control）**            | 将此文件夹连接到源功能按钮。将此文件夹连接到源功能按钮后，下面的操作将变为可用。 |
| **检出（Check Out）**                                        | 将所选文件夹标记为已检出，从而将其锁定，防止其他用户进行编辑。 |
| **标记为添加（Mark for Add）**                               | 将所选文件夹标记为添加到源功能按钮服务器。                   |
| **检入（Check In）**                                         | 提交所有编辑和添加操作，然后解锁已检出的文件夹。             |
| **同步（Sync）**                                             | 将此文件夹中的所有资产同步到最新版本。这可能会覆盖你所做的所有本地更改。 |

| **选项**                                 | **说明**                                                     |
| ---------------------------------------- | ------------------------------------------------------------ |
| **移至此处（Move Here）**                | 将文件夹移至新位置并将其从原始位置中删除。                   |
| **复制到此处（Copy Here）**              | 在目标文件夹中创建所选文件夹的副本。                         |
| **高级复制到此处（Advanced Copy Here）** | 在目标文件夹中创建所选文件夹及其依赖性的副本。还将修复因移动而破坏的所有依赖性。 |



## 4.内容浏览器设置参考

**设置（Settings）** 按钮位于 **内容浏览器（Content Browser）** 的右上角。点击该按钮会打开一个菜单，你可以在其中调整内容浏览器当前实例的各种设置，例如：

- 视图类型（资产的显示方式：图块、列表或列）。
- 搜索筛选器。
- 要包含或排除的内容。
- 搜索选项。

![内容浏览器中的](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\ue5_1-content-browser-settings.png)

### 4.01.视图类型

![image-20240827082016692](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\image-20240827082016692.png)

这些设置会影响资产视图中资产的显示方式。你可以选择以下某个视图类型：

#### 4.01.01.图块

**图块（Tiles）** 视图将所有资产布局为图块网格，如下所示：

![使用图块视图的资产视图](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\asset-view-tiles.png)

#### 4.01.02.列表

**列表（List）** 视图将所有资产布局为带有名称和文件类型的缩略图列表，如下所示：

![使用列表视图的资产视图](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\asset-view-list.png)

#### 4.01.03.列

**列（Columns）** 视图使用属性的电子表格式排列来布局所有资产，如下所示：

![使用列视图的资产视图](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\asset-view-columns.png)

显示的细节会根据资产类型而变化。例如，蓝图资产显示其类型和父类，静态网格体显示其顶点和三角形数量。

你可以对每个列执行以下操作：

- 左键点击列名，按列值的升序或降序对资产排序。
- 将鼠标悬停在列名上，然后点击垂直省略号菜单并选择 **隐藏列（Hide Column）** ，以隐藏该列。
- 在 **设置（Settings）** 菜单中选择 **切换列（Toggle Columns）** 选项并启用你想显示的列，以将该列取消隐藏。

你还可以将所有资产细节导出为 `.csv` 文件。从 **设置（Settings）** 菜单，选择 **导出为CSV（Export to CSV）** 选项。请注意，仅当资产查看者当前使用的是列视图时，才会显示此选项。

### 4.02.锁定

**锁定内容浏览器（Lock Content Browser）** 选项是可切换的设置。如果启用，此内容浏览器实例将忽略"在内容浏览器中查找"的请求。

### 4.03.视图

使用 **视图（View）** 设置切换内容浏览器中显示的内容，以及筛选行为。

| **选项**                                 | **说明**                                                     |
| ---------------------------------------- | ------------------------------------------------------------ |
| **显示文件夹（Show Folders）**           | 禁用此选项以使内容浏览器在单个视图中显示项目中的所有资产。禁用 **显示空文件夹（Show Empty Folders）** 子选项以使内容浏览器仅显示至少包含一个资产的文件夹。 |
| **显示空文件夹（Show Empty Folders）**   | 禁用此选项以使内容浏览器隐藏空文件夹。                       |
| **显示收藏夹（Show Favorites）**         | 启用此选项会在"源"面板顶部添加新的 **收藏夹（Favorites）** 类别。此类别显示你是否已将至少一个文件夹或资产添加到收藏夹。要将文件夹或资产添加到收藏夹，请右键点击它，然后从上下文菜单选择 **添加到收藏夹（Add To Favorites）** 。 |
| **以递归方式筛选（Filter Recursively）** | 切换此选项以控制资产视图筛选器是否应该以递归方式应用。       |
| **显示所有文件夹（Show All Folder）**    | 切换 `All`（所有）文件夹在"源"面板文件夹层级中的可视性。如果禁用，文件夹层级将上移一个级别。 |
| **整理文件夹（Organize Folders）**       | 启用此选项以在内容浏览器的 **资产（Asset）** 视图中自动整理文件夹。 |
| **路径视图筛选器（Path View Filters）**  | 切换会影响内容浏览器中的 **路径视图（Path View）** 的选项。在处理使用来自多个源的内容的大规模项目时，此选项很有用。 |
| **显示源面板（Show Sources Panel）**     | 切换此选项以显示或隐藏"源"面板。                             |

#### 4.03.01.内容

切换以下选项以控制特定类型的资产是否显示在资产视图中。

| **选项**                                        | **说明**                                                     |
| ----------------------------------------------- | ------------------------------------------------------------ |
| **显示C++类（Show C++ Classes）**               | 如果启用，将在"源"面板中显示 `Engine C++ Classes` 文件夹。此文件夹包含虚幻引擎中所有C++类的可浏览层级。 |
| **显示开发人员内容（Show Developers Content）** | 如果启用，将在"源"面板中显示 `Developers` 文件夹。此文件夹用于在多用户项目上与其他开发人员协作。 |
| **显示引擎内容（Show Engine Content）**         | 如果启用，将在"源"面板中显示 `Engine Content` 文件夹。此文件夹包含带有各种内容和功能的虚幻引擎现有资产的集合。 |
| **显示插件内容（Show Plugin Content）**         | 如果启用，特定于插件的内容将在内容浏览器中显示。             |
| **显示本地化内容（Show Localized Content）**    | 如果启用，本地化内容将在内容浏览器中显示。                   |

### 4.04.搜索

使用 **搜索（Search）** 选项可控制在内容浏览器中执行的搜索中包含或排除哪些内容。

- 资产类名
- 资产路径
- 集合名称

#### 4.04.01.缩略图

使用 **缩略图（Thumbnail）** 选项可控制生成和显示缩略图的方式。

| **选项**                                  | **说明**                                                     |
| ----------------------------------------- | ------------------------------------------------------------ |
| **缩略图大小（Thumbnail Size）**          | 为资产视图中显示的缩略图选择五种可能的大小之一：微小小中大超大 |
| **缩略图编辑模式（Thumbnail Edit Mode）** | 如果启用，你可以在3D资产的缩略图内左键点击并拖动以调整相应缩略图。完成后，点击"编辑完成（Done Editing）"按钮以保存更改。要恢复更改，请点击缩略图右上角的"撤销（Undo）"按钮。你必须保存资产以保存对其缩略图所做的更改。\| |
| **实时缩略图（Real-Time Thumbnails）**    | 如果启用，资产缩略图将实时渲染。                             |

### 4.05.内容浏览器编辑器偏好设置

你可以从[编辑器偏好设置](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/unreal-editor-preferences)调整会对内容浏览器造成影响的更多设置（菜单：**编辑（Edit）> 编辑器偏好设置（Editor Preferences）**，然后选择 **内容浏览器（Content Browser）** 分段）。

| **设置**                                                     | **说明**                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| **发出警告前可同时加载的资产数（Assets to Load at Once Before Warning）** | 在虚幻引擎显示警告之前，内容浏览器中可以同时加载的资产数量。 |
| **默认打开源面板（Open Sources Panel by Default）**          | 如果启用，内容浏览器将默认打开"源"面板。                     |
| **要保留在"最近打开"筛选器中的资产数（Number of Assets to Keep in the Recently Opened Filter）** | 资产视图中"最近打开"筛选器显示的资产数量。                   |
| **启用实时材质实例缩略图（Enable Realtime Material Instance Thumbnails）** | 如果启用，材质实例缩略图将实时渲染。                         |



## 5.筛选器和集合

**筛选器（Filters）** 和 **集合（Collections）** 是在内容浏览器中对资产进行排序和分组的两种不同方法。它们之间有一些主要区别：

- 筛选器 **自动** 在资产视图（Asset View）中显示或隐藏资产。你可以同时启用多个筛选器，并单独切换打开或关闭它们。筛选器可以保存在本地，并在不同项目之间共享。
- 集合包含 **手动** 添加的资产引用。你一次只能在资产视图（Asset View）中查看一个集合的内容。集合可以在你的机器本地，你也可以与其他用户共享。

筛选器和集合应用于单独的内容浏览器。这意味着你可以用不同的内容浏览器显示不同类型的资产，例如，一个内容浏览器只能显示属于特定集合的静态网格体，而另一个可以显示20个最近打开资产。

### 5.01.资产筛选器

**筛选器（Filter）** 提供了一种可以缩小内容浏览器资产视图中可见资产范围的方式。筛选器可以基于：

- 资产类型，例如蓝图、材质、静态网格体等。
- 资产状态，例如资产当前是否已从源控制点检出。

与集合不同，你可以同时激活多个筛选器。

#### 5.01.01.启用筛选器

要启用筛选器，首先要在 **内容浏览器（Content Browser）** 的 **筛选器** 部分进行添加。在内容浏览器的 **搜索栏**， 点击 **筛选器** 下拉菜单（如下图中所示）。这样会打开一个菜单，包含全部可以选择的筛选器，并且分为不同类别。

![Filters drop-down in the Content Browser](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\ue5_1-filters-button.png)

点击一个筛选器来将其添加到 **筛选器** 区域。你还可以点击类别来添加整个类别的全部筛选器。筛选器类别旁边的复选框可以表示该类别下是否有使用中的筛选器：

- 加号 (**+**) 意味着类别中的全部筛选器都启用。
- 减号 (**-**) 意味着类别中一部分筛选器启用。
- 空白的复选框意味着类别中没有筛选器被启用。

> 筛选器是累加的，这意味着你添加的任何新筛选器都会增加资产视图（Asset View）中可能显示的资产数量。例如，如果你从选择 **静态网格体（Static Mesh）** 筛选器开始，你将只会看到静态网格体。如果你随后选择 **蓝图（Blueprint）** 筛选器，你将看到静态网格体和蓝图。

你还可以从下拉菜单创建 **自定义筛选器（custom filters）**。前往 **自定义筛选器（Custom Filter） > 创建新筛选器（Create New Filter）**，然后在弹出的窗口中输入以下信息：

![Creating a custom filter](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\ue5_1-create-custom-filter.png)

- **筛选器标签（Filter Label）**: 为你的筛选器命名。筛选器名称不能重复。
- **颜色（Color）**: 使用调色盘来选择该筛选器在内容浏览器的筛选器区域中显示的颜色。
- **筛选器字符串（Filter String）**: 输入该筛选器的条件。你可以使用[高级搜索运算符](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/advanced-search-syntax-in-unreal-engine)。

#### 5.01.02.停用筛选器

有两种方式可以停用筛选器：

- 直接在 **筛选器** 区域点击来切换开关。停用了的筛选器会显示为灰色，不再生效。再次点击就可以重新打开筛选器。这样停用筛选器不会将其从 **筛选器** 区域中移除。
- 从 **筛选器** 下拉菜单，找到启用的筛选器并且点击其名称就可以将其停用。这样也会将其从 **筛选器** 区域中移除。

![An example of enabled and disabled filter](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\ue5_1-enabled-and-disabled-filters.png)

在这个示例中，启用了 关卡（Level） 和 材质（Material） 筛选器，而 动画蓝图（AnimBP） 和 开发者资产（devAssets） 筛选器没有启用。

#### 5.01.03.删除自定义筛选器

> 通过这种方式删除自定义筛选器 **不会** 弹出确认对话框，并且无法撤销操作。

要删除一个自定义筛选器，执行以下操作：

1. 在 **筛选器** 下拉菜单中，找到 **自定义筛选器（Custom Filters）**。
2. 找到要删除的筛选器，点击它旁边的 **编辑（Edit）** 按钮 (![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\ue5_1-edit-icon.png))。
3. 在弹出的窗口中，点击 **删除** 按钮。

#### 5.01.04.批量筛选器操作

右键点击 **搜索和筛选器栏（Search and Filters）** 栏中的筛选器，打开上下文菜单，其中包含以下批量筛选器操作：

| **操作**                                                     | **说明**                                                     |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| **Remove: [Filter Name]**                                    | Removes this filter from the **Filters** area. If it is a custom filter, it will not be deleted and you can re-add it from the **Filters** drop-down. |
| **仅启用此：[筛选器名称]（Enable Only This: [Filter Name]）** | 禁用除当前选定的筛选器之外的所有其他筛选器。                 |
| **启用全部筛选器（Enable All Filters）**                     | 启用全部筛选器。                                             |
| **禁用全部筛选器（Disable All Filters）**                    | 禁用全部筛选器。请注意，这不会从搜索和筛选器（Search and Filters）栏中删除任何筛选器。 |
| **删除全部筛选器（Remove All Filters）**                     | 从搜索和筛选器（Search and Filters）栏中删除全部筛选器。**此操作无法撤销。** |
| **删除除此：[筛选器名称]外的全部筛选器（Remove All But This: [Filter Name]）** | 从搜索和筛选器（Search and Filters）栏中删除除当前选择的筛选器之外的全部筛选器。**此操作无法撤销。** |

#### 5.01.05.使用最近打开筛选器

**最近打开（Recently Opened）** 筛选器使你能够查看选定文件夹的20个最近打开资产，可以在 **筛选器（Filters）** 菜单中的 **其他筛选器（Other Filters）** 类别下找到。

使用最近打开（Recently Opened）筛选器时，选择 **内容（Content）** 文件夹，将显示整个项目文件夹的最近打开资产。选择子文件夹可能只显示几个项目，或者什么都不显示。该列表取决于所选文件夹中包含的最近打开资产。

请注意，如果你在全新的项目中操作，此筛选器可能返回20个以下项目，甚至没有项目。

![内容浏览器中最近打开的筛选器。](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\recently-open-filter.png)

你可以更改最近打开筛选器列出的资产数量。在 **编辑器偏好设置（Editor Preferences）** 的 **内容浏览器（Content Browser）** 下，更改 **在最近打开筛选器中保留的资产数量（Number of Assets to Keep in the Nearly Opened Filter）** 。

### 5.02.集合

**集合** 是一种将资产集整理成组的方式。与文件夹不同，集合不包含资产本身，而仅包含对这些资产的引用。实际上，这意味着一个资产可以属于多个集合。

集合显示在文件夹树下的 **源（Sources）** 面板中。

#### 5.02.01.创建集合

要创建新集合，请按照以下步骤操作：

1. 点击集合（Collections）面板上的 **添加（Add）** （**+**） 按钮。

   ![添加新集合](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\adding-collections.png)

2. 选择集合 **类型** 。

   ![选择集合类型](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\collection-type.png)

   你可以选择以下选项之一：

   | **类型**                           | **说明**                                                     |
   | ---------------------------------- | ------------------------------------------------------------ |
   | **共享集合（Shared Collection）**  | 共享集合对其他用户可见。此选项仅在你处理多用户项目时可用。   |
   | **私人集合（Private Collection）** | 私人集合仅适用于被明确邀请查看集合的用户。此选项仅在你处理多用户项目时可用。 |
   | **本地集合（Local Collection）**   | 本地集合仅在你的本地机器上可用。                             |

3. 输入新集合的名称，然后按 **回车键（Enter）** 。

> 你可以右键点击集合（Collection），然后从出现的上下文菜单中选择 **新增（New）** ，并按照上述步骤1-3来创建子集合。

#### 5.02.02.将资产添加到集合

你可以使用以下方法之一，将一项或多项资产添加到集合中：

- 点击资产选择它，然后将其拖到集合中。

- 右键点击资产。然后，从上下文菜单中，选择 **管理集合（Manage Collections）**，然后点击你要添加资产的目标集合。

  > 资产已经归属集合的名称旁边将有复选标记。

- 点击资产可以选择它，然后启用你要添加资产的目标集合旁边的复选标记。

  > 如果资产已经是该集合的一部分，则该集合旁边的复选标记将已启用。在这种情况下，清除复选标记将从该集合中 **删除** 资产。

如果你将资产添加到具有父集合的集合，则该资产也将添加到父集合。

#### 5.02.03.从集合中删除资产

你可以使用以下方法之一从集合中删除资产：

- 右键点击资产。然后，从上下文菜单中，选择 **管理集合（Manage Collections）**，然后点击你要从中删除资产的集合。

  > 资产已经归属集合的名称旁边将有复选标记。

- 点击资产可以选择它，然后禁用你要从中删除资产的集合旁边的复选标记。

> 如果你在集合中选择资产，并按 **删除（Delete）** ，你可以完全删除该资产。你将收到提示，确认这是你要执行的操作，但请记住，删除资产意味着它 **完全** 从你的项目中删除。要简单地从集合中删除资产，请始终使用上述方法之一即可。

#### 5.02.04.重命名和删除集合

​	要重命名集合，请右键点击它，并从上下文菜单中选择 **重命名（Rename）** 。然后，输入新名称，并按 **回车键（Enter）**。要取消重命名，请按 **Esc键** 。

​	要删除集合，请右键点击它，并从上下文菜单中选择 **删除（Delete）** ，然后在出现的确认窗口中点击 **删除（Delete）** 。请注意，由于集合是对实际资产的引用，因此删除你的集合不会删除集合中的资产。



## 6.高级搜索语法

在[内容浏览器](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/content-browser-in-unreal-engine)中可以使用高级搜索运算符来查找内容。这些运算符可以进行更细致的搜索，让你更快地找到需要的内容。你还可以用它来搜索资产元数据的"键-值"对，并访问特殊键值。

![内容浏览器中高级搜索](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\advanced-search-content-browser.png)

下表显示了所有可用的运算符：

| 运算符（类型）                  | 语法           | 描述                                                         | 示例                                                         |
| ------------------------------- | -------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **Equal（二元运算）**           | `=` `==` `:`   | 判断指定键的返回值是否等于指定值。                           | `Name="Blast"` `Name==Blast` `Name:Bla...`                   |
| **NotEqual（二元运算）**        | `!=` `!:`      | 判断指定键的返回值是否不等于指定值。                         | `Name!=Blast` `Name!:"Blast"`                                |
| **Less（二元运算）**            | `<`            | 判断指定键返回的值是否小于指定值。该运算符仅支持数字类型的值。 | `Triangles<92`                                               |
| **LessOrEqual（二元运算）**     | `<=` `<:`      | 判断指定键返回的值是否小于等于指定值。该运算符仅支持数字类型的值。 | `Triangles<=92` `Triangles<:92`                              |
| **Greater（二元运算）**         | `>`            | 判断指定键返回的值是否大于指定值。该运算符仅支持数字类型的值。 | `Triangles>92`                                               |
| **GreaterOrEqual（二元运算）**  | `>=` `>:`      | 判断指定键返回的值是否大于等于指定值。该运算符仅支持数字值。 | `Triangles>=92` `Triangles>:92`                              |
| **Or（二元运算）**              | `OR` `||` `|`  | 测试两个值，任意一个为 `true` 即返回 `true`。                | `Blast OR Type:Blueprint` `!Blast || Path:Testing` `Name:"Blast" | Path:Testing...` |
| **And（二元运算）**             | `AND` `&&` `&` | 测试两个值，两个值均为 `true` 则返回 `true`。                | `Blast AND Type:Blueprint` `!Blast || Path:Testing` `Name:"Blast" | Path:Testing...` |
| **Not（一元运算）**             | `NOT` `!`      | 测试运算符后面的值，返回反转结果。                           | `NOT Blast` `! "Blast"`                                      |
| **TextCmpInvert（一元运算）**   | `-`            | 修改文本值，以便返回其所参与的运算的反转结果。               | `-Blast` `-"Blast"`                                          |
| **TextCmpExact（一元运算）**    | `+`            | 修改文本值，以便执行"精确"文本比较。                         | `+Blast` `+"Blast"`                                          |
| **TextCmpAnchor（一元运算）**   | `...`          | 修改文本值，以便执行"结尾"文本比较。                         | `...ast` `..."ast"`                                          |
| **TextCmpAnchor（后一元运算）** | `...`          | 修改文本值，以便执行"开头"文本比较。                         | `Bla...` `"Bla"...`                                          |

### 6.01.特殊键

大多数可用于搜索的键来自于从资产注册表提取的资产元数据（Asset metadata）。不过，有几个特殊键适用于所有资产类型。这些特殊键仅支持 `Equal` 或 `NotEqual` 比较运算符。

| 键              | 别名 | 描述                       |
| --------------- | ---- | -------------------------- |
| **Name**        | N/A  | 资产名称。                 |
| **Path**        | N/A  | 资产路径。                 |
| **Class**       | Type | 资产类。                   |
| **ParentClass** | N/A  | 资产的父类。               |
| **Collection**  | Tag  | 包含资产的任何集合的名称。 |

### 6.02.字符串

字符串可以带引号（单引号或双引号），也可以不带引号。带引号的字符串可以包含嵌套引号；但是，必须使用反斜杠（\）表示嵌套引号结束。使用无引号和带引号字符串的主要差异在于带引号字符串允许在搜索词中使用空格和特殊字符。默认情况下，它们将执行部分字符串匹配，除非使用了 `TextCmpExact` 或 `TextCmpAnchor` 运算符来修改此行为。

以下是使用单引号和双引号以及反斜杠的部分示例：

```c++
	"Foo\"bar"  ->  Foo"bar
	'Foo\'bar'  ->  Foo'bar
	"Foo\'bar"  ->  Foo'bar
	'Foo\"bar'  ->  Foo"bar
	"Foo\\bar"  ->  Foo\bar
	'Foo\\bar'  ->  Foo\bar
```

必须使用反斜杠来转义对另一个反斜杠的使用。

### 6.03.资产元数据

将鼠标悬停于内容浏览器中的资产名称上将显示其元数据。

![纹理资产元数据示例](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(03)：内容浏览器.assets\example-asset-metadata.png)

不同资产可能会列出特定于该类型的不同元数据，因此静态网格体不同于骨架网格体。

你可以使用任意一种元数据来搜索带有该特征的资产。搜索时应使用以下语法：

**[元数据名称] [运算符] [字符串或数字值]**

例如：

```c++
Triangles>=10500
Type==Skeletal
UVChannels>2 
CollisionPrims!=0
```

> 元数据不区分大小写，但字符中间不需要空格。例如，要搜索变形目标（Morph Target），应写成 `MorphTarget` 。

### 6.04.基本搜索示例

基本搜索以元数据对象为输入，并使用运算符来测试字符串或值。

例如：

- 搜索包含超过1500个三角形的任何资产，应使用 `Triangles>1500` 。
- 要搜索所有的蓝图资产，应使用 `Type==Blueprint`。

### 6.05.高级搜索示例

通过使用 `AND`、`OR` 和 `NOT` 运算符，你可以同时测试多个搜索运算。例如，搜索任何使用半透明材质且该材质使用默认光照着色模型的资产，应使用以下句法：

```cpp
 
	BlendMode==Translucent AND ShadingModel==DefaultLit
 
```

通过使用 `AND` 运算符，两个测试混合模式和着色模型的运算都必须求值为True才能显示结果。

当你使用 `OR` 运算符时，任一运算单独求值为True即可显示结果。比如，并不是每个使用半透明混合模式的材质都使用默认光照。对于复杂的高级搜索，同类型运算符必须始终合并起来。如果开始使用不同的运算符类型，括号可以消除不明确性。例如，我们可以执行两个搜索，然后求值来显示结果。第一个运算对半透明和默认光照的任何材质求值：

```cpp
 
	BlendMode==Translucent AND ShadingModel==DefaultLit
 
```

第二个运算会对所有属于延迟贴花类型并且不使用场景颜色的材质进行求值：

```cpp
 
	MaterialDomain==DeferredDecal AND HasSceneColor==False
 
```

可以使用括号对上述两个搜索的结果求值。

```cpp
 
	(BlendMode==Translucent AND ShadingModel==DefaultLit) OR (MaterialDomain==DeferredDecal AND HasSceneColor==False)
 
```

通过在两个括号括起的表达式之间使用 `OR` 运算符，结果将单独对每个括号中的表达式求值，然后显示任意一个为 `True` 的结果。如果使用 `AND` 运算符，则所有四个运算都必须返回 `True` 才会显示结果。