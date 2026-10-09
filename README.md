# Illustrator 助手 · 安装包与更新

Illustrator 2026 助手的公开下载与更新仓库。源码开发仓库保持私密；这里发布安装包、安装说明和校验信息。扩展包包含运行所需的客户端代码，可被提取，不构成源码保密措施。

## 当前版本：v0.1.0-dev.20261009.1

[下载已签名 ZXP 扩展包](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261009.1/IllustratorAssistant-0.1.0-dev.zxp) · [版本说明](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/tag/v0.1.0-dev.20261009.1) · [SHA-256](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261009.1/SHA256SUMS.txt) · [安装说明](INSTALL.md)

**开发预览版，适用 Windows / Illustrator 2026（30.x）。** 当前下载为 CEP ZXP 包，需要兼容的 ZXP 安装工具；具体步骤见安装说明。GitHub 自动生成的 Source code 压缩包只包含本仓库的说明文件。

本次修复扩展菜单出现两个助手入口的问题，只保留“Illustrator 设计助手”；放大预览仍从面板预览右上角图标打开。静态检查及 18 项预览相关测试通过。保留此前版本的画板单位同步、实际尺寸保存与导入、可交互预览。功能基线此前通过 264 项代码测试及 19 项原生尺寸验收与安装后复测。原生放大窗口显示、中键操作及真实模型服务仍需实际使用确认。

包内不含作者的 API 密钥、用户配置或画稿。API 功能需要自行配置服务商地址、密钥及可用模型。密钥只保留在面板内存。

后续版本在本仓库 [Releases](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases) 发布。
