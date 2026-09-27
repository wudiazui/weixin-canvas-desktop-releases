# 微鑫画布 · Windows 桌面版

本仓库只提供桌面安装包、更新签名、校验文件、更新清单和使用说明。

## 下载 v0.7.15

适用 Windows 10/11 x64，选择与现有安装相同的一种方式：

- [EXE：安装到当前用户](https://github.com/wudiazui/weixin-canvas-desktop-releases/releases/download/desktop-v0.7.15/WeixinCanvas-0.7.15-windows-x64-setup.exe)
- [MSI：安装到系统，需要管理员权限](https://github.com/wudiazui/weixin-canvas-desktop-releases/releases/download/desktop-v0.7.15/WeixinCanvas-0.7.15-windows-x64.msi)
- [完整版本与附件](https://github.com/wudiazui/weixin-canvas-desktop-releases/releases/tag/desktop-v0.7.15) · [SHA-256 校验值](https://github.com/wudiazui/weixin-canvas-desktop-releases/releases/download/desktop-v0.7.15/SHA256SUMS.txt) · [安装与升级说明](https://github.com/wudiazui/weixin-canvas-desktop-releases/releases/download/desktop-v0.7.15/UPGRADE.md)

## 本次更新

- 启动自动检查更新，可在本机设置手动检查；确认后下载，保存完成且没有活动任务时重启安装。
- 桌面首页、画布库和设置采用轻多巴胺浅深主题，支持窄屏、键盘操作和减少动态效果。
- 画布内新增“全部／本画布”角色库，可管理参考图与描述、放入画布或用作生成参考。已插入的内容保留独立快照。

## 升级和数据

v0.7.14 首次升级需彻底退出应用，再用相同类型的 v0.7.15 安装包覆盖安装；之后可使用应用内更新。

本机画布、角色、素材和加密凭据位于 `%LOCALAPPDATA%\WeixinCanvas\data\extensions\desktop`。备份前退出应用，并复制整个目录。更换 Windows 账号或系统后需要重新填写 Key。

安装包提供 Tauri 更新签名及 SHA-256 校验，未配置 Windows Authenticode 代码签名。实际验收范围以版本附件中的 `build-manifest.json` 和 `installer-acceptance.json` 为准；Windows 10/11 干净用户、系统 DPI 设置、无 WebView2 的离线安装和真实供应商调用仍需对应环境验证。
