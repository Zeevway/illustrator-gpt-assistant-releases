# Illustrator 助手 · 安装包与更新

Illustrator 2026 助手的公开下载仓库，开发源码仓保持私密。本仓仅发布安装包、安装说明和校验信息；ZXP 客户端代码可提取，不构成源码保密措施。

## 当前版本：v0.1.0-dev.20261010.6

[下载已签名 ZXP](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.6/IllustratorAssistant-0.1.0-dev.zxp) · [版本说明](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/tag/v0.1.0-dev.20261010.6) · [SHA-256](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.6/SHA256SUMS.txt) · [安装说明](INSTALL.md)

**Windows / Illustrator 2026（30.x）开发预览版。** 需要支持 CEP 的 ZXP 安装工具；GitHub Source code 压缩包仅包含发布说明。

修正放大预览首次加载时被隐藏的设置；首次打开尚未完成时，快速连点合并为一次窗口启动。窗口初始化期间有限重试连接，避免首次通知丢失后必须再次点击；过滤旧窗口的延迟消息。预览仍从“创作”或“改稿”的放大按钮打开，扩展功能菜单不增加第二个入口。

本轮 453 项代码测试及静态检查通过；隔离 Chrome 的 4 项预览窗口检查通过，使用独立页面和模拟 CEP 通信。18 个插件源文件与签名清单逐项一致。本机已安装本轮签名包，18 个部署资源与签名清单一致。 这些检查不能代替 Illustrator 原生窗口验收：首次单击、快速双击及关闭后重开是否正常、原生白屏是否消除，仍待实机确认。

API 功能需自行配置服务地址、密钥和可用模型。连接测试仅验证模型列表。包内不含作者密钥、用户凭据记录、用户配置或画稿。后续版本在 [Releases](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases) 发布。
