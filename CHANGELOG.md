# 更新日志

每个版本的详细说明见对应的 Release 页面。

## [v1.14.0](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.14.0) —— 装完模组立刻提示缺前置，能自动的当场补齐

以前装完模组只显示"已安装"，缺前置要等你自己去体检页发现。现在安装结束就检查。

## [v1.13.1](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.13.1) —— 不再把"只有源码的 GitHub 仓库"当成能自动下载

补丁版：体检能查出缺前置，修复按钮也列出来了，但其中几个下载会失败：

## [v1.13.0](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.13.0) —— 语言包（i18n 翻译包）可以直接装了

新功能：像 `Ridgeside Village chinese-9247-2-5-17-1732449848.zip` 这种**没有 `manifest.json`、

## [v1.12.7](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.12.7) —— 更新后文件名跟版本走，旧文件彻底删除

补丁版：之前自动更新会**保留旧文件名**（`sdvmm-1.12.6-win-x64.exe` 里装着 1.12.7 的版本），

## [v1.12.6](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.12.6) —— 修复：下载好的版本名 exe 无法自动替换

补丁版：从发布页下载的文件名是 `sdvmm-1.12.2-win-x64.exe`，自动更新却提示

## [v1.12.5](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.12.5) —— 升级进度条：带百分比，且不会被提示挡住

补丁版：v1.12.4 加上了进度条，但发现两个问题，这次一起修：

## [v1.12.4](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.12.4) —— 自动升级时能看到进度

补丁版：程序自动更新时原来只有一句状态栏文字，下载几十 MB 期间看不出到底在动没动。

## [v1.12.3](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.12.3) —— 修复 Nexus 索引更新失败（422）

补丁版：启动时那条 `Nexus 索引更新失败：查询参数被拒绝` 是 Nexus 把搜索接口 v3 改了，

## [v1.12.2](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.12.2) —— 更新窗口不再撑满屏幕

补丁版：检查更新时弹出的窗口太大，长一点的更新说明能把窗口撑到半屏。现在是固定尺寸，

## [v1.12.1](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.12.1) —— 更新弹窗只说重点

补丁版：v1.12.0 的更新弹窗会把整篇更新说明塞进去（表格、代码块、Markdown 标记全在），

## [v1.12.0](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.12.0) —— 程序自己也能更新了

新功能：工具会检查自己的新版本，下载、校验、替换、重启一条龙，不用再手动去 Downloads 找新版。

## [v1.11.0](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.11.0) —— 只允许运行一个实例

新功能：重复启动不会开出第二个窗口，而是把已经在运行的窗口带到前台（在托盘里也一样）。

## [v1.10.1](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.10.1) —— 修复推荐页/搜索页翻译完成后不刷新

补丁版：自动补全中文名的结果要等到翻页或重新搜索才出现。现在完成的那一刻就会显示。

## [v1.10.0](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.10.0) —— 体检能修了，也能看游戏真正报了什么

这是这一轮最大的一次功能升级：体检从"只查"变成"能修"，并接上了游戏自己的日志。

## [v1.9.1](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.9.1) —— 支持 7z 等压缩包

补丁版：从 Nexus 下载的 7z 压缩包现在能被识别并安装。之前只认 zip，7z 下载完成后程序一直没反应。

## [v1.9.0](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.9.0) —— 状态栏消息分级

次版本：状态栏不再永久停留最后一条普通操作提示。普通提示和成功反馈会自动收起，警告、错误和进行中的操作继续保留。

## [v1.8.0](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.8.0) —— 按 Nexus 数字 ID 搜索

次版本：搜索框可以直接输入 Nexus 尾号 ID，本地模组、SMAPI 清单和 Nexus 索引条目都能匹配。

## [v1.7.0](https://github.com/autism-0626/Sdvmm_Release/releases/tag/v1.7.0) —— 模组组与分享口令

次版本：新增「模组组」功能 —— 把一组模组存成清单，压缩成一串口令发给别人，对方导入后自动补齐缺失的部分。
