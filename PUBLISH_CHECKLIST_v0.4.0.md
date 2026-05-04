# v0.4.0 GitHub 发布前检查清单

## 需要上传到 GitHub Release 的文件

- `cyber-doggo-android-v0.4.0.apk`
- `cyber-doggo-windows-v0.4.0.exe`

如果实际文件名不同，请同步修改：

- `index.html` 下载链接
- `latest.json` 中的 `androidUrl` / `windowsUrl`
- `RELEASE_NOTES_v0.4.0.md` 下载文件名

## 需要提交到 GitHub Pages 仓库的文件

- `index.html`
- `CHANGELOG.md`
- `latest.json`
- `notice-0.4.0.html`
- `RELEASE_NOTES_v0.4.0.md`
- `README.md`
- `changelog.html`
- `CyberDoggo-logo.png`

## 当前页面状态

- 首页已从 v0.3.5 下载页切换为 v0.4.0 下载页。
- 旧的 0.4.0 开发公告页已改为 0.4.0 发布说明页，避免旧版本弹窗链接失效。
- `latest.json` 已从 v0.3.6 公告推送切换为 v0.4.0 正式更新提醒。
- `CHANGELOG.md` 已在顶部加入 v0.4.0 更新记录。
- `README.md` 已改为 v0.4.0 当前版本说明。

## 发布顺序建议

1. 先在 GitHub Releases 创建 `v0.4.0`。
2. 上传 Android APK 和 Windows EXE，文件名尽量使用上面的标准命名。
3. 再提交本页面包里的 GitHub Pages 文件。
4. 等 GitHub Pages 更新后，在浏览器打开下载页确认两个下载按钮都能访问。
5. 用旧版游戏启动一次，确认新版本提醒显示 v0.4.0，而不是 v0.3.6 开发公告。
