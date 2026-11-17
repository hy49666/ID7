# MGU-CN-XIAOBAI

面向已装 MGU Store 的 BMW iDrive 主机。汉化署名为抖音「小白科技杂物社」、BiliBili「小白151」、GitHub [JackieZ123430](https://github.com/JackieZ123430)。

| 项目 | 收录内容 | 原版 GitHub | 汉化记录 |
| --- | --- | --- | --- |
| iDrive 7 Apps | 15 个应用，包括故障扫描、换挡提示、暖机监测、车辆数据和加速测试 | [cauliflowermossgrape/idrive7-apps](https://github.com/cauliflowermossgrape/idrive7-apps) | [汉化仓库](https://github.com/JackieZ123430/idrive7-apps-cn) · [#12](https://github.com/cauliflowermossgrape/idrive7-apps/pull/12) · [#22](https://github.com/cauliflowermossgrape/idrive7-apps/pull/22) · [#41](https://github.com/cauliflowermossgrape/idrive7-apps/pull/41) |
| BMW Apps | 15 个应用，包括车辆健康、行程、抬头显示、胎压与底盘相关应用 | [alexp50/bmw-apps](https://github.com/alexp50/bmw-apps) | [#3](https://github.com/alexp50/bmw-apps/pull/3) |
| Cluster Themes | 仪表主题选择与设置的简体中文界面 | [bimmer-lab/apps](https://github.com/bimmer-lab/apps) | [#13](https://github.com/bimmer-lab/apps/pull/13) |
| Spotify | 简体中文界面与中文媒体标题支持 | [hexlay/idrive7-custom-apps](https://github.com/hexlay/idrive7-custom-apps) | [#3](https://github.com/hexlay/idrive7-custom-apps/pull/3) |
| RideTube | 简体中文界面与设置 | [JustAnotherPU/ridetube](https://github.com/JustAnotherPU/ridetube) | [#3](https://github.com/JustAnotherPU/ridetube/pull/3) |
| BMW 天气 | 简体中文天气界面、设置和小组件 | [flash8523/bmw-weather-mgu](https://github.com/flash8523/bmw-weather-mgu) | [#1](https://github.com/flash8523/bmw-weather-mgu/pull/1) |
| MGU Browser | 简体中文界面与字体改动，应用按车机语言选择界面 | [pllanaio/mgu-browser](https://github.com/pllanaio/mgu-browser) | [#12](https://github.com/pllanaio/mgu-browser/pull/12) |
| Vizualyse iDrive Apps | 仪表投射、Chromium 浏览器、仪表主题、Moonlight 和车载 Steam | [Vizualyse/idrive-apps](https://github.com/Vizualyse/idrive-apps) | [中文源码](https://github.com/JackieZ123430/vizualyse-idrive-apps-cn) · [中文包](https://github.com/JackieZ123430/vizualyse-idrive-apps-cn/releases/tag/vizualyse-zh-cn.1) |
| mgu-apps | 精准计时、ECU 实时数据、DPF 监测（ID7） | [原版](https://github.com/giuseppesalatino-boop/mgu-apps) | [中文 README](https://github.com/JackieZ123430/mgu-apps/blob/fa79799e6a55113239ca9bdc3f88cc450cd17de7/README.zh-CN.md) · [汉化 PR](https://github.com/giuseppesalatino-boop/mgu-apps/pull/1) |
| MGU Store | 官方发行版，已收录中文译文并跟随车机语言 | [robertnisipeanu/mgu-store](https://github.com/robertnisipeanu/mgu-store) | [汉化 #57](https://github.com/robertnisipeanu/mgu-store/pull/57) · [收录 #63](https://github.com/robertnisipeanu/mgu-store/pull/63) |

目录中的 **微信 ppppphhjjj** 是联系条目。详情页仅显示联系方式，Store 会拒绝安装请求。

## 发布到 Gitee

将本目录中的文件提交到公开仓库的根目录，保留 `catalog.json`、`packages/` 和图标的相对位置。以 `main` 分支和 `MGU-CN-XIAOBAI` 仓库为例，在 MGU Store 的「软件源 → 添加软件源」中填入：

```text
https://gitee.com/xiaobai-151/mgu-cn-xiaobai/raw/main/catalog.json
```

发布后应先确认未登录时也能读取原始 JSON 和包文件，再到车机添加。部分组件保留 GitHub 上游下载地址，其中包含超出 Gitee 普通仓库单文件体积的 Chromium 引擎。车机安装这些项目或依赖时需能访问相应地址。

目录中的汉化安装包面向 ID7。安装包内保留原项目的应用 ID，并使用 MGU Store 支持的三段式版本号。同一 ID 的官方源和汉化源并存时，Store 可能优先选择较新版本或该应用原来的安装来源。添加源后可在来源详情中确认对应条目。

`provenance.json` 记录汉化构建版本和对应 GitHub 原项目或 PR。按 MGU Store 的发行格式打包，安装时由车机生成所需的 BMW OAP SDK。各应用及组件沿用原作者的许可。

电脑版 SSH 启用工具使用 Windows 桌面工具的安装方式。 [原版仓库](https://github.com/cauliflowermossgrape/idrive7-8-ssh-root) · [汉化 PR #4](https://github.com/cauliflowermossgrape/idrive7-8-ssh-root/pull/4)

## 2026-11-16 小组件相关更新

- EDrive助手更新至 2.9.2，实时数据更新至 1.0.13，使用上游 b2880634 的代码及已合并中文词条。
- 同步上游小组件内存画面缓存和实时数据温度单位设置，沿用现有汉化署名。
- 配套 GPU renderer 更新至 2.1.18，Controller gate 更新至 1.1.0。
- 已完成中文构建、小组件测试、实时数据测试和安装包校验，尚未车机实测。

## 汽水音乐 Beta 0.1.3

面向 BMW ID7。可从本源的 MGU Store 目录安装。请同时下载[电脑端 API 与接入说明](packages/qishui-beta-backend@0.1.3.zip)，自建本地后端后再从车机扫码登录。播放取决于上游提供的完整音频。

PowerBy 小白科技杂物社 · 免费应用请勿付费。
