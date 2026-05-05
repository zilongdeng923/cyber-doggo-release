# Cyber Doggo v0.4.1

## English

This is a stability hotfix for the v0.4.0 Memory Foundation release. It focuses on natural day transitions, diary/weekly/memoir writing, and the separation between visible writing and internal personality aftertaste settlement.

### Downloads

- Android: `cyber-doggo-android-v0.4.1.apk`
- Windows: `cyber-doggo-windows-v0.4.1.exe`

Install the new version directly over the old one to keep your local save. Do not uninstall first unless you have already backed up your save.

### Changes

- Fixed a natural day-transition issue where the diary prompt could disappear before the diary was actually visible.
- Improved the transition flow for diary, weekly journal, and memoir writing.
- Diary, weekly journal, and memoir generation now follow a clearer two-stage structure:
  - first, the visible entry is written and saved;
  - then, the game continues to settle memory and personality aftertaste in the background while state-changing actions stay locked.
- Cleaned up the division of labour between AIs:
  - diary / weekly / memoir writers focus on visible writing and memory traces;
  - Article Assimilation handles personality aftertaste separately.
- Reduced the risk of personality-settlement JSON being cut off by making the Article Assimilation output more compact.
- Cleaned writer prompts so visible-content generation is less exposed to internal personality-settlement concepts.
- Kept the v0.4.0 story-memory-personality foundation unchanged.

### Notes

This is a recommended update for all v0.4.0 testers, especially if you experienced diary delay, missing diary visibility, or failed personality-aftertaste settlement after a natural day transition.

The in-game update button now points to the release page instead of directly opening a platform-specific download file. This makes the update flow clearer and avoids blank or confusing download pages.

---

## 中文

这是赛博狗子 v0.4.0 Memory Foundation 版本后的稳定性热修复。本版主要修复自然跨天、日记 / 周记 / 回忆写入，以及可见文本生成与内部人格余韵结算之间的分工问题。

### 下载

- Android：`cyber-doggo-android-v0.4.1.apk`
- Windows：`cyber-doggo-windows-v0.4.1.exe`

如果已经安装旧版，建议直接覆盖安装，不要先卸载。除非你已经提前备份存档，否则卸载可能会导致本地存档丢失。

### 更新内容

- 修复自然进入第二天时，日记提示可能提前消失，但日记还没有真正显示的问题。
- 优化日记、周记和回忆的写入流程。
- 日记、周记和回忆现在采用更清晰的两段式结构：
  - 先写下并保存可见记录；
  - 再继续整理记忆与人格余韵，此阶段会继续锁住冒险、照料、背包互动等会改变状态的功能。
- 清理 AI 分工：
  - 日记 / 周记 / 回忆写作 AI 只负责可见文本和记忆痕迹；
  - Article Assimilation AI 单独负责人格余韵结算。
- 压缩文章人格结算输出，降低 JSON 被截断导致结算失败的概率。
- 清理写作 prompt，避免生成型 AI 被内部人格结算概念污染注意力。
- 保留 v0.4.0 的故事、记忆与人格三模块基础结构。

### 说明

如果你在 v0.4.0 中遇到自然跨天后日记延迟显示、日记提示提前消失、性格余韵结算失败等问题，建议更新到本版本。

游戏内更新提示中的“前往下载”现在会跳转到发布页，而不是直接打开某个平台的安装包链接。这样玩家可以先看到说明，再选择 Android 或 Windows 下载。
