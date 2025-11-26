```markdown
# 06b02：为实现 SIAPI 的开发者提供的资源

作为玩家而非程序员，我能做的主要是链接 Valve 的官方实现文档，地址如下：

https://partner.steamgames.com/doc/features/steam_controller/getting_started_for_devs

此外，我从玩家角度总结了一些良好 SIAPI 实现的要点：

## 最佳实践（概要）

### 不推荐做法（中性/差）

* 仅机械地把 XInput 控制映射成 SIAPI，而没有调整以发挥 SIAPI 优势
* 没有为非 Steam 平台或非默认输入提供回退方案
* 不允许混合输入或不提供锁定/选择图标集的选项
* 将应为可绑定的动作硬编码成某种特定的输入风格

### 推荐做法（好）

* 为每个主要游戏上下文提供 Action Set 并保证自动切换可靠（建议不要滥用自动 Action Layers）
* 在每个上下文中提供完整且可绑定的动作集合，避免把相关但独立的动作合并为一个动作
* 包含 `absolute_mouse` 风格以支持触摸板 / 陀螺用户，若缺失请确保混合输入处理良好
* 利用 SIAPI 提供的原始数据实现创新特色（如自定义触觉、陀螺原生特性等）

```
