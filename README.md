# SillyTavern-IM-Bridge-UI

SillyTavern UI 扩展，作为 [SillyTavern-IM-Bridge](https://github.com/rinmashiro0529/SillyTavern-IM-Bridge) server plugin 的前端控制面板。

## 安装

1. 先按 server plugin 仓库 README 安装并启用 `st-im-bridge`。
2. 在 SillyTavern 网页中：Extensions → **Install Extension** → 粘贴：
   ```
   https://github.com/rinmashiro0529/SillyTavern-IM-Bridge-UI.git
   ```
3. 刷新 ST 网页 → 在「Extensions」抽屉中找到「IM Bridge」。

## 功能

- **个人 Bot** 管理：填写 Telegram Bot Token、允许列表、启停按钮、状态指示。
- **压缩配置**：调整 keepRecent / batchSize / timeoutMs / retryCount / retryDelayMs。
- **管理员视图**（admin 用户可见）：跨账号查看与启停。

## 探测

打开扩展面板时会先 `GET /api/plugins/st-im-bridge/probe`；若插件未安装则显示安装提示，不抛出错误。
