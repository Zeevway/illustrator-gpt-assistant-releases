# Illustrator 助手 · 安装包与更新

Illustrator 2026 助手的公开下载仓库，源码开发仓保持私密。本仓仅发布安装包、安装说明和校验信息。ZXP 内的客户端代码可提取，不构成源码保密措施。

## 当前版本：v0.1.0-dev.20261010.1

[下载已签名 ZXP](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.1/IllustratorAssistant-0.1.0-dev.zxp) · [版本说明](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/tag/v0.1.0-dev.20261010.1) · [SHA-256](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.1/SHA256SUMS.txt) · [安装说明](INSTALL.md)

**Windows / Illustrator 2026（30.x）开发预览版。** 当前为 CEP ZXP 包，需要兼容的安装工具；GitHub Source code 压缩包仅包含发布说明。

本次修复 API 地址仅填写域名时的生成路由：默认使用 /v1，保留显式自定义路径；网页响应给出安全提示。连接测试只验证模型列表，不证明生成可用。307 项代码测试与静态检查通过，本候选的原生操作与真实鉴权生成仍待用户验证。

保留上一版本中文输入兼容模块、可选输入窗口、画板单位和尺寸、预览缩放及放大窗口，具体验收边界见版本说明。

API 功能需要自行配置服务地址、密钥及可用模型。密钥只保留在面板内存。包内不含作者的密钥、用户配置或画稿。

后续版本在 [Releases](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases) 发布。
