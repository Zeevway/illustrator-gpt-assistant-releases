# Illustrator 助手 · 安装包与更新

Illustrator 2026 助手的公开下载仓库，源码开发仓保持私密。本仓仅发布安装包、安装说明和校验信息。ZXP 内的客户端代码可提取，不构成源码保密措施。

## 当前版本：v0.1.0-dev.20261010.2

[下载已签名 ZXP](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.2/IllustratorAssistant-0.1.0-dev.zxp) · [版本说明](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/tag/v0.1.0-dev.20261010.2) · [SHA-256](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.2/SHA256SUMS.txt) · [安装说明](INSTALL.md)

**Windows / Illustrator 2026（30.x）开发预览版。** 当前为 CEP ZXP 包，需要兼容的安装工具；GitHub Source code 压缩包仅包含发布说明。

本次修复放大预览的宿主事件兼容问题；没有打开文档时，创作结果可按设定尺寸及单位创建单画板文档并导入新图层。已有文档的尺寸、单位与原对象保留。

本次 324 项代码测试与静态检查通过，17 个插件源文件与签名清单逐项一致。两个独立真实浏览器页面的传输检查通过（CEP 事件回调为模拟）；覆盖预览接收与更新，不能替代 Illustrator 原生放大窗口验收。本候选的 Illustrator 原生导入验收尚待完成。 Illustrator 原生放大预览窗口仍待用户实际确认。

保留 API 路径修复、中文输入兼容模块、可选输入窗口、画板单位和尺寸、预览缩放与放大窗口。详细验收边界见版本说明。

API 功能需要自行配置服务地址、密钥及可用模型。密钥只保留在面板内存；连接测试只验证模型列表。包内不含作者的密钥、用户配置或画稿。

后续版本在 [Releases](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases) 发布。
