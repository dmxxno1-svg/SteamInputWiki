# 01：配置器简介

当你连接好控制器、在需要时启用了支持并调整了通用控制器设置之后，下一步就是熟悉配置器（Configurator），因为你将在其中花费相当多的时间。

如你所见，Steam 的控制器支持不仅限于游戏，还能扩展到整个电脑桌面环境。

## 配置类型

Steam 为你的控制器提供四类配置。使用这些配置时需要 Steam 正在运行。

* 桌面配置（Desktop Configuration）——当没有启动游戏或 Big Picture 模式时，使用此配置可以用控制器控制电脑桌面。
* Big Picture 模式配置（Big Picture Mode Configuration）——当 Steam 处于 Big Picture 模式（包括在桌面使用 Steam 屏幕键盘时）时，控制器使用此配置来导航界面。
* 指南键组合配置（Guide Chord Configuration）——这是一个全局配置，在按住控制器的 Guide/Home/System 按钮时可以随时访问。它适合媒体控制等功能，这样你无需在所有配置中都为这些功能找位置。
* 每款游戏的配置（Per Game Configurations）——你通过 Steam 运行的每款游戏都有自己的配置，允许你为每个游戏定制体验。

## 在哪里可以找到控制器配置

你需要先把控制器连接到电脑，才能访问相应配置。

### Steam 桌面端

你可以通过点击菜单“Steam”→“Settings”，然后在左侧选择“Controller”类别来找到桌面配置、Big Picture 配置和 Guide Chord 配置。从那里可以访问这些设置。

你可以通过三种方式访问游戏特定的配置：

* 在库（Library）视图中点击某款游戏。在“Play（开始）”按钮下方有一排链接，例如商店页面和社区中心。连接控制器时，“Controller Configuration（控制器配置）”位于该排链接的最右侧。注意：你可能需要按“更多（…）”按钮来显示该项。
* 在库中右键点击某款游戏，选择“Manage（管理）”，列表中会有“Controller Configuration”选项。
* 在游戏中打开覆盖层（Overlay）也能访问配置：
  * 在 Big Picture 模式的覆盖层中，左侧列表内会有“Controller Configuration”选项；
  * 在桌面覆盖层中，“Controller Configuration”是靠近右上角的一个按钮，点击它会最小化游戏并以单独窗口弹出配置界面。修改完成并点击“Done（完成）”后，游戏会被恢复。

### Steam Big Picture 模式

从 Big Picture 模式访问桌面、Big Picture 与 Guide Chord 配置的流程稍微复杂一些：

* 在 Big Picture 模式主页面的右上角找到齿轮图标（设置）。
* 选择齿轮图标进入 Big Picture 模式的设置页面。
* 在左侧栏目有“Controller（控制器）”类别。
* 在该类别下有“Base Configurations（基础配置）”。
* 选择它可以进入一个页面，从中访问桌面、Big Picture 和 Guide Chord 的配置。

访问游戏特定配置也略有不同：

* 在 Big Picture 模式主页面上，屏幕中央偏下的位置有“Library（库）”图标，选中并进入它。
* 这里会显示你最近游玩的或最近更新的游戏；你可以返回上一级以查看库中更多分类。
* 找到你想要配置或游玩的游戏并选中它。
* 默认高亮的是左侧栏的“Your Game（你的游戏）”按钮，但你应向下移动一项并选择“Manage Game（管理游戏）”。
* 选中后默认高亮的第一个项就是“Controller Configuration”，选择它以进入配置界面。

在游戏中，你仍可以随时通过打开 Steam Overlay 来访问配置器。

## 配置总览页面的结构（Anatomy of the Configuration Overview Page）

打开某个配置后，会进入配置总览页面（Configuration Overview Page），该页面旨在为你提供一目了然的配置视图。

页面中央是一个所配置控制器的示意图。

顶部是配置名称，正下方显示创建该配置的用户名。

标题下方列出任何动作集（action sets）或动作层（action layers）（第 04 章将介绍集与层的概念）。

如果使用 Sony DualShock 4 或 DualSense，集与层下面会显示触控板（Touchpad）设置，你可通过按钮在“统一触控板（unified）”与“分割触控板（split）”间切换。

从控制器的左侧开始向下列出：

* 左扳机完全拉到底绑定（Left Trigger Full Pull，若适用）
* 左扳机软拉（Left Trigger Soft Pull，若适用）
* 左肩键绑定（Left Bumper）
* 左握把按钮绑定（Left Grip Button，Steam 控制器专属）
* Select/- 按钮绑定
* 麦克静音（DualSense）/截屏（Capture，Switch Pro）按钮绑定
* 始终启用绑定（Always On Binding）

从顶部回到右侧向下列出：

* 右扳机完全拉到底绑定（Right Trigger Full Pull，若适用）
* 右扳机软拉绑定（Right Trigger Soft Pull，若适用）
* 右肩键绑定（Right Bumper）
* 右握把按钮绑定（Right Grip Button，Steam 控制器专属）
* Start/+ 按钮绑定

对于某些非 Xbox 控制器，在控制器图片下方会显示：

* Gyro（陀螺；通常以几个椭圆在圆圈内的图标表示）

页面底部有一排四个矩形，这些矩形代表控制器上的四个主要输入设备，顺序与控制器左右方向一致：

对于 Xbox 与 Switch Pro 控制器，顺序为：

* 左摇杆
* 方向键（D-pad）
* 右摇杆
* ABXY / B A Y X 按键簇

对于 Sony 控制器，顺序为：

* 方向键
* 左摇杆
* 右摇杆
* 十字/圈/方块/三角（Cross-Circle-Square-Triangle）按键簇

对于 Steam 控制器，顺序为：

* 左触控板
* 左摇杆
* ABXY 按键簇
* 右触控板

为了帮助定位某个绑定或输入风格对应控制器的哪个位置，页面上有连线将它们联系起来。当你高亮某个绑定或输入设备时，相应的连线会高亮以更清楚地显示对应关系。

页面最底部是一排 UI 按钮。

如果使用控制器导航配置总览页面，这些 UI 按钮对应面部按键簇上的按键。按钮包括：

* Select（选择）— 在高亮某个绑定或输入风格时，激活它会进入该绑定或输入风格的设置。
* Browse Configs（浏览配置）— 进入“Controller Configurations - Import” 页面，允许你从按类别划分的现成配置中应用一个新的配置。
* Export Config（导出配置）— 进入“Controller Configuration - Export” 页面，允许你按多种方式保存当前配置。
* Done（完成）— 关闭配置总览页面。

如果使用鼠标导航，总览页面不再显示“Select”按钮；直接点击某个绑定或输入风格即可进入设置。其余三个按钮仍然存在，但变为可点击元素而非通过面部按键激活。

接下来是：

## 在配置总览页面中导航（Navigating the Configuration Overview Page）

若使用控制器导航页面，默认操作如下：

* 方向键或左摇杆用于上下左右移动以高亮不同的绑定和输入风格。
* 屏幕底部的按键提示告诉你如何与页面交互。两个最重要的 UI 按钮是 Select（进入）和 Back（返回），它们使用面部按键簇上的按键（例如 Steam 控制器与 Xbox 为 A 和 B，Switch Pro 为 B 和 A，Sony 控制器为 Cross 与 Circle）。

配置器实际上使用 Big Picture 模式下的配置来进行交互（即配置器是 Big Picture 的一部分，即便在桌面窗口中打开也是如此）。因此，你可以通过自定义 Big Picture 模式的配置来改变在 Big Picture 与配置器中的导航方式。

如果使用鼠标导航，事情更加简单：所有操作就是点选。

## 导入配置（Importing A Configuration）

如果你想快速把配置切换为完全不同的方案，可以导入一个配置。

通过点击或按下与“Browse Configs（浏览配置）”相关联的按钮即可。

这会带你到“Controller Configurations - Import” 屏幕。注意：此屏幕上显示的配置默认均为针对你当前游戏的配置，除非另有说明。

屏幕左侧列出配置来源类别：

* Recommended（推荐）— 如果开发者为其游戏创建了配置或选择了他们认为合适的模板，你会在此看到这些配置；开发者也可能为不同的游玩风格提供多个配置。
* Personal（个人）— 这里列出你已为该游戏导出的所有个人配置。
* Your Friends（你的好友）— 如果你的好友将配置导出并分享到了社区，你可以在此快速找到他们的配置。
* Community（社区）— 这是其他玩家为该游戏导出的所有配置列表。
* Templates（模板）— 包含 Valve 提供的通用模板，作为起点而非最优解。
* Your Other Games（你的其他游戏）— 列出你为其它游戏创建的配置，适用于你希望多款游戏使用同一套控制方式的情形（例如 Dark Souls 1/2/3）。

选定类别后，该类别的配置列表会更突出地显示在屏幕中央。

可用鼠标滚轮或控制器的方向键滚动列表。

屏幕底部显示与列表交互的按键提示，包括：

* Import Config（导入配置）
* Show Other Controller Types（显示其它控制器类型）— 默认只显示为你当前控制器创建的配置。你可以查看并导入其它控制器的配置，但转换可能并不完美。
* Back（返回）
* Share Configuration（分享配置）— 会生成一个类似 `steam://controllerconfig/367520/2299077420` 的可分享链接（例如作者为 Steam 控制器制作的 Hollow Knight 配置）。在 Steam 运行时将该链接粘贴到浏览器即可查看配置。
* Remove（移除）— 仅对你自己的配置可用，用于删除配置条目。
* Sort By Votes（按票数排序）— 仅在社区配置中可用，用于根据投票数调整显示顺序。
* Upvote（投票）— 仅在社区配置中可用，用于给你喜欢的配置投票。

当你高亮某个可能感兴趣的配置时，按“Import Config（导入配置）”。

这会带你到配置总览预览页面（Configuration Overview Preview）。在该页面你可以像正常浏览配置一样查看，但不能修改任何设置；这只是让你检查配置是否符合你的需求。

如果喜欢，按“Apply Configuration（应用配置）”（位于预览页面底部）会将其完全应用。

如果不满意，可以按 Back 返回“Controller Configurations - Import”界面。

## 导出配置（Exporting A Configuration）

如果你对某个配置做了调整并想保存或分享给社区，可以导出它！

在配置总览页面底部按下“Export Config（导出配置）”按钮即可。

这会进入“Controller Configurations - Export”页面。

屏幕左侧列出可导出的目标分类（默认均为针对当前游戏）：

* Personal（个人）— 保存到你个人的配置列表中（可本地或在线保存）。
* Your Friends（你的好友）— 列出你好友导出的配置（作为导出目标时此分类的存在意义不太明显）。
* Community（社区）— 若想向任何人公开分享配置，请导出到此分类。注意：Valve 要求在上传到社区之前，你需至少以该配置游玩 5 分钟（目的在于确保配置制作者先行测试并修复潜在问题）。
* Templates（模板）— 如果你制作的配置适用于多款游戏（例如为 RTS 游戏做的通用模板），可以导出为模板。
* Your Other Games（你的其他游戏）— 列出来自你其他游戏的配置（导出时显示该分类的用途并不明确）。

选择导出目标后，会弹出一个对话框用于命名配置并填写简短描述，填写完毕后点击保存即可完成导出。