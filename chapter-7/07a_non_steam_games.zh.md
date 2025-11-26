```markdown
# 07a：将非 Steam 游戏添加到 Steam

<<<<<<< Updated upstream
为了让 Steam 的控制器配置生效，Steam Overlay 需要注入到游戏进程中。对于从其它来源启动的非 Steam 游戏，Steam 无法自动注入 Overlay。

最简单的解决方法是将该游戏添加到你的 Steam 库中并通过 Steam 启动，这样 Steam 会有机会挂入覆盖层，从而使控制器配置生效。

添加步骤：

* 在 Steam 客户端左下角点击 “Add A Game” → 选择 “Add A Non-Steam Game”
* Steam 会扫描已安装程序，若未列出则点击 “Browse…” 手动定位可执行文件
* 勾选要添加的程序并点击 “Add Selected Programs”
* 该程序将出现在你的库中；若要移除，右键该条目 → Manage → Remove non-Steam game from your library

注意：若该游戏在你购买的非 Steam 版本中实现了 SIAPI，原生配置不会生效（因为 SIAPI 属于 Steam 平台）。
=======
要让 Steam 的控制器配置生效，Steam Overlay 必须能够挂钩（hook）到游戏。如果你从别处启动游戏（例如很多非 Steam 游戏的情况），Steam 无法注入 Overlay。

最简单的解决办法是将该游戏添加到你的 Steam 库并从 Steam 启动。这样 Steam 就能挂钩游戏并提供 Overlay，从而大多数情况下允许 Steam 的控制器配置对该游戏生效。

添加非 Steam 游戏的步骤：

* 在 Steam 客户端左下角点击“Add A Game”
* 选择“Add A Non-Steam Game”
* Steam 会扫描已安装的程序
  * 如果要添加的游戏未在列表中，点击“Browse…”并定位到游戏安装目录
* 勾选要添加的程序/游戏
* 点击“Add Selected Programs”完成添加
* 之后这些游戏会显示在你的 Steam 库中；若要移除，右键该游戏 → 管理 → 从库中移除非 Steam 游戏

注意：如果某款游戏实现了 Steam Input API（SIAPI），但你是在非 Steam 平台购买的该游戏，则原生配置不可用，你需要使用更基础的配置选项，因为 SIAPI 属于 Steam 平台特性，非 Steam 版本无法提供该支持。
>>>>>>> Stashed changes

```
