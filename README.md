# Illustrator 助手 · 安装包与更新

Illustrator 2026 助手的公开下载仓库，源码开发仓保持私密。本仓仅发布安装包、安装说明和校验信息。ZXP 内的客户端代码可提取，不构成源码保密措施。

## 当前版本：v0.1.0-dev.20261010.3

[下载已签名 ZXP](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.3/IllustratorAssistant-0.1.0-dev.zxp) · [版本说明](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/tag/v0.1.0-dev.20261010.3) · [SHA-256](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases/download/v0.1.0-dev.20261010.3/SHA256SUMS.txt) · [安装说明](INSTALL.md)

**Windows / Illustrator 2026（30.x）开发预览版。** 当前为 CEP ZXP 包，需要兼容的安装工具；GitHub Source code 压缩包仅包含发布说明。

Windows 面板点击“保存配置”后，密钥使用当前 Windows 用户 DPAPI 加密，单独保存在插件安装目录之外；更新插件不会覆盖记录。重开面板时仅恢复匹配服务地址的密钥。新增“清除密钥”入口，清空密钥后保存也会删除旧记录。浏览器演示只保存地址和模型，不保存密钥。

本次 347 项代码测试与静态检查通过，18 个插件源文件与签名清单逐项一致，无调试入口。使用合成密钥在独立 Node 进程间完成 Windows 当前用户 DPAPI 的加密保存、恢复、地址隔离、替换和删除检查，未读取真实密钥或调用模型接口。本机签名候选已安装，18 个部署资源与签名清单一致。 该测试不等于 Illustrator 原生面板重启验收，重启后自动恢复仍待用户确认。

保留 API 路径修复、中文输入兼容模块、可选输入窗口、画板单位和尺寸、预览缩放及无文档导入。详细验收边界见版本说明。

API 功能需要自行配置服务地址、密钥及可用模型。连接测试只验证模型列表。包内不含作者的密钥、用户凭据记录、用户配置或画稿。

后续版本在 [Releases](https://github.com/Zeevway/illustrator-gpt-assistant-releases/releases) 发布。
