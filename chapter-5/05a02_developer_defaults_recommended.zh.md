```markdown
# 05a02：开发者默认 / 官方推荐（Developer Defaults / Recommended）

<<<<<<< Updated upstream
Valve 鼓励开发者为其游戏提供默认/推荐配置，作为玩家首次启动时的默认配置。理想情况下，该配置应能使任何启用了 Steam 控制器支持的控制器立即可玩。

开发者也可以提供多套配置：选择其中一套作为默认，其它作为可供玩家快速切换的备选方案。

在配置概览页底部点击“Browse Configs”可进入“Controller Configurations - Import”页面，默认会选中 Recommended 分类，其中会展示开发者提供的默认/推荐配置。

注意：拥有 Developer Default 并不等同于实现 SIAPI（Steam Input API），但实现 SIAPI 的游戏通常会包含默认/推荐配置。

有两类 Developer Default：

* 开发者针对不同控制器精心制作的配置（示例：FromSoftware 为《黑魂3》为 Steam 控制器制作了多个专用配置，利用其独特特性；某些作品为 Steam Controller 制作的配置会使用触摸板的模式切换等技巧）。
* 开发者若未定制配置，至少应选一个模板，系统会将该模板作为默认并放在 Recommended 分类（这虽然优于无配置，但并非最佳做法）。

如果开发者两者都未提供，系统将：

* 使用 Gamepad 模板作为默认，或
* 若存在社区配置，则默认选择评分最高的社区配置。
=======
Valve 鼓励开发者为其游戏提供一个默认/推荐配置，使玩家开箱即可使用控制器顺畅游玩。

开发者可提供多个配置，选定其中一个作为默认，其他配置供玩家在需要时选择。默认配置可极大提升玩家体验，尤其当开发者针对手柄特性进行了优化时。

在配置概览页点击“Browse Configs”可进入“Recommended”（推荐）类别，查看开发者提供的默认配置。

注意：提供 Developer Default 并不等同于实现完整的 SIAPI（Steam Input API），但若实现了 SIAPI，通常会随之提供相应默认配置。

有两类开发者默认：

* 开发者为不同控制器类型专门制作的配置（例如 Dark Souls 3 针对 Steam 控制器制作了 4 套配置，利用了双阶段触发等特色）
* 如果开发者未制作定制配置，Valve 建议至少选用一个模板作为默认；此时推荐会显示该模板

若开发者既未自制也未选模板，则会采用 Gamepad 模板或根据社区评分高的配置作为默认。
>>>>>>> Stashed changes

```
