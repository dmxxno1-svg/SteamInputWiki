<<<<<<< Updated upstream
# 02b07：摇杆相机（Joystick Camera）

推荐观看：相关演示（待补充）

此输入风格用于需要摇杆输入但与 Joystick Move（02b06）不同的场景，拥有一组不同的选项与一个关键特性：自适应中心（Adaptive Centering）。

该风格仅可应用于：

* 触控板
* 陀螺

原因在于其内置的“自适应中心”功能。

#### 什么是自适应中心（Adaptive Centering）？

Adaptive Centering 会根据首次输入的位置动态改变死区（Dead Zone）的位置。

对于触控板来说，当你的拇指接触触控板时，死区会被重新定位到拇指下方；当你抬起再放下拇指时，死区再次移动到新的接触点下方。这种行为类似移动端游戏中的软件摇杆。

对于陀螺来说，当陀螺启用时，其当前旋转会被视为“中性”死区；每次禁用然后重新启用陀螺时，该中性点都会更新。

理论上，Adaptive Centering 可以显著减少触控板与陀螺的误触，帮助“找到中心”——这是触控板作为摇杆时常见的抱怨点。

## 共享设置

### 输出（Output）

选项：Left Joystick / Right Joystick / Relative Mouse。

注意：截至 2021-08-24，Joystick Camera 在输出 Relative Mouse 时似乎存在问题。

### 摇杆响应曲线（Stick Response Curve）

选项：Linear / Aggressive / Relaxed / Wide / Extra Wide。

### 模式切换（Mode Shifting）

设置按键将设备切换为其它输入风格（详见第 04 章）。

### 触觉强度（Haptics Intensity）

随虚拟摇杆倾斜强弱给出触觉提示，选项：Off / Low / Medium / High。

### 平滑摇杆（Smooth Joystick）

开/关。启用时在抬起拇指或禁用陀螺后，虚拟摇杆会有模拟的“回中”过渡，而非瞬时回中。

### 轴反转与灵敏度缩放

提供水平/垂直轴反转与垂直灵敏度缩放等设置。注意与游戏内设置的互相影响。

### 输出抗死区（Output Anti-Deadzone）与缓冲（Buffer）

用于抵消游戏端的死区并重新建立自定义死区。

### 鼠标灵敏度（Mouse Sensitivity）

当输出为相对鼠标时，设置相对鼠标的最大灵敏度。

## 触控板专用设置

### 点击操作（Click Action）

使用触控板点击触发绑定，常用于将摇杆点击分配为某个行为。

### 滑动时长（Swipe Duration）

当在触控板上滑动/弹动时，Joystick Camera 可将虚拟摇杆短时间维持在最大输出，随后再缓慢回中（由 Smooth Joystick 控制）。选项：Off / Low / Medium / High。

## 陀螺专用设置

### 陀螺启用按钮 / 行为

选择启用陀螺的按键，及其行为（On / Off / Toggle）。

### 陀螺转向轴（Gyro Steering Axis）

选项：Yaw / Roll，决定哪种旋转控制水平移动。

### 陀螺俯仰中性角（Gyro Pitch Neutral Angle）

设置被视为死区的俯仰角度，以适配持握姿态。

## 作者总体说明

笔者认为 Adaptive Centering 存在问题：Steam 的实现会在重新定位死区的同时重新缩放虚拟摇杆的输出范围，导致响应范围在不同接触点出现不一致（靠近边缘的一侧范围被压缩，远侧被放大）。这会让输出行为难以预期，从而降低一致性。

在陀螺上效果尤其糟糕：频繁改变的死区与动态缩放常使其需要异常大的旋转才能产生响应。

尽管如此，在某些场景下 Joystick Camera 仍有用武之地，例如将右触控板设为右摇杆并启用 Swipe Duration 与 Smooth Joystick，可将触控板用作“快转”输入，感觉比 Trackball 更自然且平滑。

总体上，Joystick Camera 缺少一些关键选项（如触摸/双击绑定、Rotation 设置），令其在很多场合无法替代 Mouse-like Joystick 或 Joystick Move，但在某些需要自适应中心与点击模式切换的特定配置中，它仍有独到用途。
=======
```markdown
# 02b07：摇杆摄像（Joystick Camera）

摇杆用于控制摄像机或视角旋转，常见于第三人称或需要自由视角的游戏。与移动用摇杆不同，摄像摇杆通常需要更高灵敏度和不同的曲线设置。

常见调整项：
- 水平/垂直灵敏度比（Sensitivity Vertical Scale）
- 限幅（Clamp）设置以防止过快旋转
- 平滑（Smoothing）及加速度（Acceleration）以调整手感

技巧：在对称的摄像控制中可微调垂直缩放以匹配玩家习惯。

```
>>>>>>> Stashed changes
