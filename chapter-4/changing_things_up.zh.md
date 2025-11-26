```markdown
# 第 04 章：变换使用方式

有时候，仅靠绑定和输入风格无法满足：

* 良好地游玩某款游戏
* 符合你的游玩风格
* 或两者兼顾

例如，键鼠专用且按键繁多的游戏常属第一类，而任意类型的游戏都有可能属于第二类。

当遇到这些情况且手柄上的输入已全部占用，你可能会想有哪些办法能在不改动硬件的前提下实现更多操作。

本章将介绍如何使用 Steam Input 中的工具，在运行时大幅扩展控制器的功能。

Steam Input 提供了 4 种工具：

* Activators（触发器）
  * 改变按钮的触发方式
* Modeshifts（模式切换）
  * 改变使用输入风格的方式
* Action Sets（动作集合）
  * 可视为可切换的完整配置，适用于不同上下文（菜单、行走、飞行等）
* Action Layers（动作层）
  * 类似集合但作用范围更小，适用于临时改动少量输入

本章后续小节将逐一详述这些工具并解释相关设置，帮助你尽可能地将它们利用起来。

## 第 04a 章：Activators（触发器）

什么是 Activator？

按下按钮会触发一个动作。这就是 Activator，但它能做到的不止于此。

在绑定页面按下 Select（或点击“Show Activators”）即可进入 Activator 页面，你会看到大量选项用于自定义：按键的不同按压方式如何影响结果，以及触发后结果如何表现。你甚至可以在同一按钮上添加多个 Activator，以极大扩展配置的可能性。

“Activation Type” 下拉列表定义了按钮的实际工作方式：

- Regular Press（常规按下）：按住时持续发送输出，松开停止，这是默认类型。
- Double Press（双击）：需要快速双按才生效，第二次按下时按住会持续输出；双击时间可调。
- Long Press（长按）：按住一定时长后开始输出；所需时长可调。
- Start Press（按下触发）：按下瞬间发送一次输出并立即失效（一次性触发）。
- Release Press（释放触发）：松开时发送一次输出并立即失效（一次性触发）。
- Chorded Press（和弦按下）：要求另一个按钮先被按住并保持，当两个条件同时满足时才输出；任意一个按钮松开则停止输出。
- Analog / Soft Press（有限可用性）：用于模拟扳机软拉或外环绑定等模拟输入，可调起始/结束范围或阈值，并保留一定的触觉设置。

下方还有其它设置，影响绑定被触发后的行为，例如：

- Double Tap Time（双击时间）
- Long Press Time（长按时长）
- Chorded Button（和弦按钮选择）
- Toggle（切换模式，将瞬时按键变为开关）
- Interruptible（可被中断，影响与长按/双击的优先级）
- Fire Start/End Delay（触发延迟）
- Haptics Intensity（触觉强度，仅在支持设备上生效）
- Cycle Binding（轮换绑定）
- Hold To Repeat / Turbo（按住重复）
- Repeat Rate（重复频率）

（文中还包含若干使用建议与注意事项，例如 Toggle 可能导致与游戏对相同输入的多重识别冲突、Interruptible 用于模拟比如冲刺与闪避的差异行为等。）

## 第 04b 章：Modeshifts（模式切换）

Modeshift 示例：右摇杆默认控制视角，但按住左肩时切换为径向菜单用于武器选择。每个可使用输入风格的设备最多只能配置一个 Modeshift，设置位于输入风格的右侧顶端。

Mode Shift 配置包含两个关键项：目标输入风格与 Mode Shift Button（触发该模式的按键）。设置后按住该按键即可在该输入设备上临时启用新的输入风格。

建议把 Modeshift 留给高优先级用途（如武器轮），并在为 Mode Shift 按键添加激活器（如 Long Press + EMPTY）时注意使用 interruptible 来避免误触。

## 第 04c 章：Action Sets（动作集合）

Action Sets 允许你在同一配置内打包多套控制方案，适用于不同角色、菜单与游戏内上下文。可以在配置概览页面通过“Add Action Set”添加新集合，并可复制现有集合作为起点。

Action Set 可自动切换（例如在显示光标时切换到菜单集合），但若游戏不支持或你想用于其它目的，可通过“Change Action Set”绑定手动切换。

切换时可选择显示提示与触觉反馈（Beep on Change）。

## 第 04d 章：Action Layers（动作层）

Action Layers 是介于 Sets 与 Modeshifts 之间的工具：比 Modeshift 更长期、比 Set 范围更小。每个 Set 可拥有自己的 Layer，用于对少数输入进行临时修改。

Layer 的创建、应用与移除通过配置概览与绑定完成。Layer 的 Activators 行为更受限：进入 Layer 的 Activators 页面时大多数选项会被灰显，仅能添加 Activator，并决定是覆盖基集的 Activators 还是复制它们到 Layer。

Layer 的应用有 3 种绑定方式：Hold（按住生效）、Apply（应用，需要手动移除）、Remove（移除）。对可能导致“卡住”的场景有建议的工作流（如在 Release Press 上放置 Remove Action Layer）。

## 总结与建议

Action Layers 和其它工具都很强大，但并非万能。作者建议秉持“简单就是稳健”的原则：优先使用更简单的方案（chorded activators、modeshifts、sets），仅在必要时使用 layers 并保持数量最少。

```
