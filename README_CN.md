# Nexent Releases

[English](README.md) | 简体中文

[Nexent](https://github.com/TTTABC-pri/nexent) 的 macOS 安装包与自动更新清单。本仓库只用于发布，没有源代码。

## 安装

需要 macOS 13 或更高版本（Apple Silicon 与 Intel 均可），并已安装 [Claude Code](https://docs.claude.com/en/docs/claude-code) 与 git。

1. 从 [最新 Release](https://github.com/TTTABC-pri/nexent-releases/releases/latest) 下载 `Nexent_<版本>_universal.dmg`。
2. 打开 dmg，把 Nexent 拖进"应用程序"。

### 第一次打开

Nexent 目前没有 Apple 开发者签名和公证，macOS 会拦截第一次打开。放行方法任选其一：

- **系统设置**：先打开一次 Nexent，macOS 提示无法验证开发者，关闭这个提示。然后打开"系统设置 → 隐私与安全性"，在"安全性"一栏找到 Nexent，点"仍要打开"，在弹窗中再点"仍要打开"并输入登录密码。
- **终端**：

  ```bash
  xattr -dr com.apple.quarantine /Applications/Nexent.app
  ```

只需放行一次。之后的版本通过应用内更新安装（设置 → 关于 → 检查更新）。
