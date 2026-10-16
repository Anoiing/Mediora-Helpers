# Mediora Helpers

Mediora 的 Emby 与 Jellyfin 助手安装包下载仓库。

**[打开下载页](https://github.com/Anoiing/Mediora-Helpers/releases)**

## 选择安装包

| 媒体服务器 | Release 标签 | 下载文件 |
| --- | --- | --- |
| Emby | `emby-helper-vX.Y.Z` | `mediora-emby-helper-X.Y.Z.zip` |
| Jellyfin | `jellyfin-helper-vX.Y.Z` | `mediora-jellyfin-helper-X.Y.Z.zip` |

同时下载 ZIP 和同名 `.sha256` 文件，在同一目录运行 `shasum -a 256 -c 安装包文件名.zip.sha256`；Linux 也可使用 `sha256sum -c`。`release-evidence.json` 记录安装包摘要、源码来源和实际验收范围。

## 安装

- **Emby**：将 ZIP 内的 `MedioraEmbyHelper.dll` 放到 Emby 实际程序数据目录下的 `plugins/` 根目录，然后重启。
- **Jellyfin**：将 ZIP 内整个 `Mediora Helper_X.Y.Z.0` 文件夹放到 Jellyfin 实际程序数据目录下的 `plugins/`，然后重启。

回到 Mediora 的“影音优化 → 设置”，重新检测助手，核对并保存处理范围。升级前保留旧安装包、插件配置和完整保护状态目录。两个安装包不能互换。

## 更新方式

两个助手各自维护版本。Mediora 更新而助手未变时继续使用已有安装包；发布新助手版本后，下载页会出现对应的新 Release，也支持助手独立发版。

本仓库保存公开下载产物与安装说明。源码和构建检查由 Mediora 项目维护。
