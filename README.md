# Illustrator 助手 · 安装包与更新

Illustrator 2026 助手的公开下载仓库，源码开发仓保持私密。本仓仅发布安装包、安装说明和校验信息。ZXP 内的客户端代码可提取，不构成源码保密措施。

## 当前版本：v0.1.0-dev.20261010.5

[下载已签名 ZXP](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.5/IllustratorAssistant-0.1.0-dev.zxp) · [版本说明](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/tag/v0.1.0-dev.20261010.5) · [SHA-256](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.5/SHA256SUMS.txt) · [安装说明](INSTALL.md)

**Windows / Illustrator 2026（30.x）开发预览版。** 当前为 CEP ZXP 包，需要兼容的安装工具；GitHub Source code 压缩包仅包含发布说明。

改稿新增 AI 矢量重绘：单独选中图片，输入“AI 重绘为扁平矢量”或“把当前图片转为矢量线稿图”。插件把真实图片与原始要求发送给支持视觉的矢量与改稿模型，校验 SVG 后制作预览；点击“导入”才应用到原图层，并保留原图备份。线稿默认黑色线条、透明背景；图像描摹和照片编辑继续保留。

本次 437 项代码测试与静态检查通过，18 个插件源文件与签名清单逐项一致，无调试入口。本机签名候选已安装，18 个部署资源与签名清单一致。 图片修改与转矢量的代码测试使用受控样本及宿主替身；真实服务商看图重绘、图片编辑响应及 Illustrator 原生矢量导入、描摹和原稿应用仍待实际验收，不能将这些代码测试视为实际软件或模型验收。

保留本机密钥加密保存、API 路径修复、中文输入兼容模块、可选输入窗口、画板单位和尺寸、预览缩放及无文档导入。详细验收边界见版本说明。

API 功能需要自行配置服务地址、密钥及可用模型。连接测试只验证模型列表。包内不含作者的密钥、用户凭据记录、用户配置或画稿。

后续版本在 [Releases](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases) 发布。
