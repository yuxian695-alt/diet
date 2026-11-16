# 饮食助手（免费版 · 装到手机桌面）

全部免费：不用服务器、不用 API、不用苹果开发者账号。数据只存在你的手机上。

## 文件
- `index.html`：App 本体
- `manifest.json`、`sw.js`：让它能“添加到主屏幕”，而且没网也能打开
- `icon-*.png`：桌面图标

## 第一步：免费放到网上（GitHub Pages，约 10 分钟）
1. 注册或登录 https://github.com
2. 右上角 **+ → New repository**，名字填 `diet`，选 **Public**，点 **Create repository**
3. 在新仓库页面点 **uploading an existing file**，把这个文件夹里的全部文件拖进去，点 **Commit changes**
4. 进入仓库的 **Settings → Pages**：Source 选 **Deploy from a branch**，Branch 选 **main**、文件夹选 **/(root)**，点 **Save**
5. 等 1–2 分钟，页面上会显示网址，类似 `https://你的用户名.github.io/diet/`

（也可以在电脑上用 Claude Code 打开这个文件夹，让它帮你创建仓库并开启 Pages。）

## 第二步：装到 iPhone 桌面
1. 用 **Safari** 打开上面的网址（必须是 Safari）
2. 点底部 **分享** 按钮 → **添加到主屏幕** → **添加**
3. 之后从桌面图标打开，全屏显示，就像普通 App

## 免费替代方案
- **截图分析 / 课表导入**：App 里点“复制提示词”，打开 Claude App（免费版就行），粘贴提示词并附上截图，发送后把回复整段复制回 App。
- **提醒**：在“今天”或“我的”里点 **加到日历**，选择“添加全部”。之后由 iPhone 日历按时提醒（吃饭、出门带饭、解冻、备餐）。每周导一次。
- **备份**：“我的 → 提醒与备份”，可以复制备份或下载备份文件。换手机、清理 Safari 前先备份一次。

## 以后要改功能
把改好的 `index.html` 重新上传到 GitHub 仓库（覆盖旧的）即可。如果手机上还是旧版本，从桌面打开后关掉再打开一次。改了 `sw.js` 里的 `CACHE` 名字，会强制所有缓存更新。
