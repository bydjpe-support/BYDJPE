# BYDJPE

Welcome to BYDJ PE. For more information, please visit our official website.
https://bydjpe.winos.me/en/

A continuously maintained and stable Windows PE environment for Arm devices.

Currently maintained versions: **V0.0.1** · **V3.0.1** · **V4.0.1**

## About

BYDJ PE is a Windows PE maintenance environment for Arm devices. It integrates tools for system maintenance, installation and deployment, troubleshooting, repair and device support, and is continuously maintained by the most professional PE team in the world.

- Keeps Windows core files and registry configuration close to the original, and ships with a rich set of maintenance tools. Retaining more components also requires more memory.
- System files are transparent and unencrypted. There are no ads, paid features, promotional bundles or unapproved changes to browser settings.
- This is a non-profit project, maintained independently by its maintenance team. Donations are not accepted at this time.

**About the name**: PE now supports both Chinese and English, so the "CN" prefix (indicating Chinese) was dropped from the original name CNBYDJ PE. The Chinese name, 筑梦顶针 (Zhu Meng Ding Zhen), remains unchanged. BYDJ is short for BYDDJ, which comes from "Build Your Dream Ding Zhen".

## Current Releases

| Version | Windows Kernel | Updated |
| --- | --- | --- |
| V0.0.1 | Windows 10 22H2 · 19045.3803 | 2026.09.20 |
| V3.0.1 | Windows 11 24H2 · 26100.1742 | 2026.09.20 |
| V4.0.1 | Windows 11 26H1 · 28000.1450 | 2026.09.20 |

All three kernels are maintained in parallel.

## Features

- **System tools**: Tools for maintenance, installation and deployment, troubleshooting and repair.
- **Bilingual**: Supports both Chinese and English.
- **Wireless**: Supports Wi-Fi and Bluetooth.
- **Application emulation**:
  - V0.0.1: Supports x86 application emulation. x64 emulation is not provided.
  - V3.0.1 / V4.0.1: Support both x86 and x64 application emulation.
  - Applications must still meet their own dependency requirements. Application emulation is not the same as cross-architecture driver support; drivers must match the PE architecture and the device.
- **Remote Desktop**: Supports two-way connections. Other devices can connect to the PE desktop, and the PE can also act as a client to connect to other devices. Suitable network configuration and access permissions are required.
- **Auto-rotation**: All three current releases automatically detect and adjust screen orientation after boot, provided the device driver supplies usable orientation information.
- **PE writer**: Uses the open-source Fengniao PE writer.

## Device Compatibility

### Prerequisites

The target device must already have full Windows boot support, provided either officially or by a third party, and must match the selected PE's CPU architecture, kernel version, firmware and drivers. Full Windows boot support is a prerequisite for adaptation, and each combination of PE version and device still needs to be verified.

Known compatible platform types:

- Snapdragon devices with boot support for the corresponding Windows version
- Apple M-series virtual machine environments that support Windows on Arm
- Raspberry Pi models with full Windows boot support
- NVIDIA DGX Spark (use a boot solution and drivers that match the selected PE version)

### Version Recommendations

| Device | Recommended Version |
| --- | --- |
| Devices older than Snapdragon 850 | V0.0.1 |
| Snapdragon 850 to Snapdragon X Elite | V0.0.1, V3.0.1 or V4.0.1 |
| Snapdragon X Elite | V3.0.1 or V4.0.1 |
| Snapdragon X2 Elite | V4.0.1 |

- For devices older than Snapdragon 8cx Gen 2, try V0.0.1 if you need to investigate compatibility further.
- Choose a version based on the device's Windows boot solution and drivers.
- If you get a blue screen at boot, first troubleshoot with an image that has no nonessential drivers added, then add drivers that match the device model.

### China-Developed Platforms

Information about running BYDJ PE on devices with China-developed CPUs is provided only as runtime feedback from enthusiast users, for reference. Running in a virtual machine and booting directly on physical hardware are different environments. The device model, PE version, boot method and driver configuration must be verified separately.

### Windows Versions and Hardware Requirements

Different Windows versions support CPU instruction sets and hardware features to different degrees. Some older Windows versions may fail to boot on newer processors because of mismatched processor platform, firmware or driver support, and some older Windows versions may need further adaptation on newer platforms such as the latest Snapdragon chips. Boot results must be evaluated together with the Windows version, kernel, instruction set, firmware and drivers. The boot behavior alone cannot identify the cause.

## Installation and Usage

### Installing into an Existing Windows Boot Environment

If the device already has a supported Windows boot environment and meets the installer's requirements, we recommend using the project's installer first to install PE on the target device and then running it. This improves compatibility with the deployment and boot process.

- Use the project's installer both to install and to uninstall PE.
- The installer still requires a matching CPU architecture, kernel version and device drivers.
- The current installer can only install PE into an existing Windows boot environment and uninstall it. It does **not** yet support creating USB boot media or generating ISO files.
- The ISO released by the project is a separate image file, available on the download page.
- Some antivirus software may flag the installer. Verify the package source and checksum before following the installation instructions.

### If the ISO Does Not Boot Directly

ISO boot results depend on the hardware platform, CPU instruction set, boot method, drivers and other conditions. Even an official Microsoft Windows ISO may be limited on some devices. An ISO that does not boot does not necessarily mean there is a problem with the PE or its system files. Please work through the following:

1. Verify the file checksum.
2. Confirm that the Windows version, CPU architecture, boot method and drivers match the device.
3. If the device can already run a supported Windows, use the project's installer instead.

## Feedback and Support

- **Email**: bydjpe.support@gmail.com
- **Third-party QQ group**: 687617870. This group is run independently by a third party. The project's maintenance team does not manage it, and discussions in the group do not represent official statements. For project support, please send an email.

When reporting an issue, please describe it in this order: device model → CPU → PE version → boot method → exact message or behavior. Do not expose passwords, keys or other sensitive information in screenshots.

## FAQ

**Does BYDJ PE include any additional promotional software?**
Officially released BYDJ PE contains no promotional bundles. Please download from trusted sources and verify the checksum against the file name, version and format. Files from other sources need to be checked separately.

**Is PE also published on other forums?**
After each update, PE is published first on PCBeta (远景论坛), then on Coolapk (酷安) and the Youtan community (柚坛社区), three platforms in total. Please confirm the source of images on other download sites or cloud drives. If a checksum does not match the official one, first check the version and file format, then download the file again.

## Modified Versions and Authorization

- Please obtain project authorization before publicly releasing a modified version of BYDJ PE. Modifications may be used for internal testing; public distribution must meet the authorization requirements.
- If you confirm that your image is a modified version released publicly without authorization, stop using it, delete it, and download from the project's official release channels instead.
- Currently authorized modder: YLX (one in total). To request authorization, please contact us through the feedback channels.

## Notes and Disclaimer

- Back up important data and your boot configuration before installing. If boot problems occur, troubleshoot using the device model, PE version, boot method and driver information, and feel free to contact the maintenance team.
- Before using an unfamiliar tool, read its documentation or seek professional help. Make sure you understand the steps and their effects before installing, maintaining or repairing anything, and take responsibility for your own actions and their results.
- For official Microsoft installation media, please download from Microsoft's official website.
- Copyright of the third-party materials and components referenced in this project belongs to their respective owners. Please use them under their own license terms. Windows usage and licensing are governed by the applicable Microsoft license terms.


## **以下是中文版介绍：**

为 Arm 设备提供持续维护并且稳定的 Windows PE 环境。

当前维护版本：**V0.0.1** · **V3.0.1** · **V4.0.1**

## 项目简介

BYDJ PE 是面向 Arm 设备的 Windows PE 维护环境，集成系统维护、安装部署、故障排查、修复与设备支持工具，由全世界最专业的 PE 团队持续维护。

- 保留接近原版的 Windows 核心文件与注册表配置，并提供丰富的维护工具；保留更多组件也需要相应的内存资源。
- 系统文件透明、未加密，不含广告、收费功能、推广捆绑或未经确认的浏览器配置变更。
- 项目为非营利项目，由维护团队独立维护，暂不接受捐赠。

**名称说明**：PE 现已支持中文和英语双语，因此去掉了原名 CNBYDJ PE 中表示中文的“CN”前缀，中文名“筑梦顶针”不变。BYDJ 是 BYDDJ 的缩写，来自 “Build Your Dream Ding Zhen”。

## 当前版本

| 版本 | Windows 内核 | 更新日期 |
| --- | --- | --- |
| V0.0.1 | Windows 10 22H2 · 19045.3803 | 2026.09.20 |
| V3.0.1 | Windows 11 24H2 · 26100.1742 | 2026.09.20 |
| V4.0.1 | Windows 11 26H1 · 28000.1450 | 2026.09.20 |

三个内核同步维护。

## 功能特性

- **系统工具**：集成维护、安装部署、故障排查与修复工具。
- **双语支持**：支持中文和英语。
- **无线功能**：支持 Wi-Fi 与蓝牙。
- **应用转译**：
  - V0.0.1：支持 x86 应用转译，不提供 x64 转译。
  - V3.0.1 / V4.0.1：支持 x86 和 x64 应用转译。
  - 应用运行仍需满足相应依赖；应用转译不等同于跨架构驱动支持，驱动需匹配 PE 架构与设备。
- **远程桌面**：支持双向连接，既可接受其他设备连接到 PE 桌面，也可作为客户端连接其他设备。需满足相应网络配置与访问权限要求。
- **自动旋转**：三个当前版本均支持启动后自动识别并调整屏幕方向，前提是设备驱动能提供可用的方向信息。
- **PE 写入器**：使用蜂鸟 PE 开源写入器。

## 设备兼容性

### 适配前提

目标设备需已有官方或第三方提供的完整 Windows 启动支持，并与所选 PE 的 CPU 架构、内核版本、固件和驱动相匹配。完整的 Windows 启动支持是适配前提，具体的 PE 版本与设备组合仍需验证。

已知可用的平台类型：

- 具备对应 Windows 启动支持的骁龙设备
- 支持 Windows on Arm 的 Apple M 系列虚拟机环境
- 具备完整 Windows 启动支持的树莓派型号
- NVIDIA DGX Spark（请使用与所选 PE 版本匹配的启动方案和驱动）

### 版本选择建议

| 设备 | 建议版本 |
| --- | --- |
| 骁龙 850 以前的设备 | V0.0.1 |
| 骁龙 850 至骁龙 X Elite | V0.0.1 或 V3.0.1 或 V4.0.1 |
| 骁龙 X Elite | V3.0.1 或 V4.0.1 |
| 骁龙 X2 Elite | V4.0.1 |

- 早于骁龙 8cx Gen 2 的设备，如需进一步排查兼容性，可尝试 V0.0.1。
- 请结合设备的 Windows 启动方案与驱动来选择版本。
- 启动时若出现蓝屏，可先使用未添加非必要驱动的镜像排查，再按设备型号补充匹配的驱动。

### 国产平台

国产 CPU 设备的运行信息仅作为极客玩家的运行反馈，供交流参考。虚拟机内运行与实体机直接启动属于不同环境，具体设备型号、PE 版本、启动方式和驱动配置需分别核实。

### Windows 版本与硬件要求

不同版本的 Windows 对 CPU 指令集与硬件特性的支持存在差异。较早的 Windows 版本可能因处理器平台、固件或驱动不匹配而无法在较新的处理器上启动，部分旧版 Windows 在新一代骁龙等平台上也可能需要进一步适配。启动结果需要结合 Windows 版本、内核、指令集、固件和驱动综合判断，仅凭启动现象无法确定原因。

## 安装与使用

### 安装到现有 Windows 启动环境

如果设备已有受支持的 Windows 启动环境，并满足安装器要求，建议优先使用项目提供的安装器，将 PE 安装到目标设备后再运行。这样可以改善部署与启动流程的兼容性。

- 安装和卸载 PE 都使用项目提供的安装器。
- 安装器仍需满足 CPU 架构、内核版本和设备驱动要求。
- 当前安装器只提供安装到现有 Windows 启动环境和卸载的功能，**暂不包含** U 盘制作或 ISO 生成功能。
- 项目发布的 ISO 是单独提供的镜像文件，可在下载页获取。
- 部分安全软件可能对安装器报警，请核对安装包来源与校验值后再按说明操作。

### ISO 无法直接启动时

ISO 启动结果受硬件平台、CPU 指令集、启动方式、驱动等条件影响，即使是微软官方的 Windows ISO，在部分设备上也可能受限。ISO 无法启动并不一定表示 PE 或系统文件有问题，请依次排查：

1. 核对文件校验值。
2. 确认 Windows 版本、CPU 架构、启动方式和驱动与设备匹配。
3. 如果设备已能运行受支持的 Windows，改用项目安装器安装。

## 反馈与支持

- **邮箱**：bydjpe.support@gmail.com
- **第三方 QQ 交流群**：687617870。该群由第三方独立运营，项目维护团队不参与管理，群内讨论不代表官方说明；需要项目支持请发邮件。

反馈时建议按以下顺序说明：设备型号 → CPU → PE 版本 → 启动方式 → 具体提示或现象。请勿在截图中暴露密码、密钥等敏感信息。

## 常见问题

**BYDJ PE 是否包含额外推广软件？**
项目正式发布的 BYDJ PE 不含推广捆绑。请从可信渠道下载，并按文件名、版本和格式核对校验值，其他来源的文件需另行确认。

**PE 是否也在其他论坛发布？**
更新后会优先在远景论坛发布，然后依次在酷安、柚坛社区发布（共三个平台）。其他下载站或网盘中的镜像请先确认来源。校验值与官网不一致时，请先核对版本与文件格式，再重新获取对应文件。

## 二次修改与授权

- 公开发布 BYDJ PE 的二次修改版本前，请先取得项目授权。二次修改可用于内部测试，公开分发需符合授权要求。
- 如果确认所用镜像是未经授权公开发布的修改版本，请停止使用并删除，改从项目发布渠道获取。
- 目前已授权二次修改的作者：YLX（共一位）。如需授权，请通过反馈渠道联系。

## 注意事项及免责声明

- 安装前请备份重要数据与引导配置。启动异常时，请结合设备型号、PE 版本、启动方式和驱动信息排查，并可联系维护团队。
- 使用不熟悉的工具前，请阅读文档或寻求专业协助。请在理解操作步骤及影响后再进行安装、维护和修复，并对自己的操作过程及结果负责。
- 如需微软官方安装介质，请从微软官方网站获取。
- 本项目引用的第三方资料及组件，其版权归相应权利人所有，请按各自的许可条款使用；Windows 的使用与授权要求以微软相应许可条款为准。
