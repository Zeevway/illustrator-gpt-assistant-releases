# Illustrator 助手 · 安装包与更新

Illustrator 2026 助手的公开下载仓库，开发源码仓保持私密。本仓仅发布安装包、安装说明和校验信息；ZXP 客户端代码可提取，不构成源码保密措施。

## 当前版本：v0.1.0-dev.20261010.10

[下载已签名 ZXP](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.10/IllustratorAssistant-0.1.0-dev.zxp) · [版本说明](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/tag/v0.1.0-dev.20261010.10) · [SHA-256](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.10/SHA256SUMS.txt) · [安装说明](INSTALL.md)

**Windows / Illustrator 2026（30.x）开发预览版。** 需要支持 CEP 的 ZXP 安装工具；GitHub Source code 压缩包仅包含发布说明。

提示词级实验候选：将创作插画的风格要求与图片重绘分开，默认要求忠实保留原图几何、五官比例和外观，避免擅自美化或卡通化，同时保留用户明确指定的风格与线稿要求。

本轮 483 项代码测试及静态检查通过，18 个插件源文件与签名清单一致。本机尚未确认安装本轮签名包。本轮 6 项隔离浏览器检查使用模拟响应，只验证请求行为。沿用 v0.1.0-dev.20261010.9 的 7 项宿主和 3 阶段剪裁像素历史检查，宿主文件未变，本轮未重跑；这些检查不能证明 AI 重绘外观有所改善。上一版的人像任务已完成生成，但结果存在明显风格化偏差。本轮外观改善尚未验证，需使用同一张原图进行前后 A/B 对比；提示词调整不保证与原图一致。

API 功能需自行配置服务地址、密钥和可用模型。连接测试仅验证模型列表。包内不含作者密钥、用户凭据记录、用户配置或画稿。后续版本在 [Releases](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases) 发布。
