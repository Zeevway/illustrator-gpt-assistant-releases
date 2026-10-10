# Illustrator 助手：开发预览版安装说明

适用 Windows、Adobe Illustrator 2026（30.x）。下载包为 IllustratorAssistant-0.1.0-dev.zxp，发布标签 v0.1.0-dev.20261010，包内版本 0.1.0。它是已签名的 CEP ZXP 扩展包，需要支持 CEP 的 ZXP 安装工具；不是 EXE 安装程序。

## 安装与更新

1. 保存文档并完全退出 Illustrator，更新前备份现有插件目录。
2. 下载本次 Release 的 IllustratorAssistant-0.1.0-dev.zxp 与 SHA256SUMS.txt。GitHub 自动生成的 Source code 压缩包仅包含发布仓说明，不是插件。
3. 使用支持 CEP 的 ZXP 安装工具安装，保留完整签名文件。不同工具的操作以其说明为准，本项目未逐一验收第三方安装器。
4. 用户安装目录为 %APPDATA%\Adobe\CEP\extensions\com.local.illustrator.designassistant。该目录直接包含 CSXS\manifest.xml、index.html 与 META-INF\signatures.xml，避免额外嵌套文件夹。
5. 重启 Illustrator。面板可自动显示，也可从“窗口 → 扩展功能 → Illustrator 设计助手”打开。放大预览仍从面板预览右上角图标打开。
6. 在“连接”填写自己的服务地址与 API 密钥，测试连接后选择模型。密钥只保留在当前面板内存，重开面板需重新填写。

本次改善 Windows 上创作与改稿输入框的中文输入兼容性，保留可选“输入窗口”入口。当前机器使用微信输入法的直接输入及安装后冷启动已确认；这不代表所有输入法、系统与停靠布局均已覆盖。若其他环境仍无法输入，可使用输入窗口并反馈环境。

签名有效时无需修改 PlayerDebugMode 或 Windows 证书信任设置。签名失败应停止安装，重新下载核对；不要绕过签名。开发用自签证书不代表商业发布者认证，本包无时间戳，证书约于 2027-10-10 到期，应在此前更新签名，准确期限以证书为准。

## 文件核对

文件大小：77585 字节。

SHA-256：70add37e3ad6569863b3fb2a033364493d223c7bf7c51acbff80316669fc5b05

## 验证与范围

本轮 301 项代码测试、静态检查及 10 项真实浏览器键盘/鼠标交互检查通过，签名包和 17 个已安装插件文件核对一致。真实浏览器检查不等于原生输入法测试；微信输入法另由用户在本机确认。微软拼音及其他输入法尚未完成本候选的兼容验证。

保留 AI 矢量与图片生成、受限自然语言改稿、画板单位与尺寸、预览缩放/中键拖动/放大窗口。原生放大窗口、中键操作、保存对话框与真实模型服务仍需实际使用验收，版本继续标记为开发预览版，建议先用测试文档。

安装包不含作者 API 密钥、用户配置或设计稿。模型能力、接口和费用由用户选择的服务商决定。客户端运行代码可从 ZXP 提取，独立发布仓不构成源码保密措施。

安装参考：[Adobe CEP 打包与安装指南](https://github.com/Adobe-CEP/Getting-Started-guides/blob/master/Package%20Distribute%20Install/readme.md)。
