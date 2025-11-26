```markdown
# 05a01：模板（Templates）

<<<<<<< Updated upstream
模板是可以随时应用的通用配置。

它们有助于快速让某款游戏以手柄可玩为基准，但由于模板通常按流派而非具体游戏设计，可能缺少针对某款游戏的细节配置，因此适合作为配置开发的起点。

在配置概览页面可找到模板：点击底部的 “Browse Configurations” 进入“Controller Configurations - Import” 页面，左侧列表中可选择 Templates 分类。

## 默认模板

有些模板为共享模板，有些则根据你使用的控制器不同而不同。

### 所有控制器共享：

- Gamepad：一个“无花哨”的配置，把控制器按 Xbox 风格配置为纯手柄输入，最常见的手柄兼容方案。
  * 对于 Sony 控制器，触摸板以分割模式并复制 Start/Select。
- Keyboard (WASD) and mouse：将控制器映射为键盘鼠标输入（适用于不原生支持手柄的游戏），模板基于 FPS 常见键位。
  * 左摇杆使用方向键（Directional Pad）输入风格并绑定为 WASD
  * 右摇杆使用 Joystick Move（相对鼠标）输出
  * 对于 Sony 控制器，触摸板处于统一模式并使用鼠标输入风格

### DualShock 4 / DualSense 与 Switch Pro 共享：

- Gamepad with Flick Stick：在 Gamepad 模板基础上，右摇杆改为 Flick Stick，陀螺设为鼠标输入，用于需要精确瞄准并支持混合输入的游戏。

### DualShock 4 / DualSense 与 Steam Controller 共享：

- Gamepad with high precision camera/aim：与 Gamepad 模板类似（Steam 控制器的右触摸板被设为鼠标以提升瞄准）
- Gamepad with mouse and gyro：在 Gamepad 模板上启用陀螺为鼠标输入，便于精确瞄准

### 仅 Steam Controller：

- Gamepad with Camera Controls：将右触摸板设为 Mouse-Joystick（鼠标-摇杆）输入风格，用于不支持混合输入但仍希望更好相机控制的游戏。

## 个人模板

你也可以导出自己的模板以便在同类游戏间快速复用。导出流程：配置概览页点击“Export Config” → 选择 Templates 分类 → 保存为新的模板并填写名称与简介。

导出后模板会出现在导入页面的 Templates 列表中，便于将个人化的起始配置快速应用到其它同类游戏。
=======
模板是可随时应用的通用配置，通常按游戏类型（而非具体游戏）设计，因此能快速提供一个可玩的基线，但可能缺少针对某款游戏的特定键位。

在配置概览页点击“Browse Configurations”可进入导入页面，左侧列表中可选择 Templates 类别以浏览官方与共享模板。

## 默认模板（Default Templates）

部分模板跨设备共享，部分根据控制器类型定制。

### 所有设备共享：

* Gamepad——“简洁”配置，把控制器当作 Xbox 控制器（最常见的支持格式），仅使用手柄输入。
* Keyboard (WASD) and mouse——为不支持手柄的游戏提供键鼠输入的基础配置，常用于第一人称射击。

### DualShock 4 / DualSense 与 Switch Pro 共享：

* Gamepad with Flick Stick——基于 Gamepad 模板，把右摇杆设为 Flick Stick，且启用陀螺以提升瞄准精度。

### DualShock 4 / DualSense 与 Steam Controller 共享：

* Gamepad with high precision camera/aim 与 Gamepad with mouse and gyro——为需要精确视角控制的游戏启用触控板或陀螺作为鼠标样式。

### 仅限 Steam Controller：

* Gamepad with Camera Controls——将右触控板设为 Mouse-Joystick 样式以在不支持混合输入的游戏中仍保留类似鼠标的摄像手感。

## 个人模板（Personal Templates）

你也可以导出自己定制的模板并保存在 Templates 类别，便于在同类型游戏间快速复用。

在配置概览页点击“Export Config”，选择 Templates 类别并保存为新模板，之后可在导入时直接使用该模板作为起点。
>>>>>>> Stashed changes

```
