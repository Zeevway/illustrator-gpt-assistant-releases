# Illustrator 助手：开发预览版安装说明

适用环境：Windows、Adobe Illustrator 2026（30.x）。本次提供已签名的 CEP 扩展包 `IllustratorAssistant-0.1.0-dev.zxp`，包内版本为 0.1.0，发布标记为 v0.1.0-dev.20261009.1。它是 ZXP 扩展包，需要支持 CEP 的 ZXP 安装工具；不是双击即可执行的 EXE。

## 安装与更新

1. 保存文档并完全退出 Illustrator。更新前保留现有插件目录的备份。
2. 从本次 Release 的 Assets 下载 `IllustratorAssistant-0.1.0-dev.zxp` 和 `SHA256SUMS.txt`。GitHub 自动生成的“Source code”下载仅包含发布说明，不是插件安装包。
3. 使用支持 CEP 扩展的 ZXP 安装工具安装此 ZXP，并保留完整的签名文件。不同安装工具的操作入口以其说明为准。本项目已验证包签名和固定目录安装，但未逐个验收第三方安装器。
4. 本扩展的 Windows 用户安装目录是 `%APPDATA%\Adobe\CEP\extensions\com.local.illustrator.designassistant`。正确安装后，该目录直接包含 `CSXS\manifest.xml`、`index.html` 和 `META-INF\signatures.xml`，避免额外套一层文件夹。
5. 重新启动 Illustrator，从“窗口 → 扩展功能”打开“Illustrator 设计助手”。扩展菜单只保留这个入口；放大预览通过创作或改稿预览右上角图标打开。
6. 在“连接”中填写自己的服务地址和 API 密钥，测试连接后选择模型。密钥只保存在当前面板内存；重新打开面板需要重新填写。

签名有效时无需修改 PlayerDebugMode 或 Windows 证书信任设置。签名失败时停止安装，重新下载并核对文件，不绕过签名检查。签名是开发用自签证书，不代表经过商业发布者认证；当前包未加时间戳，预计需在 2027-10-09 前重新签名更新，准确有效期以证书为准。

## 文件核对

文件大小：73135 字节。

SHA-256：`01bd069b68d6987dff6d968dc395d671384bbca2ed4869606a91ba67b88805f1`。

## 本版本范围

- AI 生成 SVG 矢量或图片；自然语言进行六类受限改稿。
- 创作宽高及单位默认跟随当前活动画板；可手动选择单位。
- 创作与改稿预览支持滚轮缩放、中键拖动、适合窗口和独立放大窗口。
- 已移除包装工作区。

本次菜单修复通过静态检查及 18 项预览相关测试。功能基线此前通过 264 项代码测试、19 项 Illustrator 原生尺寸验收及安装后重启复测。放大窗口在 Illustrator 中的实际显示、中键操作、原生保存对话框和真实模型服务仍需实际使用验收，因此本版本标记为开发预览版。先用测试文档试用。

本发布不附带 API 密钥、用户配置或设计稿。模型能力、接口可用性和费用由用户选择的服务商决定。

安装方式参考：[Adobe CEP 打包与安装指南](https://github.com/Adobe-CEP/Getting-Started-guides/blob/master/Package%20Distribute%20Install/readme.md)。
