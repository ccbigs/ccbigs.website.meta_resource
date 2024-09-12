# UnrealEngine学习(02)：基础知识

## 1.虚幻编辑器界面

学习一款软件，我个人建议是先学习怎么用，然后是学习怎么用的好，再研究源码。

上一篇文章详细描述了我们该如何安装虚幻5引擎：

[UnrealEngine学习(01)：安装虚幻引擎![img](.\UE学习(02)：基础知识.assets\icon-default.png)https://blog.csdn.net/zuodingquan666/article/details/141539385](https://blog.csdn.net/zuodingquan666/article/details/141539385)

这一篇文章我们先来了解虚幻5编辑器的界面：

![img](.\UE学习(02)：基础知识.assets\ba3baf2ea1574473854dec65c55c8366.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)我们点击创建，项目的路径要选好哦：

![img](.\UE学习(02)：基础知识.assets\f1246091a1ff4bb1a3d530e18c1d5cd7.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)对于初学者来说，我们可以勾选初学者内容包：

![img](.\UE学习(02)：基础知识.assets\f80188902fa14dc38320b6560c725683.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)点击创建后，我们进入到如下界面：

![img](.\UE学习(02)：基础知识.assets\6ab539710f554d43bfe9b90d2e617f9a.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)UE官方将上图划分为七大部分，个人觉得很合理，该图如下：

![img](.\UE学习(02)：基础知识.assets\8f5745956c7154189ae44a4e378a82f0.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)每个部分的名称与说明如下：

| **编号** | **名称**                                | **说明**                                                     |
| -------- | --------------------------------------- | ------------------------------------------------------------ |
| 1        | **菜单栏（Menu Bar）**                  | 使用这些菜单访问编辑器专用的命令和功能。                     |
| 2        | **主工具栏（Main Toolbar）**            | 包含虚幻引擎中部分最常用工具和编辑器的快捷方式，以及用于进入 **播放（Play）** 模式（在虚幻编辑其中运行游戏）和用于将项目部署到其他平台的快捷方式。 |
| 3        | **关卡视口（Level Viewport）**          | 显示关卡的内容，例如摄像机、Actor、静态网格体等。            |
| 4        | **内容侧滑菜单（Content Drawer）** 按钮 | 打开 **内容侧滑菜单（Content Drawer）**，可以在其中访问项目中的所有资产。 |
| 5        | **底部菜单栏（Bottom Toolbar）**        | 包含命令控制台、输出日志和派生数据功能的快捷方式。此外还显示源控制状态。 |
| 6        | **大纲（Outliner）**                    | 显示关卡中所有内容的分层树状图。                             |
| 7        | **细节（Details）** 面板                | 在选择Actor时显示。显示该Actor的各种属性，例如 **变换（Transform）** （在关卡中的位置）、静态网格体、材质和物理设置。此面板显示不同设置，具体取决于你在关卡视口中选择的内容。 |

### 1.1.菜单栏

![img](.\UE学习(02)：基础知识.assets\059b7563c89c4296823622e0abf8a268.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)

第一个菜单栏不用多说，一般用于编辑器的文件创建，编辑器选项设置等等。开始不用多记，用多了就知道了。



### 1.2.主工具栏

虚幻编辑器中常用的工具和命令的快捷方式：

![img](.\UE学习(02)：基础知识.assets\3b90419855e14d71b92e207307ccfff0.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)

#### 1.2.1.保存按钮

![img](.\UE学习(02)：基础知识.assets\8903dbef85ea44968c2a53c85c2db23f.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)点击此按钮即可保存当前打开的关卡。

#### 1.2.2.模式选择

![img](.\UE学习(02)：基础知识.assets\02b97c5038944c81a0ea5f38c19cce55.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)包含的快捷方式用于在不同的模式之间快速切换，以编辑关卡中的内容：

- 选择编辑
- 地形编辑
- 植被编辑
- 网格体绘制
- 破裂编辑
- 笔刷编辑

#### 1.2.3.内容快捷方式

![img](.\UE学习(02)：基础知识.assets\35d8dd1a5e9941fdaff260d8ec5a33c9.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

包含用于添加和打开关卡编辑器中常见内容类型的快捷方式。

| **快捷方式（Shortcut）**   | **说明（Description）**                                      |
| -------------------------- | ------------------------------------------------------------ |
| **创建（Create）**         | 从常见资产列表中进行选择，以快速添加到关卡。此外还可以在此菜单中访问 **放置Actor（Place Actors）** 面板。 |
| **蓝图（Blueprints）**     | 创建和访问蓝图。                                             |
| **过场动画（Cinematics）** | 创建关卡序列或主序列过场动画。                               |

#### 1.2.4.播放模式控制

![img](.\UE学习(02)：基础知识.assets\b70f4241d1b446e2ad57b1f0501c1279.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)包含用于在编辑器中运行游戏的快捷方式按钮（播放、跳过、停止和弹出）。

#### 1.2.5.平台菜单

![img](.\UE学习(02)：基础知识.assets\1d92ad0aba4144328f32cffd08c60946.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)包含一系列选项，可以用于配置、准备项目并将其部署到不同的平台，例如台式机、台式设备或主机。

#### 1.2.6.设置

![img](.\UE学习(02)：基础知识.assets\a653482b48024a74a163cf2f7e623c8d.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑

包含虚幻编辑器、关卡编辑器视口和游戏行为的各种设置。



### 1.3. 关卡视口

**关卡视口（Level Viewport）** 显示当前打开的关卡的内容。在虚幻引擎中打开项目时，项目的默认关卡默认在关卡视口中打开。在这里可以查看和编辑活跃关卡的内容，无论是在游戏环境中、产品可视化应用中还是其他位置。

关卡视口通常以两种不同的方式显示关卡的内容：

- **视角（Perspective）** ，这是3D视图，可以从不同角度在视图中查看视口的内容。
- **直角（Ortographic）** ，这是2D视图，沿着一个主轴（X、Y或Z）俯视。

![img](.\UE学习(02)：基础知识.assets\4b870a9db9644302b4c310f7fb899d95.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)

### 1.4.内容侧滑菜单/内容浏览器

​    **内容浏览器（Content Browser）** 是文件浏览器窗口，可以显示项目中包含的所有资产、蓝图和其他文件。可以使用内容浏览器来浏览内容、将资产拖动到关卡中、在项目之间迁移资产以及执行其他操作。

![img](.\UE学习(02)：基础知识.assets\803826577e8a454d81231a4ce838493e.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)	**内容侧滑菜单（Content Drawer）** 按钮位于虚幻编辑器的左下角，可以打开内容浏览器的一个特殊实例，该实例在非焦点状态下时（即点击其他位置后）就会自动最小化。要使该实例处于打开状态，请点击内容侧滑菜单右上角的 **停靠在布局中（Dock in Layout）** 按钮。这会创建内容浏览器的新实例，但你仍然可以打开新的内容侧滑菜单（Content Drawer）。

### 1.5.底部工具栏

底部菜单栏包含命令控制台、输出日志和派生数据功能的快捷方式。此外还显示源控制状态。其中包含以下几个区域：

![img](.\UE学习(02)：基础知识.assets\e61f5c0ed2a547d3940694c11945d597.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)

| **编号** | **名称**                                | **说明**                                                     |
| -------- | --------------------------------------- | ------------------------------------------------------------ |
| 1        | **输出日志（Output Log）**              | 用于在应用程序运行时输出有用信息的调试工具。                 |
| 2        | **命令控制台（Command Console）**       | 与任何其他命令行界面行为相同：输入控制台命令即可触发特定的编辑器行为。 			键入 `help` 并按 **Enter** 键即可在浏览器中打开可用控制台的列表。 |
| 3        | **派生数据（Derived Data）**            | 提供[派生数据](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/derived-data-settings-in-the-unreal-engine-project-settings)功能。 |
| 4        | **源控制状态（Source Control Status）** | 如果项目连接到源控制（例如GitHub或Perforce），则显示源控制状态。否则，将提示 *源控制关闭*。 |

### 1.6.大纲

​	**大纲（Outliner）** 面板（以前称为"世界大纲视图"）显示关卡中所有内容的分层视图。默认情况下，此面板位于虚幻编辑器窗口的右上角。你可以最多打开四个不同的大纲界面。每个大纲的布局和过滤设置都可以不一样。

![img](.\UE学习(02)：基础知识.assets\aa2f714e0ed945798f137d25db74ebaf.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)此外，还可以使用大纲面板执行以下操作：

- 通过点击关联的 **眼睛（Eye）** 按钮，快速隐藏或显示Actor。
- 右键点击该Actor即可访问Actor的 **上下文菜单（context menu）** 。然后，可以从该菜单中执行其他特定于Actor的操作。
- 创建、移动和删除内容文件夹。

### 1.7.细节面板

在关卡视口中选择一个Actor之后，**细节（Details）** 面板将会显示影响所选Actor的设置和属性。默认情况下，该面板位于虚幻编辑器窗口右侧的 **世界大纲视图（World Outliner）** 面板下。

![img](.\UE学习(02)：基础知识.assets\e1484378339540dfbbdb60028cce2c7d.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)

### 1.8.总结

好了，以上就是UE界面的整体布局和解释。个人认为基本上懂得各个选项的含义和功能就OK了，主要还是要多做，多动手。



## 2.虚幻引擎术语

### 2.1.项目

**虚幻引擎5项目（Unreal Engine 5 Project）** 中包含游戏的所有内容。项目中包含的大量文件夹都在磁盘上，例如 `Blueprints` 和 `Materials` 。你可以按照自己的意愿命名文件夹并将其整理到项目中。**虚幻编辑器（Unreal Editor）** 中的 **内容浏览器（Content Browser）** 面板显示与磁盘上的 `Project` 文件夹相同的目录结构。

每个项目都有与其关联的 `.uproject` 文件。`.uproject` 文件是创建、打开或保存项目的方法。你可以创建任意数量的不同项目，然后并行处理它们。

![img](.\UE学习(02)：基础知识.assets\68cc63fae29d429f886e18b30dbb0ab9.png)![点击并拖拽以移动](data:image/gif;base64,R0lGODlhAQABAPABAP///wAAACH5BAEKAAAALAAAAAABAAEAAAICRAEAOw==)编辑



### 2.2.蓝图

**蓝图视觉效果脚本（Blueprint Visual Scripting）** 系统是完善的gameplay脚本系统，在虚幻编辑器中使用基于节点的界面来创建gameplay元素。就像许多常用的脚本编写语言，它可以用于在引擎中定义以object为导向（OO）的类或object。在使用虚幻引擎时，经常会发现使用蓝图定义的object被统称为"蓝图"。



### 2.3.对象

**Object** 是虚幻引擎中最基本的类——换而言之，它们就像建造系统的砖块，包含资产的大量基本功能。虚幻引擎中的几乎所有功能都继承自object（或使用其中的部分功能）。

在C++中，`UObject` 是所有object的基类，可以实施多种功能，例如垃圾回收、用于将变量提供给虚幻编辑器的元数据（`UProperty`）支持以及用于加载和保存的序列化。



### 2.4.类

**类（Class）** 定义虚幻引擎中特定Actor或Object的行为和属性。类是分层的，意味着类从其父类（即派生出类的类，或"子类"的来源）中继承信息并将该信息传递给其子项。可以在C++代码或蓝图中创建类。



### 2.5.Actor

**Actor** 是可以放到关卡中的任何object，例如摄像机、静态网格体或玩家出生点位置。Actor支持3D变换，例如转换、旋转和缩放。可以通过gameplay代码（C++或蓝图）创建（生成）或销毁Actor。

在C++中，`AActor` 是所有Actor的基类。



### 2.6.类型转换

**类型转换（Casting）** 是一种动作，将会提取特定类的Actor并尝试将其作为其他类进行处理。类型转换可能成功，也可能失败。如果类型转换成功，则可以在你类型转换到的Actor上访问特定于类的功能。

例如，如果你要制作一款游戏，在其中具有能够以不同方式影响玩家角色的多种体积类型。其中一个体积是 **火焰（Fire）**，可以随着时间降低玩家血量。当角色与关卡中的任何体积重叠时，就可以将该体积 **类型转换（Cast）** 到 **火焰（Fire）** 上，以尝试访问其"损害玩家血量"功能。

- 如果类型转换成功——即如果玩家站在火中——玩家的血量将开始下降。
- 如果类型转换失败——即如果玩家站在任何其他类型的体积中——其血量将不受影响。

类型转换不同于简单地检查Actor是否是给定的类，它将返回一个二选一的答案（是或否），但不允许你与该类的任何特定功能进行交互。

### 2.7.组件

**组件（Component）** 是一种可以添加到Actor的功能。

将组件添加到Actor时，Actor可以使用组件提供的功能。例如：

- 点光源组件将使Actor像点光源一样发光。
- 旋转移动组件将使Actor转动。
- 音频组件将使Actor能够播放音效。

组件必须连接到Actor，不能独自存在。



### 2.8.Pawn

**Pawn** 是Actor的子类，作为游戏内的形象或人像（例如游戏中的角色）。玩家或游戏的AI可以控制Pawn，将其作为非玩家角色（NPC）。

当人类或AI玩家控制Pawn时，会将其视为 *被占有* 。相反，当人类或AI玩家未控制Pawn时，会将其视为 *未被占有* 。



### 2.9.角色

**角色（Character）** 是计划用作玩家角色的Pawn Actor的子类。角色子类包括碰撞设置、双足运动的输入绑定以及用于玩家控制动作的其他代码。



### 2.10.玩家控制器

**玩家控制器（Player Controller）** 获取玩家输入，并将其转换到游戏内的互动中。每个游戏内部都至少具有一个玩家控制器。玩家控制器通常操控一个Pawn或角色作为玩家在游戏中的呈现方式。

玩家控制器还是多人游戏的主要网络互动点。在多人游戏期间，服务器具有游戏中每个玩家的玩家控制器的一个实例，因为它还必须对每个玩家进行网络功能调用。每个客户端都只有一个与玩家对应的玩家控制器，并且只能使用其玩家控制器与服务器进行通信。

关联的C++类是 `PlayerController` 。



### 2.11.AI控制器

就像玩家控制器操控Pawn作为玩家在游戏中的呈现方式，**AI控制器（AI Controller）** 操控Pawn在游戏中呈现非玩家角色（NPC）。默认情况下，Pawn和角色都以基本AI控制器终结，除非它们被玩家控制器专门操控或者收到指令不允许为自己创建AI控制器。

关联的C++类是 `AIController` 。



### 2.12.玩家状态

**玩家状态（Player State）** 是游戏参与者在游戏中的状态，例如人类玩家或模拟玩家的机器人。非玩家AI作为游戏世界的一部分而存在，没有玩家状态。

玩家状态可能包含的玩家信息示例包括：

- 名称
- 当前级别
- 血量
- 得分
- 它们当前是否在"夺旗"游戏中扛旗。

对于多人游戏，所有玩家的玩家状态都在所有机器中存在，可以将数据从游戏中复制到客户端以保持内容一致。这不同于玩家控制器，因为玩家控制器仅存在于玩家所使用的机器上。

关联的C++类是 `PlayerState`。



### 2.13.游戏模式

**游戏模式（Game Mode）** 设置要运行的游戏的规则。这些规则可以包括：

- 玩家如何加入游戏。
- 游戏是否可以暂停。
- 任何游戏特定行为，例如获胜条件。

可以在[项目设置](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/project-settings-in-unreal-engine)中设置默认游戏模式，并针对不同的关卡重载游戏模式。无论你选择以何种方式实施，每个关卡都只能有一个游戏模式。

在多人游戏中，游戏模式新存在于服务器上，而规则将复制（发送）到每个连接的客户端。

关联的C++类是 `GameMode`。



### 2.14.游戏状态

**游戏状态（Game State）** 是一个容器，包含你要在游戏中复制到每个客户端的信息。简而言之，它是每个连接的人的"游戏状态"。

游戏状态可能包含的内容示例包括：

- 与游戏得分相关的信息。
- 比赛是否开始。
- 根据世界中的玩家数量确定生成AI角色的数量。

对于多人游戏，每个玩家的机器上都有一个本地游戏状态实例。本地游戏状态实例从游戏状态的服务器实例获取更新的信息。

关联的C++类是 `GameState`。



### 2.15.笔刷

**笔刷（Brush）** 是用于描述3D形状的Actor，例如立方体或球体。可以将笔刷放置在关卡中以定义关卡几何体（这些几何体称为二进制空间分区或BSP笔刷）。例如，如果要快速封锁关卡，此功能非常有用。



### 2.16.体积

**体积（Volumes）** 是带有边界的3D空间，根据连接到体积的效果，具有不同的使用方法。例如：

- **阻挡体积（Blocking Volumes）** 是可见的，用于阻止Actor通过它们。
- **施加伤害体积（Pain Causing Volume）** 对与其重叠的任何Actor造成持续伤害。
- **触发器体积（Trigger Volumes）** 的编程方式为，在Actor进入或退出体积时触发事件。



### 2.17.关卡

**关卡（Level）** 是你定义的gameplay区域。关卡包含玩家可以看到并与其交互的所有内容，例如几何体、Pawn和Actor。

虚幻引擎将每个关卡保存为单独的 `.umap` 文件，这也是为什么你在某些情况下会看到它们被称为 **地图（Maps）** 。



### 2.18.世界

**世界（World）** 是构成游戏的所有关卡的容器。它处理关卡的流送和动态Actor的生成（创建）。



## 3.工具和编辑器

**虚幻引擎5** 提供了 **工具** 、 **编辑器** 和 **系统** 组合，供你用于创建游戏或应用程序。

本页使用以下术语：

- **工具** 即你用来执行特定任务的用具，如在关卡中放置Actor，或绘制地形。
- 编辑器 **即你用来实现更复杂目标的工具集合。例如，**关卡编辑器**可让你构建游戏关卡，或者你可以在**材质编辑器中改变材料的外观体验。
- **系统** 是功能大合集，这些功能会协同产生游戏或应用程序各方面内容。例如， **蓝图** 是用于视觉化脚本Gameplay元素的系统。

有时，系统和编辑器可能有类似的名称。例如，材质编辑器用于编辑材质资产，而材质系统为在虚幻引擎中使用材质提供底层支持。

虚幻引擎中的部分工具和编辑器是内置的，而其他工具和编辑器则是可选的 **插件（plugins）** ，这些插件可以根据项目需求来启用或禁用。要详细了解插件，请参考[使用插件](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/working-with-plugins-in-unreal-engine)页面。

本页概述了你将在虚幻引擎5中使用的主要工具和编辑器。功能说明文档中涵盖了各种虚幻引擎工具的详细使用说明。

无论你使用 **蓝图编辑器** 为关卡中的Actor编写行为脚本，还是使用 **Niagara编辑器** 创建粒子效果，了解每个编辑器的用途以及导航方法，均能优化你的工作流程，从而帮助你在开发过程中避开绊脚石。

### 3.01.关卡编辑器

**Gameplay关卡:**

**关卡编辑器** 是你构建Gameplay关卡的主要编辑器。在这里通过添加不同类型的[Actor和几何体](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/actors-and-geometry-in-unreal-engine)、[蓝图可视化脚本](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/blueprints-visual-scripting-in-unreal-engine)、[Niagara](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/overview-of-niagara-effects-for-unreal-engine)等来定义播放空间。在默认情况下，当你创建或打开项目时，虚幻引擎5会打开关卡编辑器。

如需了解更多信息，请参阅[关卡编辑器](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/level-editor-in-unreal-engine)。

### 3.02.静态网格体编辑器

**静态网格体:**

可以使用 **静态网格体编辑器（Static Mesh Editor）** 来预览外观、碰撞和UV贴图，以及设置和操控[静态网格体](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/static-mesh-actors-in-unreal-engine)。在静态网格编辑器中，你也可以针对你的静态网格体资产设置[LOD](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/creating-and-using-lods-in-unreal-engine)（或细节级别设置），以根据你的游戏运行方式和地点控制静态网格体资产出现的简洁程度或详细程度。

如需更多信息，请参阅[静态网格体编辑器UI](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/static-mesh-editor-ui-in-unreal-engine)。

### 3.03.材质编辑器

**材质:**

**材质编辑器** 是你创建和编辑材质的地方。材质是可应用于网格体以控制其视觉效果的资产。例如，你可以创建污垢材质，并将其应用到关卡中的各个地板上，从而创建看似有污垢覆盖的表面。

如需了解详细信息，请参阅[材质编辑器参考](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/unreal-engine-material-editor-user-guide)。

### 3.04.蓝图编辑器

**蓝图:**

[![img](.\UE学习(02)：基础知识.assets\ue5-blueprint-editor.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/fc510fe1-1c7d-4acc-99d2-2d82e86e8b6f/ue5-blueprint-editor.png)

**蓝图编辑器** 是你使用和修改蓝图的地方。这些特殊资产可用来创建Gameplay元素（如控制Actor或对事件编写脚本），修改材质或执行其他虚幻引擎功能，省去编写任何C++代码的过程。

如需更多信息，请参阅[蓝图编辑器参考](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/user-interface-reference-for-the-blueprints-visual-scripting-editor-in-unreal-engine)。

### 3.05.物理资源编辑器

**物理:**

你可以使用 **物理资产编辑器** 创建物理资产，以配合[骨骼网格体](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/skeletal-mesh-assets-in-unreal-engine)使用。在实践中，你可以使用此方法实现变形和碰撞等物理特性。你可以从零开始，构建完整的布娃娃设置，或使用自动化工具来创建一套基本物理形体和物理约束。

如需更多信息，请参阅[物理资产编辑器](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/physics-asset-editor-in-unreal-engine)。

### 3.06.行为树编辑器

**AI行为:**

**行为树编辑器** 是你通过一种可视化的基于节点脚本系统（类似于蓝图）为关卡中的Actor编写人工智能（AI）脚本的地方。你可以为敌人、非游戏角色（NPC）、载具等创建任意数量的不同行为。

如需更多信息，请参阅[行为树用户指南](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/behavior-tree-in-unreal-engine---user-guide)。

### 3.07.Niagara编辑器

**粒子效果:**

**Niagara编辑器** 利用由分离粒子发射器组成的全套模块化粒子效果系统，为每个效果创建特殊效果。可将发射器保在内容浏览器中，以备后用，并将作为当前和未来项目中的新发射器基础使用。

如需了解详细信息，请参阅[Niagara关键概念](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/key-concepts-in-niagara-effects-for-unreal-engine)。

### 3.08.UMG界面编辑器

**用户界面:**

**虚幻示意图形UI编辑器** 是视觉UI创作工具，可用来创建UI元素，如在游戏内头顶显示、菜单或其他界面相关的图形。

如需更多信息，请参阅[UMG UI设计器用户指南](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/umg-ui-designer-quick-start-guide-in-unreal-engine)。

### 3.09.字体编辑器

**字体:**

使用 **字体编辑器** 添加、组织和预览字体资产。你也可以定义字体参数，如字体资产布局和提示策略（*字体提示*是一种数学方法，可确保文本在任意尺寸的显示屏中都可读）。

如需更多信息，请参阅 [字体资源和编辑器](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/font-asset-and-editor-in-unreal-engine)。

### 3.10.Sequencer编辑器

**过场动画和动态事件:**

[![img](.\UE学习(02)：基础知识.assets\ue4-sequencer-meerkat.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/40f0f1f0-5f7d-4353-a989-57b54dd8a23e/ue4-sequencer-meerkat.png)



在制作Weta Digital动画短片猫鼬的过程中使用了Sequencer。点击查看完整视图。

利用 **Sequencer编辑器** 可通过专用多轨迹编辑器创建游戏过场动画。通过创建 **关卡序列（Level Sequences）** 和添加 **轨迹** （Tracks），你可以定义各个轨迹的组成，这样将确定场景的内容。轨迹可以包含动画（Animation）（用于将角色动画化）、变形（Transformation）（在场景中移动各个东西）、音频（Audio）（用于包括音乐或音效）等等。

如需了解更多信息，请参阅[Sequencer概述](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/unreal-engine-sequencer-movie-tool-overview)。

### 3.11.动画编辑器

**动画:**

**动画编辑器** 是虚幻引擎5中的动画编辑器。你可以使用该工具来编辑[骨骼资产](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/skeletons-in-unreal-engine)、[骨骼网格体](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/skeletal-mesh-assets-in-unreal-engine)、[动画蓝图](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/animation-blueprints-in-unreal-engine)，以及其他各种动画资产。

如需更多信息，请参阅[动画编辑器](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/animation-editors-in-unreal-engine)。

### 3.12.Control Rig编辑器

**动画:**

**Control Rig** 是动画工具套件，可以用于直接在引擎中操纵角色并实现其动画。使用Control Rig，你无需在外部工具中进行操纵和制作动画，而是直接在虚幻编辑器中制作动画。使用此系统，你可以在角色上创建和操纵自定义控制点，在 [Sequencer](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/cinematics-and-movie-making-in-unreal-engine) 中制作动画，并使用各种其他动画工具来帮助完成动画制作过程。

如需了解更多信息，请参阅[Control Rig](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/control-rig-in-unreal-engine)。

### 3.13.Sound Cue编辑器

**Sound Cue:**

虚幻引擎5中的音频播放的行为在Sound Cue中得到定义，可使用 **Sound Cue编辑器** 对其进行编辑。在此编辑器中，你可以组合多个声音资产后混音，以此生成单混音输出，另存为一个Sound Cue。

如需了解更多信息，请参阅[Sound Cue编辑器](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/sound-cue-editor-in-unreal-engine)。

### 3.14.媒体编辑器

**外部媒体播放:**

使用 **媒体编辑器** 来定义媒体文件或URL，以作为虚幻引擎5内部播放的源媒体使用。

你可以定义源媒体播放方式设置，如自动播放、播放速度和循环，但不能直接编辑媒体。

如需了解更多信息，请参阅[媒体编辑器参考文档](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/media-editor-reference-for-unreal-engine)。

### 3.15.nDisplay 3D配置编辑器

**虚拟制作和实时事件:**

[nDisplay](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/rendering-to-multiple-displays-with-ndisplay-in-unreal-engine)在多个同步显示设备上渲染虚幻引擎场景，如能量墙、穹顶和曲面界面。你可以使用 **nDisplay配置编辑器** 创建nDisplay设置，并使所有显示设备上的内容渲染方式可视化。

如需了解更多信息，请参阅[nDisplay 3D配置编辑器](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/ndisplay-3d-config-editor-in-unreal-engine)。

### 3.16.DMX库编辑器

**实时事件:**

[![img](.\UE学习(02)：基础知识.assets\ue4-dmx-library-editor.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/ed3ef52f-5510-4a20-a6cc-488294a499b0/ue4-dmx-library-editor.png)

DMX实操。此截图来自Moment Factory的示例项目。点击查看完整视图。

**DMX（数字多路复用）** 是在整个实时事件行业中用来控制各种设备的数字通信标准，如照明灯具、激光、烟雾机、机械设备和电子广告牌。在 **DMX库编辑器** 中，你可以自定义相关设备及其命令。

如需了解更多信息，请参阅[DMX](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/dmx-in-unreal-engine)。





## 4.坐标空间术语

| 虚幻中的空间                        | 其他名称                                                     | 描述                                                         |
| ----------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **切线（Tangent）**                 |                                                              | 正交（可能在插值之后偏离），可以是左旋或右旋。TangentToLocal变换仅包含旋转，因此它是OrthoNormal（可以通过换位反转）。 |
| **局部（Local）**                   | **对象空间（Object Space）**                                 | 正交，可以是左旋或右旋（三角形剔除顺序需要调整）。LocalToWorld变换包含旋转、非等分缩放（包括可能改变缠绕顺序的负非等分缩放）和平移。 |
| **世界场景（World）**               |                                                              | WorldToView变换仅包含旋转和平移，因此视图空间中的距离与世界场景空间中的距离相同。 |
| **平移世界场景（TranslatedWorld）** |                                                              | 世界场景 			平移世界场景 - 预览平移 	    平移世界             世界场景 + 预览平移 		   平移的矩阵用于从组合的变换矩阵中移除摄像机位置，可在变换顶点时提高精度。 |
| **视图（View）**                    | **摄像机空间（CameraSpace）**                                | ViewToClip变换包含x轴和y轴上的缩放，但不包含平移（如果平移的话将会是偏心投影）。它缩放并平移z轴。它还会应用投影来转换为齐次裁剪空间。 |
| **裁剪（Clip）**                    | **齐次坐标（HomogeniousCoordinates）**, **后投影空间（PostProjectionSpace）**, **投影空间（ProjectionSpace）** | 应用透视投影矩阵之后。请注意，裁剪空间中的W与视图空间Z中的相同。 |
| **屏幕（Screen）**                  | OpenGL 中的 **标准化设备坐标（NormalizedDeviceCoordinates）** | 经过透视分割之后： 			 		          左/右 					-1,1 				 上/下 					1,-1 				 近/远 		0,1（OpenGL RHI需要将此变换为-1,1） |
| **视口（Viewport）**                | **视口坐标（ViewportCoordinates）**、**窗口坐标（WindowCoordinates）** | 以像素计： 			 			 			左/右 					0, 宽-1 				 上/下 					0, 高-1 |

### 4.01.空间变换

空间变换应该始终使用 ***X To Y\*** 的命名格式。

**示例：**

- WorldToView
- TranslatedWorldToView
- TangentToWorld



## 5.游戏类被许可用户上手指南（略）



## 6.被许可用户（非游戏类）入门指南（略）



## 7.UE本地文件目录结构

在最高一级目录中，是你的引擎（Engine）目录以及你的所有游戏项目目录。Engine目录包含引擎自身及其随附工具。每个游戏目录都包含与该游戏有关的所有文件。与先前的引擎版本相比，UE4中的引擎和游戏在目录结构上有了更明显的区分。

为了更加直观的了解到UE的目录结构，大家可以打开UE引擎的安装路径，进入UE引擎本地文件的第一层目录如下：

![image-20240826213901604](.\UE学习(02)：基础知识.assets\image-20240826213901604.png)

### 7.01.根目录

![image-20240826213901604](.\UE学习(02)：基础知识.assets\image-20240826213901604.png)

- **Engine** - 包含构成引擎的所有源代码、内容等。
- **Templates** - 创建新项目时可用的项目模板集合。
- **GenerateProjectFiles.bat** - 用于创建在Visual Studio中使用引擎和游戏所需的UE4解决方案和项目文件。请参阅[IDE的项目文件](https://dev.epicgames.com/documentation/zh-cn/unreal-engine/how-to-generate-unreal-engine-project-files-for-your-ide)以了解详细信息。
- **UE4Games.uprojectdirs** - 辅助文件，帮助引擎找到子目录中的项目。

### 7.02.通用目录

![image-20240826214155579](.\UE学习(02)：基础知识.assets\image-20240826214155579.png)

某些子目录在引擎目录和游戏项目目录中都能找到：

- **Binaries** - 包含可执行文件或编译期间创建的其他文件。
- **Build** - 包含编译引擎或游戏所需的文件，包括为某些特定平台创建项目版本时所需的文件。
- **Config** - 配置文件，包含的参数可用于控制引擎的行为。你在游戏项目Config文件中设置的值会覆盖 `Engine\Config` 目录中设置的值。
- **Content** - 保存引擎或游戏中的内容，例如资产包、贴图。
- **DerivedDataCache** - 包含派生数据文件。这类数据专为被引用内容生成，并且在加载时生成。假如被引用内容未生成过缓存文件，则加载时间会显著增加。
- **Intermediate** - 包含编译引擎或游戏时生成的临时文件。在游戏目录中，着色器也保存在Intermediate目录中。
- **Saved** - 包含自动保存文件、配置（`.ini`）文件和日志文件。此外，**Engine > Saved** 目录还包含崩溃日志、硬件信息和Swarm选项与数据。
- Source \- 包含引擎或游戏的所有源文件，包括引擎源代码、工具和游戏类等。
  - Engine \- Engine目录中的源文件组织结构如下：
    - **Developer** - 编辑器和引擎共同使用的文件。
    - **Editor** - 仅供编辑器使用的文件。
    - **Programs** - 引擎或编辑器使用的外部工具。
    - **Runtime** - 仅供引擎使用的文件。
  - Game - 游戏项目目录中的源文件按模块分组，一个模块一个目录。每个模块包含以下内容：
    - **Classes** - 包含所有的头文件（`.h`）。
    - **Private** - 包含所有 `.cpp` 文件，包括游戏逻辑类以及各种模块的实现文件。
    - **Public** - 包含模块的头文件。

### 7.03.引擎专有目录

![image-20240826214625167](.\UE学习(02)：基础知识.assets\image-20240826214625167.png)

部分子目录只存在于Engine目录中。

- Documentation \- 包含引擎文档，包括源文件和发布的文件。
  - **HTML** - 发布的HTML文档文件。
  - **Source** - 源markdown文档文件。
- **Extras** - 其他辅助和工具文件。
- **Plugins** - 包含引擎中使用的插件。
- **Programs** - 包含UE4根目录中各个项目及其他虚幻程序（如UnrealFrontend和UnrealHeaderTool）的配置文件和日志文件。
- **Shaders** - 保存引擎的着色器源文件（`.usf`）。



### 7.04.游戏项目目录

游戏项目目录指的是我们在UE中创建的项目，我们可以在指定的路径上，找到我们创建的文件，例如我的：

![image-20240826214757221](.\UE学习(02)：基础知识.assets\image-20240826214757221.png)

| 目录                      | 说明                                                         |
| ------------------------- | ------------------------------------------------------------ |
| **Binaries**              | 包含可执行文件或编译期间创建的其他文件。                     |
| **Config**                | 游戏的默认项目设置。                                         |
| **Content**               | 包含引擎或游戏的内容，包括资产包和贴图。                     |
| **External dependencies** | 显示公有的引擎头文件（仅在Visual Studio中可见）。            |
| **Intermediate**          | 包含UnrealBuildTool生成的文件，如Visual Studio项目文件。这些文件可以删除并重新构建。 |
| **Saved**                 | 包含引擎生成的文件，如配置文件和日志。这些文件可以删除并重新构建。 |
| **Source**                | 包含游戏模块对象类文件。                                     |

### 7.05.解决方案目录

| 目录                      | 说明                                            |
| ------------------------- | ----------------------------------------------- |
| **Classes**               | 包含游戏对象的类定义（`.h` 文件）。             |
| **Config**                | 游戏的默认项目设置。                            |
| **External dependencies** | 显示公有引擎头文件（仅在Visual Studio中可见）。 |
| **Private**               | 包含私有游戏对象类的实现文件（`.cpp` 文件）。   |
| **Public**                | 包含公有游戏对象类的实现文件（`.cpp` 文件）。   |



## 8.数学基础

​	开发游戏，游戏不像是简单的CRUD，还是需要一定的数学基础，例如：游戏中的角色的移动，我们需要给与它速度，如果是开发模拟类游戏，比如飞机飞行，我们还要给它空气阻力。

虚幻引擎中的许多对象都基于数学结构和选项，可以根据数学运算进行配置和更改。本节概述了您可能会发现有用的数学结构和概念，以及这些结构与虚幻引擎中各种对象和操作之间的联系。

​	虚幻引擎（UE）默认使用以下国际单位制（SI）进行测量：

| 数量      | 单位                 |
| --------- | -------------------- |
| 距离/长度 | 厘米（cm）           |
| 质量      | 公斤（kg）           |
| 时间      | 分钟（min），秒（s） |
| 角        | 度（度）             |
| 速度      | 米/每秒（m/s）       |
| 温度      | 摄氏度（C）          |
| 力        | 牛顿（N）            |
| 扭矩      | 牛顿.米（N•m）       |


有关UE中所有可用单元的更多信息，请参阅下面的可用单元部分。

### 8.01.更改默认单位

您可以在虚幻编辑器中更改项目中这些数量的单位。要更改这些单位，请执行以下步骤：

1. 从菜单栏中，选择编辑>项目设置。。。这将打开一个新的“项目设置”窗口或选项卡。![image-20240827071322188](.\UE学习(02)：基础知识.assets\image-20240827071322188.png)
2. 导航到编辑器>外观。![image-20240827071418982](.\UE学习(02)：基础知识.assets\image-20240827071418982.png)
3. 展开“单元”>“高级”下的类别。![image-20240827071446230](.\UE学习(02)：基础知识.assets\image-20240827071446230.png)
4. 现在，您应该看到所有测量量及其单位。要更改数量，请从要更改的数量旁边的下拉菜单中选择一个新单位。



### 8.02.可用单位

以下部分包含UE中可用的所有测量单位的列表，按测量数量组织：

#### 8.02.01.距离和长度

| **Unit**     | **Abbreviation** |
| ------------ | ---------------- |
| **SI**       |                  |
| Micrometers  | µm               |
| Millimeters  | mm               |
| Centimeters  | cm               |
| Meters       | m                |
| Kilometers   | km               |
| **Imperial** |                  |
| Inches       | in               |
| Feet         | ft               |
| Yards        | yd               |
| Miles        | mi               |
| Lightyear    | ly               |

#### 8.02.02.Velocity and Speed(速度)

| **Unit**               | **Abbreviation** |
| ---------------------- | ---------------- |
| **SI**                 |                  |
| Centimeters Per Second | cm/s             |
| Meters Per Second      | m/s              |
| Kilometers Per Second  | km/s             |
| **Imperial**           |                  |
| Miles Per Hour         | mph              |

#### 8.02.03.Acceleration（加速度）

| **Unit**                       | **Abbreviation** |
| ------------------------------ | ---------------- |
| Centimeters Per Second Squared | cm/s2            |
| Meters Per Second Squared      | m/s2             |

#### 8.02.04.Angles（角）

| **Unit** | **Abbreviation** |
| -------- | ---------------- |
| Degrees  | ° , deg          |
| Radians  | rad              |

#### 8.02.05.Angular Velocity（角速度）

| **Unit**           | **Abbreviation** |
| ------------------ | ---------------- |
| Degrees Per Second | deg/s            |
| Radians Per Second | rad/s            |

#### 8.02.06.Temperature（温度）

| **Unit**                   | **Abbreviation** |
| -------------------------- | ---------------- |
| **Temperature - SI**       |                  |
| Celsius                    | C                |
| Kelvin                     | K                |
| **Temperature - Imperial** |                  |
| Farenheit                  | F                |

#### 8.02.07.Mass（质量）

| **Unit**            | **Abbreviation** |
| ------------------- | ---------------- |
| **Mass - SI**       |                  |
| Micrograms          | µg               |
| Milligrams          | mg               |
| Grams               | g                |
| Kilograms           | kg               |
| Metric Tons         | t, Mg            |
| **Mass - Imperial** |                  |
| Ounces              | oz               |
| Pounds              | lb               |
| Stones              | st               |

#### 8.02.08.Density（密度）

| **Unit**                       | **Abbreviation** |
| ------------------------------ | ---------------- |
| **Density - SI**               |                  |
| Grams Per Cubic Centimeter     | g/cm3            |
| Grams Per Cubic Meter          | g/m3             |
| Kilograms Per Cubic Centimeter | kg/cm3           |
| Kilograms Per Cubic Meter      | kg/m3            |

#### 8.02.09.Force（力）

| **Unit**                                | **Abbreviation** | **In Base Units**              |
| --------------------------------------- | ---------------- | ------------------------------ |
| **Force - SI**                          |                  |                                |
| Newtons                                 | N                | 1 N = 1 kg • m / s2            |
| Kilograms Force                         | kgf              | 1 kgf = 9.80665 kg • m / s2    |
| Kilogram Centimeters Per Second Squared | kg • cm / s2     |                                |
| **Force - Imperial**                    |                  |                                |
| Pounds Force                            | lbf              | 1 lbf = 32.174049 lb • ft / s2 |

#### 8.02.10.Torque（扭矩）

| **Unit**                                        | **Abbreviation** | **In Base Units**      |
| ----------------------------------------------- | ---------------- | ---------------------- |
| **Torque - SI**                                 |                  |                        |
| Newton Meters                                   | N·m              | 1 N·m = 1 kg • m2 / s2 |
| Kilogram Centimeters Squared Per Second Squared | kg • cm2 / s2    |                        |

#### 8.02.11.Momentum（动力）

| **Unit**          | **Abbreviation** | **In Base Units**      |
| ----------------- | ---------------- | ---------------------- |
| **Momentum - SI** |                  |                        |
| Newton Seconds    | N·s              | 1 N • s = 1 kg • m / s |

#### 8.02.12.Frequency（频率）

| **Unit**               | **Abbreviation** | **In Base Units** |
| ---------------------- | ---------------- | ----------------- |
| **Frequency - SI**     |                  |                   |
| Hertz                  | Hz               | 1 Hz = 1 s-1      |
| Kilohertz              | kHz              |                   |
| Megahertz              | MHz              |                   |
| Gigahertz              | GHz              |                   |
| Revolutions Per Minute | rpm              | 1 rpm = 1/60 s-1  |

#### 8.02.13.Pixel Density（像素密度）

| **Unit**        | **Abbreviation** |
| --------------- | ---------------- |
| Pixels Per Inch | PPI              |

#### 8.02.14.Digital Information（存储大小）

| **Unit** | **Abbreviation** |
| -------- | ---------------- |
| Byte     | B                |
| Kilobyte | kB               |
| Megabyte | MB               |
| Gigabyte | GB               |
| Terabyte | TB               |

#### 8.02.15.Luminous Flux

| **Unit** | **Abbreviation** |
| -------- | ---------------- |
| Lumens   | lm               |

#### 8.02.16.Luminous Intensity（光强度）

| **Unit** | **Abbreviation** |
| -------- | ---------------- |
| Candela  | cd               |

#### 8.02.17.Illuminance（照明度）

| **Unit** | **Abbreviation** | **In Base Units** |
| -------- | ---------------- | ----------------- |
| Lux      | lx               | 1 lx = 1 lm/m2    |

#### 8.02.18.Luminance

| **Unit**            | **Abbreviation** |
| ------------------- | ---------------- |
| Candela Per Meter 2 | cd/m2            |

#### 8.02.19.Time（时间）

| **Unit**     | **Abbreviation** |
| ------------ | ---------------- |
| Nanoseconds  | ns               |
| Microseconds | µs               |
| Milliseconds | ms               |
| Seconds      | s                |
| Minutes      | min              |
| Hours        | hr               |
| Days         | d                |
| Months       | mo               |
| Years        | yr               |

#### 8.02.20.Pressure（压强）

| **Unit**     | **Abbreviation** | **In Base Units**    |
| ------------ | ---------------- | -------------------- |
| Pascals      | Pa               | 1 Pa = 1 kg / m • s2 |
| Kilo Pascals | KPa              |                      |
| Mega Pascals | MPa              |                      |
| Giga Pascals | GPa              |                      |

### 8.03.Other Units（其他）

| **Unit**       | **Abbreviation** | **Notes**                                                    |
| -------------- | ---------------- | ------------------------------------------------------------ |
| Exposure Value | EV               | Describes how much light is in a scene.                      |
| Percentage     | %                | Numerical value between 0 and 100.                           |
| Multiplier     |                  | Unitless quantity that represents multiples of some base quantity. |
| Unspecified    |                  | No specified units.                                          |