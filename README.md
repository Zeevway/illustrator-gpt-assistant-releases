# Illustrator 助手 · 安装包与更新

Illustrator 2026 助手的公开下载仓库，开发源码仓保持私密。本仓仅发布安装包、安装说明和校验信息；ZXP 客户端代码可提取，不构成源码保密措施。

## 当前版本：v0.1.0-dev.20261010.8

[下载已签名 ZXP](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.8/IllustratorAssistant-0.1.0-dev.zxp) · [版本说明](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/tag/v0.1.0-dev.20261010.8) · [SHA-256](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.8/SHA256SUMS.txt) · [安装说明](INSTALL.md)

**Windows / Illustrator 2026（30.x）开发预览版。** 需要支持 CEP 的 ZXP 安装工具；GitHub Source code 压缩包仅包含发布说明。

AI 矢量重绘的默认等待上限调整为 10 分钟，普通请求仍为 2 分钟；执行过程中显示已等待时间和本次上限。错误提示区分插件等待到期与服务端返回超时，便于判断失败来源。保留取消操作，取消后不接收迟到结果；不会自动重试或回退到图片描摹。

本轮 477 项代码测试及静态检查通过；隔离浏览器的 5 项检查使用模拟 AI 响应，并与本轮源文件哈希绑定。18 个插件源文件与签名清单逐项一致。本机安装的 18 个插件资源已与本轮签名清单核对一致。保留 v0.1.0-dev.20261010.7 的 6 项 Illustrator 原生宿主历史检查：当前宿主文件哈希与当时一致，本轮未重新运行；这些历史检查仅使用本地 PNG/SVG 素材，不代表本轮 CEP 面板或真实 AI 服务商验收。 真实服务商请求成功率、生成质量及完整面板交互仍待用户复测，延长等待并不保证服务商能够返回结果。用户曾报告等待超过 5 分钟，与旧代码的 2 分钟设置不一致；本轮增加计时帮助复核，尚未复现并解释该时间差。

API 功能需自行配置服务地址、密钥和可用模型。连接测试仅验证模型列表。包内不含作者密钥、用户凭据记录、用户配置或画稿。后续版本在 [Releases](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases) 发布。
