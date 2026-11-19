**English** | [简体中文](#bydj-pe-简体中文)

# BYDJ PE

A continuously maintained, stable Windows PE environment built for **Snapdragon, NVIDIA, and Arm** devices.

- **Official Website**: <https://bydjpe.winos.me/en/> | [简体中文](https://bydjpe.winos.me/)
- **Maintained Versions** (`2026.11.12`): **V0.0.3** · **V1.5.2** · **V3.0.3** · **V4.0.3** · **V4.0.3-VI**

## About & Features

BYDJ PE (*"Build Your Dream Ding Zhen"*, Chinese: **筑梦顶针**, formerly CNBYDJ PE) is a non-profit Arm Windows PE maintained by a 10+ member team. It keeps Windows core files and registry settings close to stock, transparent, and unencrypted—with no ads, paid features, bundles, or donations.

- **Installer**: Deploy to `C:` with a boot entry, inject drivers, build ISOs, or write to USB/external drives.
- **System & Connectivity**: Chinese/English switching, Wi-Fi, Bluetooth, audio, remote desktop, and auto screen rotation.
- **Accessibility (`V4.0.3-VI`)**: English default, built on V4.0.3 with NVDA screen reader, dark mode, black wallpaper, inverted pointers, and system sounds.
- **App Translation**: `V0.0.x` supports x86; all other versions support x86 & x64 (requires app runtime dependencies; does not support x86 drivers).

## Current Versions

| Version | Windows Kernel | Updated | Translation | Wallpaper (Version ID) |
| --- | --- | --- | --- | --- |
| **V0.0.3** | Win10 22H2 · 19045.3803 | 2026.11.12 | x86 | Snow mountains & autumn forest on a lake |
| **V1.5.2** | Win11 23H2 · 22631.2861 | 2026.11.12 | x86, x64 | Floating sea otter |
| **V3.0.3** | Win11 24H2 · 26100.1742 | 2026.11.12 | x86, x64 | Sunset waves, rocks & birds |
| **V4.0.3** | Win11 26H1 · 28000.1450 | 2026.11.12 | x86, x64 | Coastal beach & cliffs |
| **V4.0.3-VI** | Win11 26H1 · 28000.1450 | 2026.11.12 | x86, x64 | Solid black |

## Device Compatibility

Devices must support native Windows boot and match the selected PE's architecture, kernel, firmware, and drivers.

| Platform / CPU | Supported Versions |
| --- | --- |
| **Older than Snapdragon 850** | **V0.0.3** or **V1.5.2** (recommended) |
| **Snapdragon 850 – 8cx Gen 3** | **V0.0.3** – **V4.0.3-VI** |
| **Snapdragon X Elite** | **V3.0.3** (required), **V4.0.3** / **V4.0.3-VI** (compatible) |
| **Snapdragon X2 Elite & NVIDIA CPUs** | **V4.0.3** / **V4.0.3-VI** (required) |
| **Apple M-series VMs** | All maintained versions (**V0.0.3** – **V4.0.3-VI**) |

- **NVIDIA PCs**: Must inject required drivers before use (e.g., `nvgpio.inf.zip` for GB10 / DGX Spark).
- **Chinese-made CPUs** (Zhaoxin, Hygon, Phytium, etc.): Must be able to boot Windows natively; real-hardware behavior varies and requires physical testing.

## Usage & Troubleshooting

Only a ZIP package is provided—extract it and run the installer inside (standalone ISOs are no longer offered). Read the [website guide](https://bydjpe.winos.me/en/) first, verify checksums, and never reboot or force-close during installation.

- **VM ISO boot failure**: Email VM settings screenshots and physical machine specs.
- **Physical USB boot failure**: Use the built-in installer instead of third-party tools like Ventoy.
- **BSOD / freeze after driver injection**: Keep only basic drivers (storage, USB, keyboard/mouse/touchpad) and test incrementally.

## Support, Authorization & Disclaimer

- **Support**: `bydjpe.support@gmail.com` (include device model, CPU, PE version, boot method, and symptoms; hide sensitive info). *Third-party QQ group `687617870` is unofficial.*
- **Modifications**: Public redistribution of modified builds requires authorization (internal testing exempt); public videos/tutorials must credit **BYDJ PE**. Authorized modifier: **YLX**.
- **Disclaimer**: Download from official channels, verify checksums, and back up data/boot configs before use. Official Microsoft media and Windows licensing are governed by Microsoft's terms.

---

# BYDJ PE (简体中文)

为**骁龙、英伟达与 Arm** 设备提供持续维护、稳定可靠的 Windows PE 环境。

- **官方网站**：<https://bydjpe.winos.me/> | [English](https://bydjpe.winos.me/en/)
- **当前版本**（`2026.11.12`）：**V0.0.3** · **V1.5.2** · **V3.0.3** · **V4.0.3** · **V4.0.3-VI**

## 简介与特性

BYDJ PE（中文名**筑梦顶针**，原名 CNBYDJ PE，意为 *"Build Your Dream Ding Zhen"*）是由 10 人以上团队维护的非营利 Arm Windows PE。保留接近原版的系统文件与注册表，透明未加密，无广告、收费、捆绑及捐赠渠道。

- **一体化安装器**：支持安装进 `C` 盘并添加启动项、注入驱动、生成 ISO 或写入 U 盘/移动硬盘。
- **系统与连接**：支持中英双语切换、Wi-Fi、蓝牙、音频、远程桌面及自动旋转屏幕。
- **视障辅助版（`V4.0.3-VI`）**：基于 V4.0.3，默认英语与暗黑模式（纯黑壁纸+反色指针），内置 NVDA 读屏与系统提示音。
- **应用转译**：`V0.0.x` 支持 x86，其余版本支持 x86 与 x64（需满足应用运行库依赖，不支持安装 x86 驱动）。

## 当前版本

| 版本 | Windows 内核 | 更新日期 | 应用转译 | 壁纸主题（用于区分版本） |
| --- | --- | --- | --- | --- |
| **V0.0.3** | Win10 22H2 · 19045.3803 | 2026.11.12 | x86 | 湖面雪山与秋日森林 |
| **V1.5.2** | Win11 23H2 · 22631.2861 | 2026.11.12 | x86、x64 | 水面仰躺的海獭 |
| **V3.0.3** | Win11 24H2 · 26100.1742 | 2026.11.12 | x86、x64 | 夕阳海浪、礁石与飞鸟 |
| **V4.0.3** | Win11 26H1 · 28000.1450 | 2026.11.12 | x86、x64 | 俯瞰海岸沙滩与悬崖 |
| **V4.0.3-VI** | Win11 26H1 · 28000.1450 | 2026.11.12 | x86、x64 | 纯黑背景 |

## 设备兼容性

设备需具备完整的 Windows 启动支持，且与所选 PE 的架构、内核、固件和驱动匹配。

| 平台 / 处理器 | 推荐 / 支持版本 |
| --- | --- |
| **早于骁龙 850** | 推荐 **V0.0.3** 或 **V1.5.2** |
| **骁龙 850 至 8cx Gen 3** | **V0.0.3** – **V4.0.3-VI** |
| **骁龙 X Elite** | **V3.0.3**（必选），**V4.0.3** / **V4.0.3-VI**（可用） |
| **骁龙 X2 Elite、英伟达系列 CPU** | **V4.0.3** / **V4.0.3-VI**（必选） |
| **Apple M 系列虚拟机** | 当前所有版本（**V0.0.3** – **V4.0.3-VI**） |

- **英伟达电脑**：使用前必须按官网教程注入对应驱动（如 GB10 / DGX Spark 需安装 `nvgpio.inf.zip`）。
- **国产处理器**（兆芯、海光、飞腾等）：前提是本身可启动 Windows，实机表现需以实测为准。

## 使用与排查

仅提供 ZIP 压缩包，解压后运行内置安装器即可（不再单独提供 ISO）。使用前请阅读[官网](https://bydjpe.winos.me/)说明并核对校验值，操作中请勿重启或强制关闭安装器。

- **虚拟机 ISO 无法启动**：请附带虚拟机配置截图与物理机配置信息发邮件排查。
- **物理机 U 盘启动失败**：若 Ventoy 等第三方工具无法引导，请改用自带安装器制作启动盘。
- **注入驱动后蓝屏/卡死**：先仅保留硬盘、USB 及键鼠/触控板等基础驱动排查。

## 支持、授权与免责声明

- **反馈支持**：`bydjpe.support@gmail.com`（请附设备型号、CPU、PE 版本、启动方式及现象，勿暴露敏感信息）。*第三方 QQ 群 `687617870` 非官方运营。*
- **二改与署名**：未经许可禁止公开发布二改版（内部测试除外）；公开视频、教程、测评须明确标注 **「BYDJ PE」**。已授权作者：**YLX**。
- **免责声明**：请从官方渠道下载并核对校验值，操作前备份数据与引导。微软官方介质及 Windows 授权以微软条款为准。
