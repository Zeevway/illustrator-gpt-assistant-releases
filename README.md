# Illustrator 助手 · 安装包与更新

Illustrator 2026 助手的公开下载仓库，开发源码仓保持私密。本仓仅发布安装包、安装说明和校验信息；ZXP 客户端代码可提取，不构成源码保密措施。

## 当前版本：v0.1.0-dev.20261010.9

[下载已签名 ZXP](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.9/IllustratorAssistant-0.1.0-dev.zxp) · [版本说明](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/tag/v0.1.0-dev.20261010.9) · [SHA-256](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.9/SHA256SUMS.txt) · [安装说明](INSTALL.md)

**Windows / Illustrator 2026（30.x）开发预览版。** 需要支持 CEP 的 ZXP 安装工具；GitHub Source code 压缩包仅包含发布说明。

修复 AI 矢量重绘结果在导入预览时被 Illustrator 的 SVG Tiny 兼容提示阻塞的问题。仅在导入已校验的重绘 SVG 期间临时关闭交互提示，导入完成或失败都会恢复原交互状态；保留原生剪裁结构和可编辑矢量路径。

本轮 480 项代码测试及静态检查通过，18 个插件源文件与签名清单逐项一致。本机安装的 18 个插件资源已与本轮签名清单核对一致。本轮 7 项 Illustrator 原生宿主检查通过；使用本地测试 SVG，验证剪裁结果在预览、应用到图层及保存 AI 后重新打开时保留，并核对透明区域和着色区域的像素。这不代表真实 AI 服务商或完整 CEP 面板交互验收。 浏览器证据沿用 v0.1.0-dev.20261010.8 的 5 项模拟响应检查，仅覆盖哈希未变的面板和 API；本轮没有重跑浏览器检查，该证据不验证新的宿主改动。真实服务商生成质量和用户完整操作流程仍待复测。

API 功能需自行配置服务地址、密钥和可用模型。连接测试仅验证模型列表。包内不含作者密钥、用户凭据记录、用户配置或画稿。后续版本在 [Releases](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases) 发布。
