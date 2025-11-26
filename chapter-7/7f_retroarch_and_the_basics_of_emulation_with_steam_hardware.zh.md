```markdown
# 7f：RetroArch 与使用 Steam 硬件的模拟基础

## 本指南的预期

本指南尽量简短，不会深入到每个模拟器的具体安装细节。本节示例使用 RetroArch，因其高度通用且覆盖大量机种。

示例将包括如 MS-DOS 等系统的模拟，重点在于如何启动 RetroArch 并让它与 Steam Input 正确挂钩。

**注意**：本文编写于 Steam Deck 发布前，暂不覆盖 SteamOS 上的安装细节。

## 免责声明

请确保你在本地合法拥有用于模拟的 BIOS 与 ROM 文件。Steam Input Wiki 不支持违法或侵权行为。

## 什么是 RetroArch？

RetroArch 是 Libretro 的前端，支持通过核心（cores）加载不同平台的模拟器。本指南使用 Steam 商店版 RetroArch 的流程，并说明如何添加核心与与 Steam 配合使用的基本步骤。

### 安装 RetroArch

在 Steam 商店搜索 RetroArch 并安装。若需安装额外核心，可在 DLC 页面或按本指南手动下载核心文件。

### 为 DOSBox Pure 安装核心（示例）

从项目的 Releases 页下载核心（.dll 和 .info），将 .dll 放入 RetroArch 的 cores 目录，并将 .info 放入 cores 的 info 子目录，随后即可在 RetroArch 中加载该核心。

### 将游戏加入 Steam

通过 Steam 添加非 Steam 快捷方式并在其属性的 Launch Options 中填写 RetroArch 的命令行参数以指定核心与 ROM，例如：

```
"path\to\retroarch.exe -L cores\<corename>.dll "path\to\<romname>.zip""
```

根据实际路径替换占位符。

### 在 RetroArch 中配置控制

启动游戏后打开 RetroArch 的快捷菜单（默认 F1 或 Start+Select），进入 Controls → Port 1 Controls，为模拟的端口选择合适的设备类型并按需保存 Remap 文件。

不同核心与游戏的支持差异较大，有时需要针对每款游戏单独调校模拟摇杆或按键。

```
