# UnrealEngine学习(04)：自定义虚幻引擎

​	**虚幻引擎5** （UE5）在操作体验的自定义方面提供了极大的灵活性。你可以使用UE5的内置工具来创建和保存自定义布局，改变界面配色方案，编辑快捷键，添加或删除各种保存在独立插件中的功能。

## 1. 使用插件

**插件（plugin）** 是可选的软件组件，用于向 **虚幻引擎（Unreal Engine）** 添加特定功能。插件可以添加全新的功能以及修改内置功能，而不直接修改虚幻引擎代码。例如，插件可以将新菜单项和工具栏命令添加到编辑器，甚至可以添加全新的功能和编辑器子模式。

你可以根据需要为每个项目独立启用或禁用插件。

虚幻引擎中提供了两种类型的插件：

- 虚幻引擎插件。
- 第三方插件。

### 1.01.启用插件

要启用虚幻引擎插件，请执行以下步骤：

1. 在主菜单中，前往 **编辑（Edit）> 插件（Plugins）** 。这将打开 **插件（Plugins）** 窗口。

	![image-20240827094123638](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\image-20240827094123638.png)

	![虚幻引擎5中的](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\ue5-plugins-window.png)

2. 使用屏幕左侧的列表查找你想启用的插件。或者，在 **搜索（Search）** 框中输入一个词以搜索包含该词的所有插件名称和说明。

	![按名称搜索插件](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\finding-plugins.png)

	> 此示例显示"xr"一词的所有搜索结果。请注意，搜索词在出现的所有地方都已高亮显示。

3. 要启用插件，请点击其旁边的复选框。

	![启用插件。](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\enabling-a-plugin.png)

	> 对于非生产就绪的插件（例如测试版插件），你可能会看到警告，要求你确认你想启用该插件。

4. 保存你的工作，然后重新启动虚幻引擎。

第三方插件可能要求执行额外步骤，你才能将其启用。有关更多信息，请参阅你想安装的第三方插件的文档。请注意，Epic Games对第三方插件的内容概不负责。

### 1.02.禁用插件

要禁用插件，请执行以下步骤：

1. 在主菜单中，前往 **编辑（Edit）> 插件（Plugins）** 。这将打开 **插件（Plugins）** 窗口。

	![虚幻引擎5中的](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\ue5-plugins-window.png)

	`虚幻引擎5中的"插件"窗口。`

2. 使用屏幕左侧的列表查找你想禁用的插件。或者，在 **搜索（Search）** 框中输入一个词以搜索包含该词的所有插件名称和说明。

	![按名称搜索插件](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\finding-plugins.png)

	`此示例显示"xr"一词的所有搜索结果。请注意，搜索词在出现的所有地方都已高亮显示。`

3. 要禁用插件，请清除其旁边的复选框。

	![禁用插件](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\disabling-a-plugin.png)

	`禁用插件`

	> 如果你想禁用的插件是其他插件的 *依赖项* （即，其他插件需要该插件才能运行），你将看到通知，询问你是否也要禁用这些插件。请注意，如果你使用了其中的插件来实现项目中的现有功能，禁用插件后可能会破坏该功能。

4. 保存你的工作，然后重新启动虚幻引擎。

### 1.03.从虚幻引擎商城安装插件

即使虚幻引擎包含能提供许多不同种类功能的插件，你仍可以从[虚幻商城](https://www.unrealengine.com/marketplace/zh-CN/store)安装额外的插件。

要使用此方法安装插件，请执行下面的步骤。这些步骤使用Epic Games提供的免费"glTF导出器（glTF Exporter）"插件作为示例。

1. 在Epic Games **启动程序（Launcher）** 中，导航到 **虚幻引擎（Unreal Engine）** 选项卡，然后转到 **商城（Marketplace）** 。

	![虚幻引擎商城](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\marketplace-plugins-1.png)

2. 搜索你想安装的插件。

	![搜索虚幻引擎商城上的插件](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\marketplace-plugins-2.png)

3. 在插件的图块上，点击 **添加到购物车（Add to Cart）** 。

	![将插件添加到购物车](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\marketplace-plugins-3.png)

4. 点击 **购物车（Cart）** 按钮并结账。

	![结账](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\marketplace-plugins-4.png)

	对于免费插件，你在此阶段不需要执行额外的步骤。对于付费插件，你必须完成付款流程，才能进行使用。

	> 结账后，插件的图块将显示OWNED一词。

5. 在启动程序中转到插件的页面。为此，你可以搜索该插件，然后点击该插件的图块。然后，在插件的图块上，点击 **安装到引擎（Install to Engine）** 。

	![插件的](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\marketplace-plugins-5.png)

6. 选择你想安装插件的引擎版本，然后点击 **安装（Install）** 。

	![选择虚幻引擎版本](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\marketplace-plugins-6.png)

	> 此下拉菜单仅显示插件支持的虚幻引擎版本，即使你安装了其他虚幻引擎版本。

7. 安装完成后，打开你为其安装插件的虚幻引擎版本，然后按照此页面上的"启用插件"分段中的说明操作，以 **启用** 该插件。

### 1.04.插件安装位置

虚幻引擎将所有插件存储在以下位置：

- Windows上的 `C:\Program Files\Epic Games\UE_[version]\Engine\Plugins`
- macOS上的 `/Users/Shared/Epic Games/UE_[version]/Engine/Plugins`



## 2.自定义按键快捷键

介绍如何调整虚幻引擎中常用命令的快捷键，创建新的快捷键以便适应你的使用习惯。

**按键快捷键**，也叫做 **键绑定**，本质上是一种组合按键，可以执行特定命令或操作。你可以为一些常用命令和工具设置快捷键，以便满足你的个人习惯。设置方法如下：打开 **编辑器偏好设置** 窗口，在主菜单中，进入 **编辑 > 编辑器偏好设置**，然后选择 **键盘快捷键**。

![Keyboard Shortcuts editor in Unreal Engine](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\keyboard-shortcuts.png)

`编辑器偏好设置 窗口中的快捷键编辑器。`

此处的命令按功能区域分组。每个命令最多可以绑定两个快捷键。

### 2.01.新建一个键盘快捷方式

1. 点击需要绑定快捷键的命令旁的 **文本字段**。

2. 按下你希望使用的组合键。

	![Adding a new keyboard shortcut](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\adding-new-shortcut.png)

当你点击文本字段以外的任何位置时，虚幻引擎会自动保存新的快捷键。

> 如果你设置的组合键已经与另一个命令绑定，你会看到一个警告。如果你想删除已有的绑定，并将快捷键分配给新的命令，请点击 **覆盖** 按钮。如果你想保留现有的绑定，并取消新的绑定，请点击文本字段外的位置。

![键盘快捷方式已经存在](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\shortcut-already-exists.png)

### 2.02.移除已有的快捷键

要删除一个已有的快捷键，请点击它旁边的 **删除**（**X**）按钮。

![Removing a keyboard shortcut](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\removing-a-shortcut.png)

### 2.03.导入和导出键盘快捷键

你可以将自定义按键绑定导出为一个 `.ini` 文件，然后导入并用于其他虚幻引擎编辑器。假如你需要在不同计算机上工作，或者经常需要重新安装引擎，这就很有用。

如需将自定义键位保存为 `.ini` 文件，请单击 **导出** 按钮。点击 **导入** 按钮可以导入外部 `.ini` 文件的自定义键位。这两个按钮都位于 **按键快捷键** 编辑器的顶部。

![Export and Import buttons in the Keyboard Shortcuts editor](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\export-import-buttons.png)

`导出 和 导入 按钮的位置。`



## 3.编辑器偏好设置

用于配置控件、视口、源码管理等通用编辑器行为的选项。

[![Editor Preferences Dialog](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\editorpreferences.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/bff6bb82-c1a4-4dc8-b799-ecc93fafc80e/editorpreferences.png)

**编辑器偏好设置（Editor Preferences）** 窗口用于修改与控件、视口、源码控制、自动保存等相关的编辑器行为的设置。

要打开 **编辑器偏好设置（Editor Preferences）** 窗口，单击 **编辑（Edit）> 编辑器偏好设置（Editor Preferences）**。

[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\editmenu.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/b7e832fc-03ec-4009-9fbe-e5ee355f32a8/editmenu.png)

### 3.01.关卡编辑器偏好设置 - 视口

### 3.02.控制选项

| 选项                                                         | 说明                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| **飞行摄像机控制类型（Flight Camera Control type）**         | 该设置决定了是否使用飞行摄像机及如何获得它。飞行摄像机使用W、A、S和D键来推动和平移摄像机，与标准的FPS控件的工作方式类似。W和S向内和外推动摄像机，而A和D从一侧向另一侧平移或扫过摄像机。启用此选项后，将覆盖使用这些控件的所有热键，包括用于切换显示标志的热键。选项说明**使用WASD控制摄像机（Use WASD for Camera Controls）**始终启用飞行摄像机和WASD控制。**仅当按下鼠标右键时使用WASD控制（Use WASD Only When Right Mouse Button is Held）**仅当按下鼠标右键时才启用飞行摄像机和WASD控制。**永远不使用WASD摄像机控制（Never Use WASD for Camera Controls）**永远不启用飞行摄像机和WASD控制。 |
| **通过拖拽来移动正交摄像机（Grab and Drag to Move Orthographic Cameras）** | 如果启用该项，那么在正交视口中单击鼠标左键或右键并拖拽鼠标将会滚动摄像机。本质上讲，这在实际操作中意味着当你单击并拖拽时场景将会随着鼠标移动。如果禁用该项，场景将向鼠标相反的方向移动。 |
| **正交缩放到光标位置处（Orthographic Zoom to Cursor Position）** | 如果启用该项，在正交视口中进行缩放操作将会围绕鼠标光标中心进行。当禁用该项，缩放将以视口中央为中心进行。 |
| **连接正交视口移动（Link Orthographic Viewport Movement）**  | 如果启用该项，那么将会连接所有正交视口，使它们聚焦到同一位置。因此，当在一个正交视口中移动摄像机时将会导致其他正交视口跟随着移动。当禁用该项时，每个视口可以独立移动。 |
| **高宽比轴约束（Aspect Ratio Axis Constraint）**             | 确定当改变大小时使用透视口的哪个坐标轴来控制视场(FOV)，从而维持高宽比。选项说明**维持Y-轴视场（Maintain Y-Axis FOV）**使用Y-轴（垂直轴）来决定视场。**维持X-轴视场（水平）（Maintain X-Axis FOV**使用X-轴（水平轴）来决定视场。**维持主轴视场（Maintain Major Axis FOV）**使用两个轴中较大的一个来决定视场。 |
| **鼠标滚动摄像机的速度（Mouse Scroll Camera Speed）**        | 确定在使用鼠标导航时透视图摄像机的移动速度。                 |

#### 3.02.01.视口外观和感觉

| 选项                                                         | 说明                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| **突出显示鼠标下的对象（Highlight Objects Under Mouse Cursor）** | 如果启用该项，那么当将鼠标光标悬停到某个对象上时，将会在视口中使用一个透明的覆盖层突出显示该对象。 |

<iframe width="560" height="315" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen="" src="https://www.youtube-nocookie.com/embed/yvwZUtmW12I" style="box-sizing: border-box; border: 0px; position: absolute; top: 0px; left: 0px; width: 808.6px; height: 454.837px;"></iframe>

#### 3.02.02.编辑器外观和感觉

| 选项                                             | 说明                                                         |
| ------------------------------------------------ | ------------------------------------------------------------ |
| **使用小工具栏图标（Use Small Tool Bar Icons）** | 如果启用该项，整个编辑器的工具栏图标将变为较小的图标，且没有标签。![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\look_and_feel_normal.png)![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\look_and_feel_small.png)**正常图标****小图标** |

#### 3.02.03.关卡编辑

| 选项                                                         | 说明                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| **启用组合的平移/旋转控件（Enable Combined Translate/Rotate Widget）** | 启用后，合并后的平移和旋转-Z工具将变为可用。![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\transrotation_widget.png) |
| **单击BSP启用画刷（Clicking BSP Enables Brush）**            | 如果启用该项，单击画刷（Brush）表面选中画刷，并按下 **Ctrl + Shift + 单击** 选中表面。当禁用该项时，则相反；单击鼠标选中表面，按下 **Ctrl + Shift + 单击** 键选中画刷。 |
| **自动更新BSP（Update BSP Automatically）**                  | 如果启用该项，当在视口中移动或修改画刷时会自动重新构建画刷（Brush）几何体。当启用该项时，则必须手动重新构建几何体来查看改变。 |
| **在替换对象上保持Actor缩放比例（Preserve Actor Scale on Replace）** | 如果启用该项，那么替换的Actor将遵循原始Actor的比例。否则，替换Actor的比例是1.0。 |

### 3.03.源码控制

| 选项                                                         | 说明                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| **当修改包时提示检出它（Prompt for Checkout on Package Modification）** | 如果启用该项，编辑器将自动在修改包时提示从源码控制签出该包。 |
| **允许源码控制（Allow Source Control）**                     | 如果启用该项，则为包和地图应用编辑器源码控制集成。           |
| **修改后添加新文件（Add New Files when Modified）**          | 如果启用该项，将自动添加新文件到源码控制中。                 |
| **主机（Host）**                                             | 源码控制服务器的主机和端口。示例：`hostname:1234`            |
| **用户名（Username）**                                       | 连接源码控制时使用的用户名。                                 |
| **工作区（Workspace）**                                      | 源码控制的客户端配置项。                                     |

#### 3.03.01.粒子

| 选项                                             | 说明                                                         |
| ------------------------------------------------ | ------------------------------------------------------------ |
| **使用分布曲线（Use Curves for Distributions）** | 如果启用该项，当在编辑器中渲染分布时，分布将使用曲线展现而不是烘焙的查找表。 |

#### 3.03.02.内容浏览器

| 选项                                                         | 说明                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| **自动重新导入纹理（Auto Reimport Textures）**               | 如果启用该项，则监控纹理的源文件，当源文件发生改变时自动重新导入纹理。 |
| **在警告出现之前设置一次性导入资源的数量（Assets to Load at Once before Warning）** | 在显示加载太多资源的警告之前 **内容浏览器** 内一次性加载对象的数量。 |

#### 3.03.03.隐私

虚幻引擎4（UE4）中的编辑器收集使用数据，以帮助Epic不断改进UE4。编辑器可以收集三种类型的数据：

- 崩溃报告 - 在出现导致引擎崩溃的错误时生成。
- Bug报告（也称为保证） - 在出现某些问题，导致项目进入某种未预见到的特定状态，但没有崩溃时生成。
- 使用数据（也称为分析）- 关于用户的数据集。

引擎崩溃时会生成崩溃报告。崩溃报告自动为你提供是否向Epic发送崩溃数据的选择。

##### 3.03.03.01.禁用Bug报告

关于Bug报告，可以在编辑器偏好设置的 **隐私** 分类下禁用数据收集。请按以下步骤操作以禁用Bug报告。

1. 在菜单栏中，单击 **编辑（Edit）> 编辑器偏好设置（Editor Preferences）**。

	[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\editmenu.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/bf475014-fbff-4f22-8d00-3aee4e791728/editmenu.png)

2. 在编辑器偏好设置（Editor Preferences）对话框中，向下滚动至 **隐私（Privacy）** 类别。

	[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\editorprefsprivacysection.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/f37b9317-b4c0-4ba1-bbf6-b0d008c6e49f/editorprefsprivacysection.png)

3. 单击 **Bug报告（Bug Reports）**。在右窗格的 **选项（Options）** 下，默认设置为 **发送无人值守的Bug报告（Send unattended bug reports）**。

	[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\editorprefsbugreportsdefault.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/b9a323ef-347b-4a5c-aa75-9eac9c3f083e/editorprefsbugreportsdefault.png)

4. 如果不希望将bug报告发送给Epic，请单击 **不发送（Don't Send）**。

	[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\editorprefsbugreportsoptout.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/737496a0-a6b4-445e-95f2-8297db0a145b/editorprefsbugreportsoptout.png)

##### 3.03.03.02.禁用使用数据

使用数据主要由聚合或匿名信息组成，这些信息不会直接将你作为个人用户识别出来。然而，这些使用数据也可能包括以下内容：

- 用户的IP地址
- 用户的Internet服务提供商（ISP）
- 用户所在的洲、国家/地区和城市
- 用户的Epic帐户ID
- 用户的项目名称

如果你担心隐私问题，希望选择退出用户数据收集，你可以在编辑器偏好设置的 **隐私** 分类下进行设置。要禁用使用数据收集，请参见下面的步骤。

1. 在 **编辑器偏好设置（Editor Preferences）** 对话框中，向下滚动至 **隐私（Privacy）** 类别。

	[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\editorprefsprivacycategory.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/d307ed1b-53fd-42d3-9d0d-3d54300307d2/editorprefsprivacycategory.png)

2. 单击 **使用数据（Usage Data）**。在右窗格的 **选项（Options）** 下，默认设置为 **发送使用数据（Send Usage Data）**。

	[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\usagedatadefault.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/0cc9c7e3-c0b8-4556-875a-0f0685c52527/usagedatadefault.png)

3. 如果不希望将使用数据发送给Epic，请单击 **不发送（Don't Send）**。

	[![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\usagedataoptout.png)](https://d1iv7db44yhgxn.cloudfront.net/documentation/images/23fd27de-cd55-49c6-a493-df07a7da573f/usagedataoptout.png)

### 3.04.自动保存

| 选项                                               | 说明                                                         |
| -------------------------------------------------- | ------------------------------------------------------------ |
| **启用自动保存（Enable AutoSave）**                | 如果启用该项，编辑器将按指定的时间间隔自动保存操作。         |
| **保存地图（Save Maps）**                          | 如果启用该项，自动保存过程将会尝试保存已加载的修改后地图。   |
| **保存包（Save Packages）**                        | 如果启用该项，自动保存过程将会尝试保存已修改的内容包。       |
| **保存频率，以分钟为单位（Frequency in Minutes）** | 每次自动保存之间的时间间隔，以分钟为单位。                   |
| **多少秒后出现警告（Warning in Seconds）**         | 在执行自动保存前的多少秒内显示警告。![img](D:\TyporaData\UnrealEngine\参考手册\01_理解基础知识\UnrealEngine学习(04)：自定义虚幻引擎.assets\autosave_warning.png) |