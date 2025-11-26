```markdown
# 7f：RetroArch 与使用 Steam 硬件的模拟基础

<<<<<<< Updated upstream
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
=======
## 指南期望

在开始之前说明：本指南尽量简洁，不会深入到每个模拟器的详细安装与调试。我们仅覆盖用 RetroArch 快速上手并让其与 Steam Input 正常挂钩的基础流程。

选择 RetroArch 是因为它高度通用、支持大量平台，并能通过不同的核心（cores）覆盖多个世代的模拟需求。本指南以 MS-DOS 的模拟为示例，既具有历史价值也在运行与映射上稍微复杂一些，能代表某些常见问题场景。

**注意**：由于本文撰写于 Steam Deck 发布之前，本指南暂不涉及在 SteamOS 上的安装细节。

## 免责声明

关于用于模拟的 BIOS 与 ROM 文件，请确保在本地法律与使用条款允许的前提下获取与使用。本 Wiki 不支持或鼓励盗版行为；本指南假定你是以合法方式获得需要的文件。

## 什么是 RetroArch？

RetroArch 是一个基于 Libretro 的开源前端，Libretro 是一个模块化的模拟系统，允许使用针对特定硬件设计的核心（core）。本指南以 Steam 版本的 RetroArch 为例进行说明。

### 安装 RetroArch

在 Steam 商店搜索 RetroArch 并安装（Steam 版已在撰写时正式发布）。安装后可在库中运行以确保运行时依赖安装完毕。

若你使用 32 位系统，请注意 Steam 版可能不支持并出现缺失可执行文件的问题；在此情形下请从官方或 GitHub 手动下载相应版本。

### 下载并安装 DOSBox Pure

示例中我们使用 DOSBox 的一个分支 DOSBox Pure（https://github.com/schellingb/dosbox-pure/releases）。Steam 版 RetroArch 的某些核心需手动下载并放入 RetroArch 的 `cores` 目录。

核心通常包含 `.dll`（或平台对应的二进制）与 `.info` 文件，`.dll` 放入 `cores` 目录，`.info` 放入同目录下的 `info` 文件夹中。完成后就能在 RetroArch 中加载该核心并挂载内容。

## 将游戏添加到 Steam

接下来介绍如何把 ROM（或已打包为 .zip 的 DOS 游戏）通过 Steam 快捷方式运行：

1. 在 Steam 左下角点击“+” → “Add a Non-Steam Game” → 若未列出 RetroArch，点击“Browse…”找到 `retroarch.exe` 并添加。
2. 在库中右键该快捷方式 → 属性，在“Launch Properties”里的目标（Target）中填写启动参数，格式示例：

```
"path\\to\\retroarch.exe" -L cores\\<corename>.dll "path\\to\\<romname>.zip"
```

将 `path\\to\\retroarch.exe`、`<corename>`（如 `dosbox_pure_libretro`）与 ROM 路径替换为实际路径即可。

为该快捷方式设置封面（推荐使用 `https://www.steamgriddb.com/` 获取海报与图标）能让库界面更美观。

## 在 RetroArch 中配置控制

确保 Steam Overlay 能在游戏中调出（Big Picture Overlay 对自定义控制更友好）。不同核心与游戏的默认映射差异很大，某些核心需要在 RetroArch 设置中指定设备类型。

关于 DOS 的模拟与模拟摇杆的设置：

* 在游戏运行后打开 RetroArch 快捷菜单（默认 F1 或手柄的 Start+Select），进入 Controls → Port 1 Controls
* 选择合适的虚拟摇杆类型（例如 “First DOS Joystick (2 Axes, 2 Buttons)”），并保存 Game Remap 文件以便复用
* 某些 DOS 游戏需要在程序内启用摇杆并进行标定；可能需按 `Scroll Lock` 激活游戏焦点以允许键盘控制

注意：并非所有 DOS 游戏都能良好绑定摇杆；遇到无法配置或校准失败的游戏时，可尝试其它 DOSBox 版本或查找游戏的开源移植。
>>>>>>> Stashed changes

```
