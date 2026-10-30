# sdvmm · 星露谷物语模组管理器

Windows 上管理《星露谷物语》SMAPI 模组的工具：扫描、启用/停用、安装、卸载、检查更新、体检、搜索与中文名。

> 本仓库只用于**分发发布包**（源代码不公开）。下载请到
> [Releases](https://github.com/autism-0626/Sdvmm_Release/releases) 页面。

## 下载：三种选一个

| 文件 | 大小 | 说明 |
|---|---|---|
| **`sdvmm-<版本>-win-x64.exe`** | 约 69 MB | **单文件图形版**，不需要装 .NET、不用解压，双击即用 —— 推荐 |
| `sdvmm-<版本>-win-x64-selfcontained.zip` | 约 69 MB | 不需要 .NET，解压即用；含图形界面 + 命令行 |
| `sdvmm-<版本>-win-x64.zip` | 约 0.6 MB | 需要 **.NET 8 桌面运行时**；含图形界面 + 命令行 |

> 单文件 exe 只带图形界面。要用命令行（`sdvmm.exe`）请下载两个压缩包之一。

要求：Windows 10/11 x64。改模组前**关掉游戏**，否则文件被占用会失败。

## 校验下载

每个 Release 都附一份 `SHA256SUMS.txt`。下载后核对：

```powershell
Get-FileHash .\sdvmm-1.9.0-win-x64.exe -Algorithm SHA256
```

和文件里那一行比对即可。也可以在 Releases 页面直接看 GitHub 为每个资产计算的 SHA256。

## 第一次使用

1. 双击打开，程序会自动找游戏目录（Steam 库 / GOG / 注册表）
2. 找不到就用「文件 → 选择 Mods 文件夹…」手动选一次，之后会记住
3. 列表里出现模组就说明接上了

## 主要功能

| 功能 | 说明 |
|---|---|
| 启用 / 停用 | 停用会把文件夹移到 `Mods.disabled`，SMAPI 一定加载不到 |
| 卸载 | 移到 `Mods.removed` 隔离区（带时间戳），`--purge` 才真删 |
| 安装 | 拖入 zip 即可，装前校验整包，重复安装会被拒绝 |
| 检查更新 | GitHub 的模组可全程免浏览器；Nexus 的会打开下载页并监控下载目录 |
| 体检 | 查重复 UniqueID、缺前置、缺 DLL、依赖环 |
| 搜索 | 本地已装 + SMAPI 清单 + Nexus 三路合并，支持按 Nexus 数字 ID 搜 |
| 中文名 | 打开即显示中文名，查不到时自动翻译并写回对照表，之后离线可用 |
| 模组组 | 把一组模组存成清单，压缩成一串口令发给别人，导入后自动补齐缺的 |

命令行：

```text
sdvmm list | check | install <zip> | enable/disable <组> | update | smapi status
sdvmm catalog search <关键词>
sdvmm nexus search <关键词>
sdvmm groups list|show|create|export|import|install
sdvmm settings
```

完整用法见程序内「帮助 → 使用说明」。

## 界面预览

发布包内自带。截图会随版本更新补在 Release 说明里。

## 更新日志

见 [CHANGELOG.md](CHANGELOG.md)，或到 [Releases](https://github.com/autism-0626/Sdvmm_Release/releases) 看每个版本的完整说明。

## 反馈

- 有问题请开 [Issue](https://github.com/autism-0626/Sdvmm_Release/issues)，附上「帮助 → 导出诊断信息」产出的文件夹
- 崩溃排查：程序会记录崩溃原因、日志位置和崩溃前最近的操作

## 许可

[MIT](LICENSE)
