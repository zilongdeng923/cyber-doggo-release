# Cyber Doggo v0.4.0

## English

Cyber Doggo v0.4.0 is a major test release and the first complete “three-module convergence” build. The story system, memory system, and personality system now work together more closely: adventures and daily care create lived experiences, memories compress and preserve those experiences, and personality slowly absorbs long-term traces before influencing future stories.

This version is a large structural update. Please back up your save before installing, especially if you are updating from v0.3.x.

### Downloads

- Android: `cyber-doggo-android-v0.4.0.apk`
- Windows: `cyber-doggo-windows-v0.4.0.exe`

Install the new version directly over the old one to keep your local save. Do not uninstall first unless you have already backed up your save.

### Main changes

- Integrated the story, memory, and personality systems into a more coherent long-term life loop.
- Added a stronger Memory Foundation structure: daily journals, weekly summaries, memoirs, memory anchors, semantic anchors, and cold archives.
- Established the 24-dimensional background personality model as the current personality foundation.
- Added article-based personality assimilation for diaries, weekly memories, and memoirs, with routine daily journals skipping personality analysis to avoid over-interpreting simple care days.
- Improved adventure settlement, story-thread closure, item return handling, and item description repair.
- Improved Android/Desktop feature parity for the 0.4.0 game logic while keeping platform-specific bridges separate.
- Fixed Android save sharing, Android NativeApi gaps, version display issues, signing/build cleanup, and release packaging problems.
- Added a clearer day-transition loading overlay to prevent accidental interaction while diaries and memories are being organized.
- Increased AI token budget for article personality settlement to reduce truncated JSON responses.

### Notes

This is still a friend-facing test build, but it is the first version that fully expresses the game’s intended electronic-life loop: stories become memories, memories shape personality, and personality changes future experiences.

---

## 中文

Cyber Doggo v0.4.0 是一次大型测试版更新，也是第一个完整意义上的“三模块合龙”版本。故事、记忆与人格系统现在会更紧密地互相咬合：冒险和日常照料产生经历，记忆系统压缩并保存经历，人格系统吸收长期痕迹，再反过来影响之后的故事。

这是一次底层结构更新。如果你从 v0.3.x 更新，建议先在游戏内导出或分享备份存档，再覆盖安装新版。

### 下载

- Android：`cyber-doggo-android-v0.4.0.apk`
- Windows：`cyber-doggo-windows-v0.4.0.exe`

如果已经安装旧版，建议直接覆盖安装，不要先卸载。除非你已经提前备份存档，否则卸载可能会导致本地存档丢失。

### 主要更新

- 整合故事、记忆、人格三大系统，让它们形成更完整的长期生命循环。
- 新增并整理更完整的 Memory Foundation 结构：日记、周记、回忆、记忆锚点、语义锚点与冷档案。
- 24 维后台人格坐标正式成为当前版本的人格基座。
- 日记、周记与回忆现在可以进行文章人格余韵结算；普通照料日记会跳过人格结算，避免把简单日常过度解释成人格变化。
- 优化冒险结算、故事线收束、物品带回与物品描述修复。
- Android 端同步桌面冻结版核心逻辑，同时保留 Android 系统分享面板与手机端桥接差异。
- 修复 Android 存档分享、NativeApi 接口缺失、版本号显示、签名构建与发布打包等问题。
- 进入下一天时加入更清晰的加载遮罩，避免整理日记或记忆时误操作。
- 提高文章人格结算的 AI 输出预算，降低长文章结算时 JSON 被截断的概率。

### 说明

这仍然是面向朋友测试的版本，但它已经第一次完整呈现了这个游戏的核心电子生命循环：故事成为记忆，记忆塑造人格，人格改变之后的经历。
