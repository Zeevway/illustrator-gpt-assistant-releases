# Illustrator 助手 · 安装包与更新

Illustrator 2026 助手的公开下载仓库，开发源码仓保持私密。本仓仅发布安装包、安装说明和校验信息；ZXP 客户端代码可提取，不构成源码保密措施。

## 当前版本：v0.1.0-dev.20261012.1

[下载已签名 ZXP](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261012.1/IllustratorAssistant-0.1.0-dev.zxp) · [版本说明](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/tag/v0.1.0-dev.20261012.1) · [SHA-256](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261012.1/SHA256SUMS.txt) · [安装说明](INSTALL.md)

**Windows / Illustrator 2026（30.x）开发预览版。** 需要支持 CEP 的 ZXP 安装工具；GitHub Source code 压缩包仅包含发布说明。

修复生成 SVG 在根元素或分组上设置字体时，被误报“属性不在允许列表 font-family”的兼容问题。支持这些位置继承既有的 8 项文字属性，并继续校验属性值；危险内容的拦截规则保持不变。

本轮 488 项代码测试及静态检查通过，18 个插件源文件与签名清单一致。本机安装的 18 个插件资源已与本轮签名清单核对一致。本轮 3 项隔离浏览器检查使用同类 SVG 和模拟响应。沿用 v0.1.0-dev.20261010.9 的 7 项宿主和 3 阶段剪裁像素历史检查，宿主文件未变，本轮未重跑。尚未取得本次报错的原始 SVG，验证使用同类示例。真实服务商结果、字体实际呈现及原图相似度仍待用户复测。

API 功能需自行配置服务地址、密钥和可用模型。连接测试仅验证模型列表。包内不含作者密钥、用户凭据记录、用户配置或画稿。后续版本在 [Releases](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases) 发布。
