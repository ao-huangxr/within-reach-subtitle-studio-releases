# Within Reach Subtitle Studio

Official macOS and Windows downloads, Sparkle feed, and WinSparkle feeds.

本仓库用于：

- 官方软件下载安装；
- Release Notes；
- Sparkle / WinSparkle 自动更新 Feed；
- SHA256 校验；
- Build Manifest。

当前公开版本为 **Within Reach Subtitle Studio 0.1.0 Beta 4 / Build 7**。
本软件仍处于 Beta 阶段，仅支持 Apple Silicon，系统要求为 macOS 26.0
或更高。发布的应用经过 Developer ID 签名和 Apple Notarization；这不表示
软件已成为稳定正式版。

Beta 4 默认使用 packet-sparse qtrle 快速导出，支持完整时间线、当前
Segment、选中的多个 Segment 和全部 Segment；Compatibility Mode 继续提供传统
True-CFR qtrle。DaVinci Resolve 可能把 Sparse 素材显示为非项目帧率，或对部分
素材创建略短的 TimelineItem；严格逐帧和尾端长度工作流请使用 Compatibility。
DaVinci Resolve 自动时间线创建当前仍以完整工程为单位，Segment 时间线自动创建
尚未支持。

## Windows Beta

本仓库同时提供 macOS 和 Windows 版本。macOS 使用 Sparkle 更新，Windows
使用 WinSparkle 签名在线更新。当前 Windows 公开测试版为 **Within Reach
Subtitle Studio 0.1.0 Beta 4 / Build 9**，支持 Windows x64：

[下载 Windows Beta 4 Build 9 安装器](https://github.com/ao-huangxr/within-reach-subtitle-studio-releases/releases/download/windows-v0.1.0-beta.4-build9/Within-Reach-Subtitle-Studio-0.1.0-beta.4-build9-windows-x64-setup.exe)

Windows 安装器目前具有 WinSparkle EdDSA 更新签名，但尚未使用
Authenticode 签名。Windows 可能显示未知发布者或 SmartScreen 提示。
Build 10 prerelease 仅供内部在线更新测试，不通过普通用户的 Production
Feed 提供。

源代码不在本仓库公开。Bug 反馈请使用本仓库的
[Issues](https://github.com/ao-huangxr/within-reach-subtitle-studio-releases/issues)。
