```markdown
# 07a：将非 Steam 游戏添加到 Steam

为了让 Steam 的控制器配置生效，Steam Overlay 需要注入到游戏进程中。对于从其它来源启动的非 Steam 游戏，Steam 无法自动注入 Overlay。

最简单的解决方法是将该游戏添加到你的 Steam 库中并通过 Steam 启动，这样 Steam 会有机会挂入覆盖层，从而使控制器配置生效。

添加步骤：

* 在 Steam 客户端左下角点击 “Add A Game” → 选择 “Add A Non-Steam Game”
* Steam 会扫描已安装程序，若未列出则点击 “Browse…” 手动定位可执行文件
* 勾选要添加的程序并点击 “Add Selected Programs”
* 该程序将出现在你的库中；若要移除，右键该条目 → Manage → Remove non-Steam game from your library

注意：若该游戏在你购买的非 Steam 版本中实现了 SIAPI，原生配置不会生效（因为 SIAPI 属于 Steam 平台）。

```
