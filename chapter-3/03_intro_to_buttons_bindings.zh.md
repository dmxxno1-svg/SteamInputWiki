```markdown
<<<<<<< Updated upstream
# 第 03 章：按钮与绑定简介

## 介绍

按钮是一个简单的二元“开/关”输入设备：按下它，会告诉被控制的对象执行某个操作。

在触摸板、触摸屏、屏幕内菜单盛行的时代，按钮也可以是虚拟（Virtual）的；例如在触摸板上的某一区域被指定为一个按钮。它的行为像按钮，但并非物理按压，而是“触碰”该区域来触发。

绑定（Binding）是将按钮按下时触发的动作。

## 哪些物理按钮可以分配绑定？

以下是你可能熟悉的物理按钮，有些按钮自游戏早期就存在，有些是较新的补充：

- 单个 A、B、X、Y（或 Sony 等效）按钮 / 按钮面板输入风格中的绑定位置
- 单个方向键（D-Pad）方向（方向键输入风格中的绑定位置）
- 左/右摇杆按下（Stick Click），在相应输入风格中作为“Click Action”出现
- 左/右触摸板点击（Steam Controller 的触摸板），在相应输入风格中作为“Click Action”出现
- 右/左/单独触摸板点击（Sony 触摸板），在相应输入风格中作为“Click Action”出现
- Start / Forward / +
- Select / Back / -
- Capture（Nintendo Switch Pro 控制器）
- 右/左肩键（Bumper）
- 右/左扳机的完全按下（Trigger Full Pull）——适用于仅数字扳机或在模拟扳机拉到底的情形
- 麦克风静音（Sony DualSense）
- 左/右握把按钮（Steam Controller）
- Xbox Elite 系列 2 控制器的 1-4 号拨片（在开启 Extended Support 且控制器本体加载空白配置时）

注意：无法重新绑定控制器上的 Guide/Home/System 按钮，Steam 将其保留用于访问 Steam 功能或 Guide Chord 配置。

## 哪些虚拟按钮可以分配绑定？

这些并非传统的物理按钮，而是可以触发绑定的软件事件。例如在 Steam Input 中使用触摸板时，仅仅触碰触摸板就可以作为一个虚拟按钮来激活绑定。

- 虚拟 A、B、X、Y（或 Sony 等效）：当“按钮面板（Button Pad）”输入风格应用于触摸板或摇杆等非 ABXY 传统设备时可用
- 虚拟方向键方向：当“方向键（Directional Pad）”输入风格应用于触摸板或摇杆等非方向键传统设备时可用
  - 也用于“方向滑动（Directional Swipe）”输入风格
- “触摸绑定（Touch Binding）”，常见于将输入风格应用于触摸板时
  - 在“单按钮（Single Button）”输入风格中被重命名为“Trackpad Touch”
- “双击绑定（Double Tap Binding）”，常见于触摸板输入风格
- “外环绑定（Outer Ring Binding）”，出现在可应用于 XY 坐标输入设备的多个输入风格中
- 触摸菜单按钮 1-16，出现在“Touch Menu”输入风格中
  - 也出现在 Hotbar Menu 输入风格中
- 径向菜单按钮 1-20，出现在“Radial Menu”输入风格中
- “中心/未选中按钮（Center/Unselected Button）”，出现在“Radial Menu”输入风格中
- “向前/向后滚动绑定（Scroll Forward/Backward）”，出现在滚轮输入风格中
- 滚轮列表选项 1-10，出现在滚轮输入风格中
- “陀螺向左/向右倾斜绑定（Gyro Lean Left/Right）”，仅对陀螺输入设备可用
- “始终开启绑定（Always On Binding）”，在配置概览页面作为左侧最靠近的输入设备上方的无限符号显示
- 右/左扳机软拉动（Trigger Soft Pull）——适用于模拟扳机，使用用户定义的阈值作为逻辑点击
- 力传感电阻（Force Sensing Resistor）——物理设备但不提供机械点击，用压力阈值（由用户设置）作为逻辑点击

## 可以指派到按钮的绑定类型有哪些？

共有 5 种绑定类型：

- 鼠标按键（Mouse Buttons）
- 键盘按键（Keyboard Buttons）
- 手柄按键（Gamepad Buttons）
- Steam / 系统操作（Steam/System Actions）
- SIAPI 游戏内动作（SIAPI In-Game Actions）

这些将在本章稍后部分更详细地讨论。
=======
# 第03章：按钮与绑定简介

## 介绍

“按钮”是最简单的二元（开/关）输入设备；你按下它，它就会告诉你正在控制的对象该做什么。

在触控板、触摸屏、屏幕菜单等普及的今天，按钮也可以是“虚拟”的；例如把触控板上的某一区域指定为一个按钮。它的工作方式像按钮，但并不是实体按键——你是“触摸”该区域，而不是“按下”实体按键。

“绑定”是指当按钮被按下时会发生的动作。

## 哪些物理按键可以分配绑定？

下面是你可能熟悉的物理按键，有些按键可以追溯到游戏早期，也有些是较新的增加项。

* 单个 A、B、X、Y（或索尼的等价键）——见按钮面板输入样式的绑定位置
* 十字键（D-Pad）的各个方向——见方向键输入样式的绑定位置
* 左/右摇杆按下（Stick Click），作为各自输入样式中的“Click Action”
* 左/右触控板点击（Steam 控制器触控板），作为各自输入样式中的“Click Action”
* 左/右/独立触控板点击（索尼触控板），作为各自输入样式中的“Click Action”
* Start / Forward / +
* Select / Back / -
* Capture（任天堂 Switch Pro 控制器）
* 左/右肩（Bumper）
* 左/右触发器的完全触发（Trigger Full Pull）——适用于只有数字触发器的手柄，或模拟触发器的行程末端
* 麦克风静音（Sony DualSense）
* 左右握把按钮（Steam 控制器）
* Xbox Elite Series 2 的 1-4 号桨板（Paddles），在控制器上启用扩展支持并加载空白配置时可用

注意：你不能重新绑定控制器上的 Guide / Home / System 按钮，Steam 会保留该键用于访问 Steam 功能或 Guide Chord 配置。

## 哪些“虚拟按钮”可以被绑定？

这些不是传统的物理按键，而是可以用来触发绑定的软件事件。例如在 Steam Input 中使用触控板时，简单的触摸就可以作为一个虚拟按钮来激活绑定。

* 当把“按钮面板（Button Pad）”输入样式应用到不常见的设备（如触控板或摇杆）时，会产生虚拟的 A、B、X、Y（或索尼等价）按钮
* 当把“方向键（Directional Pad）”输入样式应用到不常见的设备时，会产生虚拟的十字键方向
  * 在“方向滑动（Directional Swipe）”输入样式中也会使用该方式
* “触摸绑定（Touch Binding）”，通常在将输入样式应用到触控板时出现
  * 在“单按钮（Single Button）”输入样式中称为“触控板触摸（Trackpad Touch）”
* “双击绑定（Double Tap Binding）”，通常在将输入样式应用到触控板时出现
* “外环绑定（Outer Ring Binding）”，在若干可应用到 XY 坐标输入设备的输入样式中可见
* 触摸菜单（Touch Menu）中的按钮 1-16
  * 在热键栏菜单（Hotbar Menu）中也可见
* 环形菜单（Radial Menu）中的按钮 1-20
* 环心/未选中按钮（Center/Unselected Button），见环形菜单输入样式
* 滚轮前进/后退绑定（Scroll Forward/Backward Binding），见滚轮输入样式
* 滚轮列表选项 1-10，见滚轮输入样式
* 陀螺左右倾斜绑定（Gyro Lean Left/Right Binding），仅对陀螺设备可用
* “始终开启绑定（Always On Binding）”，在配置概览页上显示为靠左的无限符号，表示始终有效
* 左/右触发器软触发（Trigger Soft Pull）——适用于模拟触发器，使用用户定义的阈值，当触发器超过阈值时视为逻辑点击
* 力敏电阻（Force Sensing Resistor）——这是一种物理设备但没有物理扣动感；它使用用户设定的压力阈值作为逻辑点击

## 可以分配给按钮的绑定类型有哪些？

有 5 类绑定：

* 鼠标按键（Mouse Buttons）
* 键盘按键（Keyboard Buttons）
* 手柄按键（Gamepad Buttons）
* Steam/系统操作（Steam/System Actions）
* SIAPI 游戏内动作（SIAPI In-Game Actions）

这些内容将在本章后续部分中更详细地介绍。
>>>>>>> Stashed changes

```
