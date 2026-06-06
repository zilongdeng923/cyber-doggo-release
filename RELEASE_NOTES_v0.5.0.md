# Cyber Doggo v0.5.0

Release date: 2026-06-06

This is a large test release. Please back up your save before updating.

## Download files

- Android: `cyber-doggo-android-v0.5.0.apk`
- Windows: `cyber-doggo-windows-v0.5.0.exe`

## Main changes

- Full-screen adventure flow with backpack confirmation before going out.
- Reorganised backpack and item cabinet layout.
- Carried items now influence story atmosphere and direction through the experimental Story Gravity layer.
- Adventure item outcomes are settled after the story: kept, returned, transferred, consumed, lost, only observed, or unchanged.
- Full-text item discovery can recover clearly kept items when structured `itemSeeds` are missing.
- Test-build confirmation dialogs appear for uncertain item ownership, suspected living/sentient entities, and high-risk item changes.
- Added short-term personality `temporary`, merged into `effective = base + growth + temporary` for all personality reads.
- Improved weekly catchup for older saves.
- Large internal refactor of adventure, item, memory, personality, settlement, and metadata systems.

## Known issues

- Long stories and StoryThreads are still experimental.
- Titles may repeat.
- Weekly journals covering long absences may still contain imperfect wording about the owner returning.
- Horror / Cthulhu / super-unfold stories, full English in-game support, cloud saves, accounts, and automatic multi-device sync are not finished yet.

---

# 赛博狗子 v0.5.0

发布日期：2026-06-06

这是一次大型测试版更新。更新前请先备份存档。

## 下载文件

- Android：`cyber-doggo-android-v0.5.0.apk`
- Windows：`cyber-doggo-windows-v0.5.0.exe`

## 主要更新

- 冒险改为独立全屏流程，出门前会先确认背包携带物品。
- 背包和物品柜结构重新整理。
- 携带物品会通过试验性的 Story Gravity 层影响故事氛围和方向。
- 冒险结束后统一结算物品：带回、放回、转交、消耗、遗失、只是看过或保持不变。
- 新增全文物品发现，避免故事文本明确带回物品但结构化 `itemSeeds` 缺失时漏结算。
- 新增测试版确认弹窗，用于处理不确定物品归属、疑似生物/有意识实体和高风险物品变化。
- 新增短期人格 `temporary`，所有人格读取统一使用 `effective = base + growth + temporary`。
- 改进旧存档周记补写。
- 大规模整理冒险、物品、记忆、人格、结算和发布元数据相关底层代码。

## 已知问题

- 长故事和 StoryThreads 仍在测试中。
- 标题可能重复。
- 长期缺席期间的周记文本可能仍有“主人回来了”一类不够准确的表述。
- 恐怖 / 克苏鲁 / 超展开故事、完整英文版、云存档、账号和自动多端同步仍未完成。
