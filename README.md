**English** | [简体中文](#bydj-pe-简体中文)

# BYDJ PE

Welcome to BYDJ PE. For more information, please visit our official website: <https://bydjpe.winos.me/en/>

A continuously maintained, stable Windows PE environment for Arm devices.

Currently maintained versions: **V0.0.2** · **V1.5.1** · **V3.0.2** · **V4.0.2**

## About

BYDJ PE (Chinese name "筑梦顶针") is a Windows PE for Arm devices. It bundles tools for system maintenance, deployment and repair, and is maintained by a professional team of more than 10 people.

- Keeps the Windows core files and registry configuration close to the original; system files are transparent and unencrypted.
- No ads, paid features or bundled promotions. A non-profit project that does not currently accept donations.
- Formerly named CNBYDJ PE; the "CN" prefix was dropped because the PE now supports both Chinese and English. BYDJ comes from "Build Your Dream Ding Zhen".

## Current Versions

| Version | Windows kernel | Updated |
| --- | --- | --- |
| V0.0.2 | Windows 10 22H2 · 19045.3803 | 2026.10.30 |
| V1.5.1 | Windows 11 23H2 · 22631.2861 | 2026.10.30 |
| V3.0.2 | Windows 11 24H2 · 26100.1742 | 2026.10.30 |
| V4.0.2 | Windows 11 26H1 · 28000.1450 | 2026.10.30 |

The wallpaper changes with every update, so you can use it to tell versions apart.

## Features

- Installer: install to system, add drivers, generate ISO, write to USB drive
- Chinese and English, Wi-Fi, Bluetooth, remote desktop, auto screen rotation
- App translation: V0.0.x supports x86; the other versions support x86 and x64 (this does not mean cross-architecture drivers can be installed)

## Device Compatibility

The device must already have complete Windows boot support, and it must match the selected PE's architecture, kernel, firmware and drivers.

| Device | Recommended version |
| --- | --- |
| Before Snapdragon 850 | V0.0.2 |
| Snapdragon 850 to 8cx gen3 | Any version |
| Snapdragon X Elite | V3.0.2 or V4.0.2 |
| Snapdragon X2 Elite | V4.0.2 |

If you get a blue screen at boot, first test with an image that has no unnecessary drivers added, then add the matching drivers. Run reports for China-made CPUs are community feedback only, for reference.

## Installation and Use

Only the ZIP is provided. Extract it and use the installer inside; a separate ISO is no longer offered. Before use, read the installer guide and turn off your antivirus software. Do not restart the computer or force-close the installer during an operation, or the boot configuration and PE files may be damaged.

If the ISO will not boot: verify the checksum → confirm the version, architecture, boot method and drivers match the device → if the device can already run Windows, use the installer instead.

## Feedback and Support

- Email: bydjpe.support@gmail.com
- Third-party QQ group: 687617870 (not run by the project; its content is not official, and for support please send an email)

When reporting an issue, include: device model, CPU, PE version, boot method and the exact symptoms. Do not expose passwords or other sensitive information in screenshots.

## Modifications and Authorization

Obtain authorization before publicly releasing a modified version of BYDJ PE (internal testing excepted). If you find an unauthorized modified image, stop using it and get the PE from the project's official channels. Authorized modifier: YLX.

## Notes and Disclaimer

- Download from trusted sources and verify the checksum.
- Back up your data before any operation, follow the instructions strictly, and take responsibility for your own actions and their results.
- Get official Microsoft installation media from Microsoft's website. Third-party materials and components belong to their respective owners; use of Windows is governed by Microsoft's license terms.

---

# BYDJ PE (简体中文)

欢迎使用 BYDJ PE，更多信息请访问我们的官网：<https://bydjpe.winos.me/>

为 Arm 设备提供持续维护、稳定可靠的 Windows PE 环境。

当前维护版本：**V0.0.2** · **V1.5.1** · **V3.0.2** · **V4.0.2**

## 项目简介

BYDJ PE（中文名“筑梦顶针”）是面向 Arm 设备的 Windows PE，集成系统维护、安装部署与故障修复工具，由 10 人以上的专业团队持续维护。

- 保留接近原版的 Windows 核心文件与注册表配置，系统文件透明、未加密。
- 不含广告、收费功能或推广捆绑；非营利项目，暂不接受捐赠。
- 原名 CNBYDJ PE，因支持中英双语而去掉“CN”。BYDJ 来自 “Build Your Dream Ding Zhen”。

## 当前版本

| 版本 | Windows 内核 | 更新日期 |
| --- | --- | --- |
| V0.0.2 | Windows 10 22H2 · 19045.3803 | 2026.10.30 |
| V1.5.1 | Windows 11 23H2 · 22631.2861 | 2026.10.30 |
| V3.0.2 | Windows 11 24H2 · 26100.1742 | 2026.10.30 |
| V4.0.2 | Windows 11 26H1 · 28000.1450 | 2026.10.30 |

每次更新都会更换壁纸，可借此区分版本。

## 功能特性

- 安装器：安装进系统、添加驱动、生成 ISO、写入 U 盘
- 中英双语、Wi-Fi、蓝牙、远程桌面、自动旋转屏幕
- 应用转译：V0.0.x 支持 x86，其余版本支持 x86 和 x64（不等于能安装跨架构驱动）

## 设备兼容性

设备需已有完整的 Windows 启动支持，并与所选 PE 的架构、内核、固件和驱动匹配。

| 设备 | 建议版本 |
| --- | --- |
| 骁龙 850 以前 | V0.0.2 |
| 骁龙 850 至 8cx gen3 | 任意版本 |
| 骁龙 X Elite | V3.0.2 或 V4.0.2 |
| 骁龙 X2 Elite | V4.0.2 |

启动蓝屏时，先用未添加非必要驱动的镜像排查，再补充匹配的驱动。国产 CPU 的运行信息仅为玩家反馈，仅供参考。

## 安装与使用

只提供 ZIP，解压后用其中的安装器即可，不再单独提供 ISO。使用前请阅读使用须知并关闭杀毒软件；操作中请勿重启或强制关闭安装器，否则可能损坏系统引导和 PE 文件。

ISO 无法启动时：核对校验值 → 确认版本、架构、启动方式和驱动匹配 → 若设备能运行 Windows，改用安装器。

## 反馈与支持

- 邮箱：bydjpe.support@gmail.com
- 第三方 QQ 群：687617870（非官方运营，内容不代表官方；需要支持请发邮件）

反馈时请说明：设备型号、CPU、PE 版本、启动方式、具体现象。截图请勿暴露密码等敏感信息。

## 二次修改与授权

公开发布二次修改版前，请先取得授权（内部测试除外）。如发现未经授权的修改版，请停止使用，改从项目渠道获取。已授权作者：YLX。

## 注意事项及免责声明

- 请从可信渠道下载并核对校验值。
- 操作前请备份数据，严格按说明操作，并对自己的操作及结果负责。
- 微软官方安装介质请从微软官网获取。第三方资料及组件的版权归其权利人所有；Windows 的使用与授权以微软许可条款为准。
