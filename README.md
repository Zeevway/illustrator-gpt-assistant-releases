# Illustrator 助手 · 安装包与更新

Illustrator 2026 助手的公开下载仓库，开发源码仓保持私密。本仓仅发布安装包、安装说明和校验信息；ZXP 客户端代码可提取，不构成源码保密措施。

## 当前版本：v0.1.0-dev.20261010.7

[下载已签名 ZXP](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.7/IllustratorAssistant-0.1.0-dev.zxp) · [版本说明](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/tag/v0.1.0-dev.20261010.7) · [SHA-256](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.7/SHA256SUMS.txt) · [安装说明](INSTALL.md)

**Windows / Illustrator 2026（30.x）开发预览版。** 需要支持 CEP 的 ZXP 安装工具；GitHub Source code 压缩包仅包含发布说明。

普通图片转矢量和矢量线稿统一使用 AI 重绘，原生图片描摹已禁用，旧描摹计划会明确拒绝，AI 请求失败不会回退描摹。重绘要求尽可能保留原图轮廓、比例、透视、构图和关键结构，不擅自改成图标；线稿去除光影并保留结构线。AI 重绘不保证与原图完全一致。另修复图片重绘来源快照的兼容问题，避免来源未改变时被误判为过期；实际来源变化仍须重新生成。

本轮 460 项代码测试及静态检查通过；隔离浏览器的 3 项检查使用模拟 AI 响应，并与本轮源文件哈希绑定。18 个插件源文件与签名清单逐项一致。本机安装的 18 个插件资源已与本轮签名清单核对一致。本轮 6 项 Illustrator 原生宿主检查通过，使用本地 PNG/SVG 测试素材；这不代表 CEP 面板交互或真实 AI 服务商已验收。 真实服务商生成质量、图片相似度及完整面板交互仍待用户验收。

API 功能需自行配置服务地址、密钥和可用模型。连接测试仅验证模型列表。包内不含作者密钥、用户凭据记录、用户配置或画稿。后续版本在 [Releases](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases) 发布。
