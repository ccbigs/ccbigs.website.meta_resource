# UE学习(05)：使用项目和模板

`介绍如何创建和管理虚幻引擎项目、使用模板作为起始点以及创建自定义模板。`

虚幻引擎 **项目** 包含游戏和应用程序的所有内容，并将所有内容联系在一起。它包含磁盘上的许多文件夹和资产，例如蓝图、材质、3D资产、动画等。

**虚幻编辑器（Unreal Editor）** 中的[**内容浏览器（Content Browser）**](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/content-browser-in-unreal-engine)使用与磁盘上的 `Project` 文件夹相同的文件和文件夹结构。

[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\project-folder-structure.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/fb6a1ea0-2e79-4e77-a81a-5e7c1b41fc24/project-folder-structure.png)



"内容浏览器（Content Browser）"采用与磁盘上的虚幻引擎项目相同的文件和文件夹结构。点击图片查看大图。

每个虚幻引擎项目都有一个与之关联的 `.uproject` 文件。`.uproject` 文件是你创建、打开或保存项目的方式。你可以创建任意数量的不同项目并且并行处理它们。

## 1.新建项目

`介绍如何在虚幻引擎中创建并配置新项目。`

当你启动 **虚幻引擎** 时， **虚幻项目浏览器（Unreal Project Browser）** 会自动打开。你可以在此处：

- 新建项目。
- 打开现有项目。
- 管理现有项目。

下图说明了在虚幻引擎中新建项目的步骤。

![在虚幻引擎中新建项目](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\creating-new-project.png)

在虚幻引擎中，从 项目浏览器（Project Browser） 窗口新建项目。

要新建项目，请按照以下步骤操作：

1. 选择最符合你的行业和项目目标的 **开发类别** （1）。

	你可以从以下类别中进行选择：

	- 游戏
	- 电影、电视和直播活动
	- 建筑、工程和施工（AEC）
	- 汽车、产品设计和制造（APM）

2. 为你的项目选择 **模板** （2）。你可以选择的模板基于你在步骤1中选择的类别。

	> 虚幻引擎包含许多 **项目模板**，你可以将其用作自己项目的起始点。要了解有关可用的不同项目模板的更多信息，请参阅[模板参考](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/unreal-engine-templates-reference)页面。

3. 配置 **项目默认值（Project Defaults）** （3）。在此分段中，你可以选择目标平台（即运行游戏或应用程序的硬件，如计算机或移动设备）、配置质量和光线追踪设置等。

	> 以下某些设置可能不适用于某些模板。例如，手持式AR模板只能使用蓝图实现。

	你可以配置以下设置：

	| 设置                                | 说明                                                         |
	| ----------------------------------- | ------------------------------------------------------------ |
	| **实现（Implementation）**          | 选择你要如何实现项目的逻辑，例如角色移动、关卡过渡等。你可以选择以下选项：**蓝图（Blueprint）** ，如果你要在虚幻编辑器中构建项目，并使用蓝图视觉效果脚本（Blueprint Visual Scripting）系统来创建交互和行为。**C++** ，如果你要通过在Visual Studio中使用C++编程来构建你的项目。有关实现方法的更多信息，请参阅以下页面：[蓝图视觉效果脚本](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/blueprints-visual-scripting-in-unreal-engine)[使用C++编程](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/programming-with-cpp-in-unreal-engine) |
	| **目标平台（Target Platform）**     | 选择你的项目适用的平台类型：**桌面（Desktop）****移动端（Mobile）** |
	| **质量预设（Quality Preset）**      | 根据你的项目目标平台，选择最高质量级别。我们建议你选择：**最大值（Maximum）** ，如果你正在为计算机或游戏主机开发项目。**可扩展（Scalable）** ，如果你正在为移动设备开发项目。 |
	| **初学者内容包（Starter Content）** | 选择你是否希望新项目包含 **初学者内容包** 。初学者内容包包括一些带有基本纹理和材质的简单静态网格体。如果你想立即开始学习和试验，这将非常有用，且无需为获取和导入自定义内容担心。 |
	| **光线追踪（Ray Tracing）**         | 为你的项目选择是启用还是禁用 **光线追踪**。关于虚幻引擎中光线追踪的更多信息，请参阅[实时光线追踪](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/ray-tracing-and-path-tracing-features-in-unreal-engine)页面。 |

4. 选择你要存储项目的位置，并为项目命名（4）。

5. 点击 **创建（Create）** （5），完成项目新建。



## 2.打开现有项目

`介绍如何访问和打开虚幻引擎中的现有项目。`

可通过多种方式打开现有虚幻引擎项目，具体取决于该项目所在位置以及创建该项目所使用的虚幻引擎版本。

### 2.01.从Epic Games启动程序打开项目

在Epic Games启动程序中，点击左侧导航中的 **虚幻引擎（Unreal Engine）** ，然后点击启动程序顶部的 **库（Library）** 。你将在本地计算机上看到所有虚幻引擎项目的列表。

> 如果你从其他计算机或从互联网复制了项目，该项目仅当你在本地将其打开至少一次之后才会显示在此列表中。请参阅此页面上的 **从磁盘打开项目（Opening Projects From Disk）** 分段，了解更多信息。

[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\epic-launcher-myprojects.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/ff19b7b0-84da-4b4f-925f-26e5710ed15d/epic-launcher-myprojects.png)

`Epic Games启动程序的"我的项目（My Projects）"分段。点击查看大图。`

双击某个项目缩略图以打开该项目。

启动程序会为每个项目显示以下信息：

- 项目名称
- 项目缩略图
- 项目兼容的虚幻引擎版本

右键点击启动程序中的项目缩略图会显示上下文菜单，其中包含以下选项：

| **选项**                             | **说明**                                                     |
| ------------------------------------ | ------------------------------------------------------------ |
| **打开（Open）**                     | 在项目兼容的虚幻引擎版本中打开项目。                         |
| **在文件夹中显示（Show in folder）** | 在新的Windows资源管理器(Windows)或访达(macOS)窗口中打开项目文件夹。 |
| **创建快捷方式（Create shortcut）**  | 在桌面上创建项目的快捷方式。                                 |
| **克隆（Clone）**                    | 创建项目的精确副本。你可以指定新项目的名称和位置。           |
| **删除（Delete）**                   | 永久删除项目。==项目文件 **不会** 像你从Windows资源管理器或访达中删除项目文件夹时那样移入回收站。如果你使用此选项意外删除了项目，将无法恢复该项目。== |

### 2.02.从项目浏览器打开项目

当你启动某个 **虚幻引擎（Unreal Engine）** 版本时，**项目浏览器（Project Browser）** 会显示，并默认打开 **最近项目（Recent Projects）** 面板。此分段会显示磁盘上的所有虚幻引擎项目，这与Epic Games启动程序中的项目列表非常类似。

> 如果你从其他计算机或从互联网复制了项目，该项目仅当你在本地将其打开至少一次之后才会显示在此列表中。请参阅此页面上的 **从磁盘打开项目（Opening Projects From Disk）** 分段，了解更多信息。

[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\project-browser-ue5.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/3173803e-bc06-45be-b7ea-b5c970d76869/project-browser-ue5.png)

`虚幻引擎5中的项目浏览器。点击查看大图。`

双击某个项目缩略图以打开该项目。或者，点击选中该项目，然后点击 **打开（Open）** 。

启动程序会为每个项目显示以下信息：

- 项目名称
- 项目缩略图
- 项目兼容的虚幻引擎版本

右键点击项目浏览器中的项目缩略图会显示上下文菜单，其中包含用于在Windows资源管理器或访达窗口中打开项目文件夹的选项。

> 启用项目浏览器左下方的 **启动时始终加载最后一个项目（Always load last project on startup）** 复选框，以使虚幻引擎5在你启动引擎时始终打开你工作过的最后一个项目。

### 2.03.从虚幻引擎打开项目

在 **虚幻引擎（Unreal Engine）** 的主菜单中，转到 **文件（File）> 打开项目（Open Project）** 。这将打开一个窗口，其中显示本地项目的列表，类似于 **项目浏览器（Project Browser）** 。

[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\open-project-from-ue.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/0c71bf0d-71d2-4292-8984-2435cabc7f67/open-project-from-ue.png)

`从虚幻引擎打开项目。点击查看大图。`

要打开项目，请执行以下一项操作：

- 从列表选择项目，然后点击 **打开（Open）** 。
- 双击项目缩略图。

如果你要打开的项目不在列表中，请点击 **浏览（Browse）** ，然后浏览到项目文件夹，并打开 `(ProjectName).uproject` 文件。

> 如果打开项目所用虚幻引擎版本不同于创建该项目所用版本，这可能导致数据损坏和数据丢失。推荐打开项目的副本，保留原始项目。

### 2.04.从磁盘打开项目

如果你从其他计算机或从互联网复制了项目，该项目仅当你在本地将其打开至少一次之后才会显示在此列表中。

要从磁盘打开项目，请执行以下步骤：

1. 确保你已安装创建项目所用的虚幻引擎版本。
2. 导航至磁盘上的项目文件夹。
3. 双击 `(ProjectName).uproject` 文件。此文件就位于项目所在的文件夹中。

![从磁盘打开虚幻引擎项目](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\open-project-from-disk.png)

`在此示例中，你将双击 MyProject.uproject 文件。`

如果你没有创建项目所用的虚幻引擎版本，系统将显示一个弹出窗口，要求你选择使用哪个虚幻引擎版本打开项目。

![选择用于打开项目的虚幻引擎版本](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\select-ue-version.png)

从下拉菜单选择虚幻引擎版本，或点击 **省略号** (**...**)按钮以浏览到磁盘上的虚幻引擎可执行文件，然后点击 **确定（OK）** 。

> 如果打开项目所用虚幻引擎版本不同于创建该项目所用版本，这可能导致数据损坏和数据丢失。推荐打开项目的副本，保留原始项目。



## 3.模板参考

`虚幻引擎中的模板与模板的用法`

在创建新的虚幻引擎项目时，你可以使用现有模板之一来作为游戏或应用程序的基础。虚幻引擎模板中包含角色控制器、蓝图和其他不需要额外配置即可运行的功能。

如需有关如何根据模板创建新项目的说明，请参阅[新建项目](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/creating-a-new-project-in-unreal-engine)页面。

在选择模板时，你将会看到一则说明，详细介绍模板以及模板中包含的内容。

[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\example-template-description.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/3a47bbe0-4d3b-412a-a413-69b40e21ffa5/example-template-description.png)

`第三人称游戏模板的模板说明示例。点击查看大图。`

此外，你还可以根据任何现有项目来创建自定义模板。如需了解更多信息，请参阅[创建自定义模板](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/converting-a-project-to-an-unreal-engine-template)页面。

### 3.01.为可以操控的角色配置输入

很多模板中都包含一个可以使用键盘、鼠标或控制器来控制的角色。在虚幻引擎属于中，这种角色称为Pawn。

你可以在 **项目设置（Project Settings）** 的 **输入（Input）** 部分中查看Pawn的现有功能按钮和配置新功能按钮。要打开项目设置，请执行以下操作：

1. 在主菜单中，前往 **编辑（Edit）> 项目设置（Project Settings）**。
2. 在左边的侧边栏中，向下滚动到 **引擎（Engine）** 部分，然后点击 **输入（Input）**。

展开 **绑定（Bindings）** 部分，你可以看到以下选项：

- **动作映射（Action Mappings）**：定义用于控制动作（例如跳跃）的按键。
- **轴映射（Axis Mappings）**：控制移动。根据模板的不同，可以将角色移动限制到一个或几个轴上。例如，在"横版过关游戏"模板中，Pawn只能左右移动和跳跃。

[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\input-example.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/324166a1-f87c-4197-b6bf-39ebbd4d0e34/input-example.png)



### 3.2.虚幻引擎中的模板

虚幻引擎中的模板分为以下几类：

- 游戏
- 电影、电视和直播活动
- 建筑、工程和施工
- 汽车、产品设计和制造
- 模拟

每种类别中都包含一个 **空白（Blank）** 模板，该模板包含一个空项目，没有任何其他内容和设置。这是最基础的模板。

#### 3.2.1.游戏模板

![虚幻引擎5中的载具高级模板](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\templates-vehicle-advanced.png)

`虚幻引擎5中的载具高级模板。`

虚幻引擎的 **游戏（Games）** 模板是构建各种游戏的快速起点，例如第一人称或第三人称游戏、横版过关游戏或赛车游戏。

> 虽然这些模板都标记为"游戏"模板，其实可以用作任何类型项目的起点。例如，可以使用VR模板来创建三维空间的虚拟现实指南。第三人称模板通常都是很多不同类型项目的良好起点。

| 模板名称                        | 模板内容                                                     | 其他文档                                                     |
| ------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **第一人称（First Person）**    | 第一人称角色，配备的枪可以基于物理原理射出发射物。玩家从角色的视角体验关卡内容。 | [第一人称模板概述](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/first-person-template-in-unreal-engine) |
| **第三人称（Third Person）**    | 第三人称角色和基本几何体。摄像机位于角色后上方。             | [第三人称模板概述](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/third-person-template-in-unreal-engine) |
| **自上而下（Top Down）**        | 点按新位置后可移动的角色。摄像机位于角色上方的固定位置，并随着角色的移动而移动。 |                                                              |
| **手持式AR（Handheld AR）**     | 用来创建AR应用程序的起点，以便部署到Android或iOS。包含用于扫描环境来收集数据的运行时逻辑，这些数据用于在虚拟场景中创建交互式平面，并且可以提供照明和场景深度信息。 | [手持式AR模板快速入门](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/handheld-ar-template-quickstart-in-unreal-engine)[手持式AR模板技术参考](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/handheld-ar-template-technical-reference) |
| **载具（Vehicle）**             | 符合物理特性的简单载具，具有两个不同的摄像机视角——一个在载具内部，另一个在载具后上方——还有HUD。 |                                                              |
| **虚拟现实（Virtual Reality）** | 虚幻引擎5中的所有虚拟现实(VR)项目的起点。并且封装了传送以及常见输入操作（例如将物品在握手中）的逻辑。 | [VR模板](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/vr-template-in-unreal-engine)[在虚幻引擎中开发VR](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/developing-for-xr-experiences-in-unreal-engine) |

#### 3.2.2.电影、电视和直播活动模板

![虚幻引擎5中的DMX模板](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\templates-dmx.png)

`虚幻引擎5中的DMX模板。`

**电影、电视和直播活动（Film, Television, and Live Events）** 模板为直播制片工作提供了一个良好的起点。

| 模板名称                           | 模板内容                                                     | 其他文档                                                     |
| ---------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **虚拟制片（Virtual Production）** | 具有适用于VR探查、虚拟摄像机、SDI视频、Composure和nDisplay的功能。 | [虚拟探查概述<br/>](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/virtual-scouting-overview)[虚拟摄像机Actor快速入门](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/virtual-camera-component-in-unreal-engine) |
| **DMX**                            | 其中包括用于寻址、修补和控制代理光照灯具，以及进出虚幻引擎的实时DMX数据流送的录制和播放示例。 | [DMX](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/dmx-in-unreal-engine) |
| **InCamera VFX**                   | 适用于摄像机内视觉特效处理工作流的蓝图、插件和示例舞台。将此模板用作使用LED体积来实现虚拟制片拍摄时的基础。 | [摄像机内视觉特效处理模板<br />](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/in-camera-vfx-template-in-unreal-engine)[摄像机内视觉特效处理概述](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/in-camera-vfx-in-unreal-engine) |
| **nDisplay**                       | 通过计算机集群实现的显示功能。将此模板作为起点，在复杂排列的物理显示器上进行渲染，以获得直播效果。 | [nDisplay模板<br />](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/ndisplay-template-in-unreal-engine)[利用nDisplay渲染到多个显示器](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/rendering-to-multiple-displays-with-ndisplay-in-unreal-engine) |

#### 3.2.3.建筑、工程和施工模板

![虚幻引擎5中的建筑模板](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\templates-aec.png)

`虚幻引擎5中的建筑模板。`

**建筑、工程和施工（Architecture, Engineering, and Construction）** 模板使用Datasmith将各种3D程序中的内容导入到虚幻引擎，而你可以在虚幻引擎中对这些内容进行进一步优化，以便于在桌面应用程序和XR应用程序中使用。

| 模板名称                              | 模板内容                                                     | 其他文档                                                     |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **建筑（Archvis）**                   | 样板建筑可视化工作流，其中带有可以用于阳光研究、内部渲染和非真实感风格渲染的示例场景。 |                                                              |
| **设计配置器（Design Configurator）** | 可使用Variant Manager、UMG和蓝图功能来构建项目，在项目中可以切换不同的对象状态，例如可见性、启动动画序列、切换视图、切换不同设计选项。 |                                                              |
| **协作查看器（Collab Viewer）**       | 适用于协作式会话中的台式机和VR的导航和交互功能。此模板包含一些专门用于建筑领域的初学者内容包，默认启用了一些其他组件，包括OpenXR和LiveLink。 | [协作查看器模板](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/collab-viewer-templates-in-unreal-engine) |
| **手持式AR（Handheld AR）**           | 可作为创建AR应用的起点，供你部署到Android或iOS上。包括用于扫描环境的运行时逻辑，可以收集数据并在虚拟场景中创建交互式平面，以及收集光照和场景深度信息。 | [手持式AR模板快速入门](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/handheld-ar-template-quickstart-in-unreal-engine)[手持式AR模板技术参考](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/handheld-ar-template-technical-reference) |

#### 3.2.4.汽车、产品设计和制造模板

![虚幻引擎5中的Photo Studio模板。](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\templates-apm.png)

`虚幻引擎5中的Photo Studio模板。`

**汽车、产品设计和制造（Automotive, Product Design, and Manufacturing）** 模板使用Datasmith将各种3D程序中的内容导入到虚幻引擎，而你可以在虚幻引擎中对这些内容进行进一步优化，以便于在桌面应用程序和XR应用程序中使用。

| 模板名称                               | 模板内容                                                     | 其他文档                                                     |
| -------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **Photo Studio**                       | 这是一个预制的摄影工作室场景，可以用于过场动画或产品展示。   |                                                              |
| **产品配置器（Product Configurator）** | 可使用Variant Manager、UMG和蓝图功能来构建常规产品配置器，这是一种程序，在程序中可以切换不同的零部件来测试产品的新外观，例如汽车的不同颜色。 | [产品配置器](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/product-configurator-template-in-unreal-engine) |
| **协作查看器（Collab Viewer）**        | 适用于协作式会话中的台式机和VR的导航和交互功能。此模板还包含可以在VR中探索的样板模型汽车。 | [协作查看器模板](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/collab-viewer-templates-in-unreal-engine) |
| **手持式AR（Handheld AR）**            | 可作为创建AR应用的起点，供你部署到Android或iOS上。包括用于扫描环境的运行时逻辑，可以收集数据并在虚拟场景中创建交互式平面，以及收集光照和场景深度信息。 | [手持式AR模板快速入门](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/handheld-ar-template-quickstart-in-unreal-engine)[手持式AR模板技术参考](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/handheld-ar-template-technical-reference) |

#### 3.2.5.模拟模板

![虚幻引擎5中的模拟模板](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\templates-simulation.png)

虚幻引擎5中的模拟模板的用法说明。

**模拟** 模板为各种企业模拟应用程序提供了范围广泛的起始点。这些模板包含以下功能：

- 户外环境的特定设置。
- 逼真的天空和光照。
- 地理配准工具。

| 模板名称                         | 模板内容                                                     | 其他文档                                                     |
| -------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **模拟空白（Simulation Blank）** | 该模板由带有必需设置并启用了插件的空白项目组成。此模板适合作为大部分模拟应用程序的起始点，并包含以下功能：地球大气大气光照体积云地理坐标[世界大地测量系统 (WGS84)）](https://zh.wikipedia.org/wiki/世界大地测量系统) |                                                              |
| **手持式AR（Handheld AR）**      | 用来创建AR应用程序的起点，以便部署到Android或iOS。包含用于扫描环境来收集数据的运行时逻辑，这些数据用于在虚拟场景中创建交互式平面，并且可以提供照明和场景深度信息。 | [手持式AR模板快速入门](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/handheld-ar-template-quickstart-in-unreal-engine)[手持式AR模板技术参考](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/handheld-ar-template-technical-reference) |
| **虚拟现实（Virtual Reality）**  | 虚幻引擎5中的所有虚拟现实(VR)项目的起点。该模板封装了传送移位以及常见输入操作的逻辑，例如抓取物品和将物品附着到手上。 | [VR模板](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/vr-template-in-unreal-engine)[在虚幻引擎中开发VR](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/developing-for-xr-experiences-in-unreal-engine) |



### 3.3.第一人称模板

虚幻引擎中第一人称模板介绍

当你创建新项目时，**虚幻引擎（Unreal Engine）** 会向你提供模板列表，供你选择。这些模板包含一些可立即使用的资产，例如关卡几何体、你可以控制的角色以及简单的角色动画。许多教程将其中一款模板用作起始点。

在 **第一人称** 游戏中，玩家从他们扮演角色的视点来查看游戏。一些第一人称游戏会显示角色模型的某部分，例如角色的手臂或武器。这与[第三人称游戏](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/third-person-template-in-unreal-engine)不同，在后者中，你可以从角色背后略上方的位置看到角色动作。

虚幻引擎5的 **第一人称** 模板包含以下内容：

- 一个玩家可以控制的第一人称角色，可以移动和射击。
- 一把可以发射子弹并被捡起的枪。
- 一个带有基本几何体（斜坡、平台等）的关卡。
- 会对角色及子弹的撞击做出反应的立方体。

#### 3.3.1.创建第一人称项目

启动虚幻引擎5会打开 **项目浏览器（Project Browser）** 窗口，你可以在其中选择打开现有的虚幻项目，或创建新项目。要创建第一人称项目，请选择左侧的 **游戏（Games）** 类别，然后选择 **第一人称（First Person）** 模板。

![在虚幻引擎5中创建新的第一人称项目。](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\create-new-project.png)

`在虚幻引擎5中创建新的第一人称项目。`

你可以为第一人称项目配置几个附加设置。有关这些内容的概述，请参阅[新建项目](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/creating-a-new-project-in-unreal-engine)页面。

> 如果你想要一些现成的对象来填充你的关卡，请在配置项目设置（Project Settings）时，选择 **带初学者内容包（With Starter Content）** 选项。在你熟悉虚幻引擎中的功能按钮和工作流程的过程中，这些选项非常有帮助。

完成这些步骤后，你应该拥有一个基本关卡，并带有一个可以控制的第一人称角色。你可以通过鼠标和键盘控制人物。

> 试试你的新关卡吧！在主工具栏（Main Toolbar）中，点击 **运行（Play）**，然后尝试四处移动，并射击一些立方体。使用WASD键来移动角色，移动鼠标来观察四周。走到枪面前并捡起，然后点击鼠标左键来发射子弹。

#### 3.3.2.模板内容

第一人称模板包含了创建第一人称射击游戏或者任何第一人称体验所需的所有基本元素。以下小节将会详细介绍这些元素并且指出如何在 **内容浏览器（Content Browser）** 中找到它们。

##### 3.3.2.1.蓝图

第一人称模板包含以下蓝图：

- 玩家角色蓝图
- 步枪蓝图
- 步枪子弹蓝图
- 游戏模式蓝图

这些蓝图位于 `Content/FirstPerson/Blueprints` 文件夹中。

每个蓝图的 **事件图表（Event Graph）** 都包含注释和标注，可以帮助用户学习不同节点组的功能和背后的实现逻辑。

[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\bp_rifle-blueprint.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/bd479816-3048-4fd1-9598-798cfd4295af/bp_rifle-blueprint.png)

`这里可以看到 BP_Rifle 蓝图中的开发者注释。点击查看大图。`

##### 3.3.2.2.第一人称角色

用于玩家角色的资产位于 `Content/FirstPersonArms` 文件夹。这里可以找到骨骼网格体、材质、纹理以及角色使用的动画。![image-20240827111254651](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\image-20240827111254651.png)

##### 3.3.2.3.步枪和子弹

`Content/FPWeapon` 文件夹包含了步枪和子弹使用的资产。步枪使用骨骼网格体 (**SK_FPGun**)。子弹随着鼠标左键点击生成，并且向关卡中撞击的任何启用物理的Actor施加物理冲击。你可以在 `Content/FirstPerson/Blueprints` 文件夹里的 **BP_FirstPersonProjectile** 蓝图中看到该逻辑如何实现。

##### 3.3.2.4.关卡

组成关卡几何体的资产 (静态网格体、材质和纹理) 位于 `Content/LevelPrototyping` 文件夹。

#### 3.3.3.改进你的项目

现在你有了一个可游玩的关卡，就可以向其中导入内容并且进行调整来让你的游戏更加有趣。

向关卡中添加内容最简单的方法是将其从 **内容浏览器（Content Browser）** 中拖入。如果你在创建项目时选择包含了 **初学者内容（starter content）** ，你应该已经有了一些可以拖入关卡的额外内容。

更多关于如何充实关卡的详细教程，可以参考[关卡设计师快速入门](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/level-designer-quick-start-in-unreal-engine)。

#### 3.3.4.接下来呢？

你已经了解创建第一人称体验的基础知识，以下是你可以尝试的其他一些内容：

- 为你的枪[导入和配置](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/fbx-skeletal-mesh-pipeline-in-unreal-engine)不同的模型，或选择完全不同的武器。你可以从虚幻引擎[商城](https://www.unrealengine.com/marketplace/en-US/store)下载预制资产，或创建自己的资产。
- 试着用[Quixel Bridge](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/quixel-bridge-plugin-for-unreal-engine)中的免费资产丰富你的关卡。你可以用它们来搭建各种室内外场景，并且素材库中的资产会不断丰富。
- 使用[后期处理](https://www.unrealengine.com/en-US/onlinelearning-courses/post-processing-essentials)为你的游戏添加一些特别的视觉效果，例如运动模糊或晕影。
- 使用[虚幻运动图形（UMG）](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/umg-editor-reference-for-unreal-engine)创建游戏内平视显示器（HUD），显示玩家生命值和弹药数量等信息。
- 使用[行为树](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/behavior-trees-in-unreal-engine)添加AI角色。你可以将其设置为追逐、逃跑、帮助或伤害玩家。



### 3.4.第三人称模板

介绍虚幻引擎中的第三人称模板

当你创建新项目时，**虚幻引擎（Unreal Engine）** 会向你提供模板列表，供你选择。这些模板包含一些可立即使用的资产，例如关卡几何体、你可以控制的角色以及简单的角色动画。许多教程将其中一款模板用作起始点。

在 **第三人称** 游戏中，玩家从位于固定距离以外、稍高于其角色的摄像机查看游戏世界。在虚幻引擎中，你可以控制摄像机距离和位置，并根据需要进行调整。

虚幻引擎5中的 **第三人称** 模板包含以下元素：

- 可操作的第三人称角色，可以移动和跳跃。
- 角色的额外网格体。
- 带有基本几何体（斜坡、平台等）的关卡。
- 会对角色的撞击做出反应的启用物理的立方体。

模板还包括经过重新设计的人体模特。

#### 3.4.1.创建第三人称项目

启动虚幻引擎5会打开 **项目浏览器（Project Browser）** 窗口，你可以在其中选择打开现有的虚幻项目，或创建新项目。要创建第三人称项目，请选择左侧的 **游戏（Games）** 类别，然后选择 **第三人称（Third Person）** 模板。

![在虚幻引擎5中创建新的第三人称项目。](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\create-new-project.png)

`在虚幻引擎5中创建新的第三人称项目。`

你可以为第三人称项目配置几个额外的设置。有关这些内容的概述，请参阅[新建项目](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/creating-a-new-project-in-unreal-engine)页面。

> 如果你想使用一些可立即使用的对象来填充关卡，请选择 **使用初学者内容包（With Starter Content）** 选项。在你熟悉虚幻引擎中的功能按钮和工作流程的过程中，这些选项非常有帮助。

执行这些步骤后，你应该有一个基本关卡，其中有一个你可以控制的第三人称角色。

> 何不试试你的新关卡？在主工具栏中，点击 **运行（Play）**。 使用WASD键移动角色，按下空格键跳起，移动鼠标查看周围环境。

#### 3.4.2.模板内容

第三人称模板包含了简易第三人称体验的所有元素。可以以此为起点制作一个传统的角色扮演游戏（RPG）、第三人称射击游戏或者其它任何应用。以下部分详细介绍模板元素以及如何在 **内容浏览器（Content Browser）** 中找到它们。

##### 3.4.2.1.第三人称角色

玩家角色使用的资产位于 `Content/Characters` 文件夹。默认情况下，第三人称模板初始带有一个女性的虚幻引擎5人体模特。该文件夹还有玩家角色的额外骨骼网格体，包括新的虚幻引擎5和旧版本虚幻引擎的人体模特的风格。

![虚幻引擎5人体模特](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\ue5-mannequins.png)

`虚幻引擎5人体模特`

> 虚幻引擎5中新的人体模特叫做Manny和Quinn。

虚幻引擎5的人体模特还带有可以调整的 **多层次细节（Level of Detail (LOD)）** 设置。LOD可以帮助针对不同平台优化你的应用。例如，针对移动平台（安卓、iOS）的应用应该使用细节较少的角色模型。这样会改善你的应用在这些平台上的性能。控制人体模特LOD的数据资产位于 `Content/Characters/Mannequins/Meshes` 文件夹。

##### 3.4.2.2.动画

UE5人体模特的动画位于 `Content/Characters/Mannequins/Animations` 文件夹。针对两个人体模特有两组动画。

动画蓝图使用了虚幻引擎5全新的[IK Rig](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/unreal-engine-ik-rig)系统。与以往的版本不同，IK Rig可以用于动态修改基于姿势的解算器参数。以下截图便是一个例子：Quinn的脚部位置会根据她所处的地形动态调整。

![IK Rig动态姿势解算器](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\ue5-mannequin-ik-rig.png)

要了解如何实现，可以查看 `Content/Mannequins/Rigs` 文件夹中的 **CR_Mannequin_BasicFootIK** rig。

同样位于 `Rigs` 文件夹中，**CR_Mannequin_Body** Control Rig资产可以用于直接在编辑器中轻易地为人体模特调整姿势和添加动画。要了解如何使用Control Rig调整姿势和添加动画，参考虚幻引擎5文档的[Control Rig](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/control-rig-in-unreal-engine)分段。

##### 3.4.2.3.关卡

组成关卡几何体的资产（静态网格体、材质和纹理）位于 `Content/LevelPrototyping` 文件夹中。

#### 3.4.3.改进你的项目

现在你有了一个可游玩的关卡，就可以向其中导入内容并且进行调整来让你的游戏更加有趣。

##### 3.4.3.1.角色

你可以通过修改 **静态网格体（Static Mesh）** 来改变角色的外观。举个例子，我们来改变默认的人体模特网格体。请执行以下步骤：

1. 在 **内容浏览器（Content Browser）** 中，找到 `Content/ThirdPerson/Blueprints` 然后双击 **BP_ThirdPersonCharacter** 蓝图来在蓝图编辑器中将其打开。

	![打开第三人称角色蓝图](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\open-third-person-character-bp.png)

2. 在蓝图编辑器中的 **组件（Components）** 面板，点击 **网格体（Mesh(CharacterMesh)）** 组件来将其选中。

	[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\select-character-mesh.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/1c84af54-c733-4cab-a384-e72642243924/select-character-mesh.png)

3. 选中 **网格体（Mesh(CharacterMesh)）** 组件后，找到蓝图编辑器右侧的 **详情（Details）** 面板。然后，在 **网格体（Mesh）** 部分，点击 **骨骼网格体（Skeletal Mesh）** 参数旁的下拉菜单并从中选择 `SKM_Manny` 。

	[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\change-character-mesh.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/2fe08786-1053-45e9-90f9-3e80b46552d0/change-character-mesh.png)

4. 仍然在 **详情（Details）** 面板中，找到 **动画（Animation）** 部分，设置以下选项：

	- **动画模式（Animation Mode）**: 使用动画蓝图
	- **动画类（Anim Class）**: ABP_Manny

	[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\change-animation-bp.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/7270358e-0e91-4030-91ac-b3c74b8a022e/change-animation-bp.png)

5. **编译（Compile）** 并 **保存（Save）** 蓝图。

	![编译并保存蓝图](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\compile-save-blueprint.png)

6. 点击 **视口（Viewport）** 选项卡来确认网格体是否已经更新。

	[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\viewport-confirmation.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/3e7a749d-286a-496d-8015-8ddc50c0e120/viewport-confirmation.png)

你的角色已经可以跑和跳，而你还可以添加其他类型的 **角色运动**，如行走或蹲伏。有关详细的教程，请参阅[设置角色动作](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/setting-up-character-movement)。

##### 3.4.3.2.关卡

你的关卡已经有一些简单的几何体，如楼梯和平台。在里面添加更多内容的最简单方法是从 **内容浏览器（Content Browser）** 进行拖放。

如果你在创建项目时选择包括 **初学者内容包（starter content）**，你应该已经可以将一些东西拖放到关卡中。

有关如何填充关卡的更深入说明，请参阅[关卡设计师快速入门](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/level-designer-quick-start-in-unreal-engine)。

#### 3.4.4.接下来呢？

现在你已掌握了创建第三人称体验的基础知识，可以尝试下面的其他一些内容：

- 为你的玩家角色[导入和配置](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/fbx-skeletal-mesh-pipeline-in-unreal-engine)不同的模型。你可以从虚幻引擎[商城](https://www.unrealengine.com/marketplace/en-US/store)下载预制角色，或[使用MetaHuman](https://docs.metahuman.unrealengine.com/zh-CN/retargeting-animations-to-a-metahuman-at-runtime/)。
- 试着用[Quixel Bridge](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/quixel-bridge-plugin-for-unreal-engine)中的免费资产丰富你的关卡。你可以用它们来搭建各种室内外场景，并且素材库中的资产会不断丰富。
- 使用[后期处理](https://www.unrealengine.com/en-US/onlinelearning-courses/post-processing-essentials)将一些花式视觉效果添加到你的游戏中，例如动作模糊或渐晕。
- 使用[UMG](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/umg-editor-reference-for-unreal-engine)创建游戏内的抬头显示器(HUD)，以显示玩家生命值和武器数量等信息。
- 使用[行为树](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/behavior-trees-in-unreal-engine)添加AI角色。你可以将其设置为追逐、逃跑、帮助或伤害玩家。



### 3.5.模拟空白模板

`介绍虚幻引擎中的模拟空白模板`

**模拟空白（Simulation Blank）** 模板是一种 **空世界（Empty World）** 关卡模板，内附特定于模拟的设置和功能。它由带有以下功能和特征的空环境组成：

- 作为地面/地板的扁平静态网格体。
- 带有特定于地球的设置的[SunSky](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/geographically-accurate-sun-positioning-tool-in-unreal-engine)系统：
	- 与地理配准插件规范兼容的北偏移。
	- 带有逼真太阳属性（ **强度（Intensity）** 、 **源角度（Source Angle）** ）的定向光源，投射利用[虚拟阴影贴图](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/virtual-shadow-maps-in-unreal-engine)系统的远阴影（需要在 **项目设置（Project Settings）> 平台 - Windows（Platforms - Windows）** 下启用 **DirectX 12（SM6试验性）（DirectX 12 (SM6.Experimental)）** 选项，还需要兼容的显卡）。
- [体积云](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/volumetric-cloud-component-in-unreal-engine)，带有外观自然的材质。
- [指数高度雾](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/exponential-height-fog-in-unreal-engine)。
- 星星（请注意，这些仅用于美化目的，并不能准确表示给定现实世界位置的真实星星定位）。
- 带有对应人眼视觉的 **曝光（Exposure）** 设置的全局后期处理体积。
- [地理配准](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/georeferencing-a-level-in-unreal-engine)Actor，用于定位地球上的环境。

> SunSky和地理配准Actor中UE原点的地理位置已设置为73W, 45N。你必须根据实际环境位置酌情调整。

该模板还随附自定义 `BP_SimGameMode` 蓝图，它定义了特定 `BP_SimPlayerController` 和 `BP_SimfloatingPawn` 。这些蓝图示例说明了如何增强Controller和Pawn基类的默认功能，详见下文。

#### 3.5.1.模拟玩家控制器（BP_SimPlayerController）

该控制器随附一些快捷键，用于在运行时允许以下玩家操作：

- 使用运行之时生成的浮动Pawn自由寻路（ `BP_SimfloatingPawn` ）。
- 在此浮动Pawn和关卡中已存在的Pawn之间交替。
- 控制当日时间。
- 显示分析和统计数据控件。
- 显示地理空间位置状态栏。

以下键盘快捷键可供使用：

| **键**           | **操作**                                                     |
| ---------------- | ------------------------------------------------------------ |
| Pawn功能按钮     |                                                              |
| **Enter**        | 在浮动Pawn和预先存在的关卡Pawn之间交替。                     |
| **Tab**          | 控制关卡Pawn时，切换到下一个可控制的Pawn。                   |
| **Shift + Tab**  | 控制关卡Pawn时，切换到上一个可控制的Pawn。                   |
| **1 - 6**        | 用于控制特定关卡Pawn的直接快捷键。如果数量超过6个，请使用 **Tab** 键。 |
| 当日时间功能按钮 |                                                              |
| **End**          | 减少当前的当日时间。                                         |
| **Page Down**    | 增加当前的当日时间。                                         |
| **Insert**       | 将当日时间平滑过渡到黎明值。                                 |
| **Home**         | 将当日时间平滑过渡到中午值。                                 |
| **Page Up**      | 将当日时间平滑过渡到傍晚值。                                 |
| 控件功能按钮     |                                                              |
| **P**            | 显示/隐藏分析控件。                                          |
| **G**            | 显示/隐藏地理空间控件。                                      |

##### 3.5.1.1地理空间控件

[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\geospatial-widget.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/1d477ef7-1bc9-4443-ad3c-c669ded0300d/geospatial-widget.png)

**地理空间控件（Geospatial Widget）** 是在不同坐标系中显示你在地球上的当前位置的状态栏：

- 投影CRS。
- 地理CRS（纬度/经度）。
- 地心（ECEF）。

如需更多信息，请参阅[关卡地理配准](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/georeferencing-a-level-in-unreal-engine)页面。

##### 3.5.1.2.分析控件

[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\profiling-widget.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/55aac68f-6c04-4c9c-8362-44ae706039f0/profiling-widget.png)

**分析控件（Profiling Widget）** 是用于分析应用程序性能的调试工具。

左侧按钮堆栈将显示或隐藏不同的性能计数器，你也可以通过关联的 `stat counterName` 控制台命令访问这些计数器。控件显示了最常见、最有用的计数器：

- FPS
- Unit
- Engine
- SceneRendering
- Game
- GPU

由于分析与每秒帧数（FPS）密切相关，你可以在第二列按钮中启用或禁用垂直同步（VSync），或根据需要将FPS限制为30或60FPS。

#### 3.5.2.模拟浮动Pawn（BP_SimfloatingPawn）

模拟浮动Pawn是虚幻引擎默认Pawn的改进版本，增加了使用 **鼠标滚轮** 控制最大寻路速度的功能。这有助于处理大型环境。

**点击** 鼠标滚轮将重置为默认速度。



## 4.升级项目以便兼容新的编辑器版本(略)

## 5.恢复中心

此插件可在编辑器崩溃或异常退出后帮助恢复虚幻引擎会话。

**恢复中心（Recovery Hub）** 是一个虚幻引擎插件，可在编辑器崩溃或异常退出后帮助恢复引擎会话。在虚幻引擎4中，此插件名为"灾难恢复（Disaster Recovery）"。

默认情况下不启用恢复中心插件。必须先[启用该插件](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/working-with-plugins-in-unreal-engine)后才能使用。

如果使用的资产大于2GB，恢复中心在记录每个操作时将占用大量磁盘空间。如果磁盘空间开始变得不足，应暂时禁用该系统。为此，请在[项目设置（Project Settings）](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/project-settings-in-unreal-engine)窗口的 **插件（Plugins）> 恢复中心（Recovery Hub）** 分段中禁用 **启用（Is Enabled）** 选项。

### 5.1.恢复中心的工作原理

当编辑器启动时，灾难恢复会自动检查上次会话是否异常结束。如果是，编辑器将检索以前记录的操作列表，并提供重新运行这些操作的选项。可选择重新运行部分或全部的操作，以帮助恢复上次编辑器会话崩溃时可能丢失的工作。

恢复中心将对Actor或资产的每项更改作为 **操作** 进行读取，并维护近期操作的列表。如果编辑器崩溃，可将项目回滚到上一个操作以恢复所有丢失的工作。

由于恢复中心仅支持关卡编辑和Sequencer，因此它与自动保存文件配合使用的效果最佳，且其初衷并非替代自动保存功能。每次保存和自动保存都计为恢复中心内的一个操作。

请在[编辑器偏好设置（Editor Preferences）](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/unreal-editor-preferences)的 **通用（General）> 加载和保存（Saving & Loading）** 分段中启用 **自动保存（Autosave）**。

### 5.2.恢复中心界面

[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\ue5_1-recovery-hub-ui.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/dd411ea2-f08b-441a-8800-6b6202455437/ue5_1-recovery-hub-ui.png)

"恢复中心（Recovery Hub）"窗口包含以下区域：

| **编号** | **名称**                        | **描述**                                                     |
| -------- | ------------------------------- | ------------------------------------------------------------ |
| 1        | **主工具栏**                    | 包含两个按钮：**导入（Import）**：导入 `.json` 格式的崩溃数据转储。**删除（Delete）**：删除当前选定会话。 |
| 2        | **会话（Sessions）** 面板       | 显示已保存会话的列表。                                       |
| 3        | **配置（Configurations）** 按钮 | 单击此按钮可在"项目设置（Project Settings）"中打开恢复中心插件设置。 |
| 4        | 会话细节                        | 显示当前选定会话的操作列表。                                 |

### 5.3.恢复会话

要在崩溃后恢复虚幻编辑器会话，请执行以下步骤：

1. 打开恢复中心。从主菜单转到 **工具（Tools）> 恢复中心（Recovery Hub）**。
2. 在 **会话（Sessions）** 面板中，选择要恢复的会话。
3. 单击 **全部恢复（Recover All）**。在编辑器崩溃后会出现此按钮。

### 5.4.删除会话

如果要释放磁盘空间，可删除不再需要的早期恢复中心会话。请按照以下步骤执行此操作：

1. 打开恢复中心。从主菜单转到 **工具（Tools）> 恢复中心（Recovery Hub）**。
2. 在 **会话（Sessions）** 面板中，选择要删除的会话。
3. 单击 **删除（Delete）** 按钮。



## 6.创建自定义模板

将已有的项目转换为模板所需的步骤

虚幻引擎的模板可以提供一个制作项目更好的起始点。你可以使用它们来快速地针对某个平台开始开发或者创建特别项目，比如多屏幕体验。

使用虚幻引擎时，你可以使用已有的项目创建 **自定义模板（custom templates）** 来达到你的各种需求。

自定义模板是一个虚幻引擎项目，设置为在创建新项目时作为模板和其它的模板一起在引擎中显示。

自定义模板可以包含内容、设置和代码，并且可以设置默认启用或禁用指定的插件。

### 6.1.步骤

在以下教程中，[ProjectName] 代表你的虚幻引擎项目名（比如 `MyProjectName.uproject` ）。这与 `DefaultGame.ini` 文件中的变量 **ProjectName** 不同（没有方括号）。

要将已有的项目转换为模板：

1. 将 **整个** 项目文件夹复制到你的引擎安装目录的 `Templates` 文件夹啊。如果你从Epic Games启动器安装了虚幻引擎，那么 `Templates` 文件夹会位于：

	- Windows系统： `C:\Program Files\Epic Games\UE_[version]\Templates`
	- Mac： `/Users/Shared/Epic Games/UE_[version]/Templates`

	如果你从源代码编译了虚幻引擎，那么 `Templates` 文件夹会位于 `[ForkLocation]\UE4\Templates` 。

2. 打开 `[ProjectName]\Config\DefaultGame.ini 文件` 。然后添加或更新 **ProjectName** 变量。这是在创建新项目时显示在模板选择区域内的名称。

	示例：

	```cpp
	     [/Script/EngineSettings.GeneralProjectSettings]
	     ProjectID=E6468D0243A591234122E38F92DB28F4
	     ProjectName=MyTestTemplate
	```

	注意 **ProjectID** 变量是为每一个项目生成的一个独特的ID。

3. 在你的虚幻引擎安装目录中，找到 `Templates\TP_FirstPerson\Config\` 。将 `TemplateDefs.ini` 文件复制到 `[ProjectName]\Config` 文件夹。

	除了 `TP_FirstPerson` 以外，你还可以使用任何已有的模板文件夹，只要其中包含一个 `TemplateDefs.ini` 文件即可。

4. 打开上一步复制的 `TemplateDefs.ini` 文件并且更新 **LocalizedDisplayNames** 和 **LocalizedDescriptions** 变量。一共有四组变量，每组对应一个虚幻引擎支持的语言：英文 (en)、韩文 (ko)、日文 (ja) 以及简体中文 (zh-Hans)。

	示例：

	```cpp
	         [/Script/GameProjectGeneration.TemplateProjectDefs]
	         LocalizedDisplayNames=(Language="en",Text="My Test Template")
	         LocalizedDescriptions=(Language="en",Text="This is a custom template that includes a first-person character and uses Blueprint.")
	```

5. 当你创建新项目时，你的模板会在 `TemplateDefs.ini` 文件中定义的类别里出现。这由 **Categories** 变量所控制。不管变量名称是什么，一个模板只能分配 **一个** 类别。

	可以使用的类别有：

	- **Games** - 游戏
	- **ME** - 电影、电视和现场活动
	- **AEC** - 建筑、工程和建造
	- **MFG** - 汽车、产品设计和生产

	更多信息可以参考 `[虚幻引擎安装目录]\UE_[版本]\Templates` 文件夹下的 `TemplateCategories.ini` 文件。

6. 你可以在 `[ProjectName]\Media` 文件夹中添加一个图标和预览图。这些图片必须为PNG格式并且满足以下命名要求：

	- 图标： `[ProjectName].png`.
	- 预览图： `[ProjectName]_Preview.png`.

### 6.2.最终结果

现在你应该可以在新项目对话框中看到新的模板。

![示例中虚幻项目浏览器中有一个名为My Test Template的新的自定义模板。](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(05)：使用项目和模板.assets\custom-template.png)

*示例中虚幻项目浏览器中有一个名为My Test Template的新的自定义模板。*

要查看新的模板，仅需关闭并重新打开新项目窗口。然而，如果对已有的模板进行了任何更改（更改名称或描述），就必须重启虚幻引擎来让窗口中显示这些变动。

