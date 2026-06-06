# Cyber Doggo Changelog

## v0.5.0 — 2026-06-06

### Important notice
- v0.5.0 is a large test release that touches adventures, backpack flow, item settlement, personality, memory, and old-save compatibility. Please export or share a save backup before updating.
- Older saves may write missing weekly journals when first opened or continued. This is a compatibility process, not save corruption.
- Long stories, StoryThread behaviour, absence weekly wording, title variety, horror / Cthulhu / super-unfold stories, and full English support are still planned for later builds.

### Adventure system rewrite
- Adventures now use a separate full-screen flow, with a backpack confirmation step before going out.
- Final adventure titles are generated after the story resolves, reducing title/story mismatch.
- Return buttons, loading dots, and the old adventure floating bubble have been cleaned up.
- The ordinary adventure frame pool has been compressed into clearer event-driven cards, reducing weak pacing/ending cards in the main story pool.

### Backpack and carried items
- Backpack and item-cabinet layout have been reorganised for clearer ordinary item and memento management.
- Players can carry ordinary items, consumables, or mementos before an adventure, or choose to bring nothing.
- Carried items now act as Story Gravity: they can influence the day’s atmosphere, places, encounters, and story direction instead of merely being mentioned.
- Mementos lean toward mood and tendency, while ordinary items can become concrete interactions or story echoes.

### Item outcome and test-build confirmation
- New adventure items are no longer added immediately. At the end of the adventure, the game settles whether they were kept, returned, transferred, consumed, lost, only observed, or unchanged.
- Full-text item discovery can catch clearly kept items even if the story AI forgot to output structured itemSeeds.
- Fixed animal-shaped objects being blocked by old keyword-based living-creature guards, such as a woven little dog being treated as a real dog.
- Test-build confirmation dialogs appear for uncertain item ownership, suspected living/sentient entities, or high-risk changes to existing items.
- Fixed a history-binding bug where item outcomes could be written into the wrong adventure record when titles repeated; outcomes now bind more strictly by adventureId / day.

### Personality and memory loop
- Added short-term personality `temporary`, so adventures, care, and absence can briefly affect the dog’s current state.
- Temporary personality decays over time; long-term growth still settles slowly through diaries, weekly journals, and memoirs.
- All personality consumers now read `effective = base + growth + temporary`.
- Personality-settlement prompts were calibrated to reduce overusing dimensions such as poeticness merely because the text sounds lyrical.
- Weekly catchup has been improved; older saves may write some missing weekly journals when continued.

### Refactor and stability
- Large parts of the old runtime have been split and reorganised for future maintenance.
- Desktop and Android web assets and release metadata have been kept in sync.
- Added more automated checks for adventures, items, backpack flow, personality, memory, settlement, and release metadata.
- Normal adventure flow now avoids silently rewriting already-finalized past records.

### Known issues
- Long stories and StoryThreads are still experimental; ordinary adventures may still feel too daily or repetitive.
- Title variety and story continuity need further tuning.
- Weekly journals covering long absences may still contain imperfect wording such as implying the owner has already returned.
- Cloud saves, accounts, automatic multi-device sync, comments/feedback forms, full English in-game support, and horror / Cthulhu / super-unfold stories are not finished yet.

## v0.4.1 — 2026-05-05

### Diary and natural day-transition stability hotfix
- Fixed a natural day-transition issue where the diary prompt could disappear before the diary was actually visible.
- Diary, weekly journal, and memoir writing now follow a clearer two-stage flow: first the entry is written and shown, then memory and personality aftertaste continue to settle.
- During memory / personality aftertaste settlement, adventures, care actions, backpack interactions, and other state-changing operations stay locked to reduce save-state desynchronisation.

### Cleaner AI division of labour
- Diary, weekly journal, and memoir writers now focus on visible writing, memory traces, and source coverage.
- Personality aftertaste is handled by a separate Article Assimilation AI.
- Writer prompts were cleaned to avoid exposing visible-content generation to internal personality-settlement fields.
- The program strips any personality fields that a writing AI may accidentally include before saving, keeping the structure of “write the piece first, then let its aftertaste settle.”

### Personality-aftertaste settlement stability
- Article Assimilation output was made more compact, reducing the chance of long JSON replies being cut off before becoming valid JSON.
- If personality-aftertaste settlement temporarily fails, the diary / weekly journal / memoir that has already been written will still be kept and shown.
- The v0.4.0 story-memory-personality foundation remains unchanged.

### Update prompt
- The in-game “Go to downloads” button now opens the release page instead of directly opening an installer link.
- Please export or share a save backup before updating, then install this version directly over the old one.

## v0.4.0 — 2026-05-04

### Three-module foundation
- Story, memory, and personality now influence one another more tightly: stories create lived events, memory lets those events settle, and personality absorbs long-term traces that can shape later stories.
- This is a large foundation update. Players on older versions should export or share a save backup before updating.
- v0.4.0 is used as an important update reminder for older players, replacing the previous development notice.

### Memory system
- Added and reorganised memory layers including diaries, weekly journals, memoirs, memory anchors, semantic anchors, and cold archive.
- Older or lighter raw events now step back into the background once they are carried by a diary, weekly journal, or memoir, reducing repeated context and old-material pollution for the AI.
- Fixed the memoir / article personality-settlement pipeline so memoirs, weekly journals, and diaries can more reliably preserve their sources and compression traces.

### Personality system
- The 24-dimensional background personality coordinate system is now the foundation of the current personality model.
- Adventures, diaries, weekly journals, memoirs, and long-term daily traces can all leave slow, tiny, explainable influences on personality.
- Ordinary care diaries can still preserve a sense of everyday life, but they no longer force article-level personality settlement, avoiding over-reading routine daily notes.

### Story and backpack
- Improved adventure settlement, story closure, item carry-back, and item-description repair.
- Strengthened boundaries around cases such as living creatures being brought into the backpack, future events being written into past diaries, and item states falling out of sync.
- Old stories, old items, and old images are used as continuity references rather than a mechanical material bank to repeat.

### Android and Windows synchronisation
- Android has been synchronised with the desktop v0.4.0 frozen core logic, style, memory system, and personality system.
- Android keeps system share-sheet save export, while Windows keeps file export/import and desktop bridge logic.
- Fixed pre-release issues including a missing Android NativeApi item-description repair endpoint, signing/build configuration, version display, and Android save sharing.

### Experience and stability
- Added a clearer loading overlay when entering the next day, reducing accidental operations while diaries or memory are being organised.
- Increased the output budget for article personality settlement, reducing the chance of JSON truncation on long articles.
- Fixed cases where ordinary care diaries could trigger failed AI settlement. Ordinary diaries may still appear occasionally, but skip personality settlement.
- Kept the v0.3.5 Android save-sharing hotfix and still recommends backing up saves before updating.

## Older versions — Chinese archive

English summaries for older builds will be added gradually. For now, the full historical archive before v0.4.0 is available in Chinese in `CHANGELOG.md`.

### v0.3.6 notice push — 2026-05-04
- A temporary in-game announcement, not a new installer release.
- Warned older-version players that v0.4.0 was under development and advised them to avoid pushing daily adventures until the foundation update was released.

### v0.3.5 — 2026-04-30
- Android save-sharing hotfix.
- Fixed cases where exporting a save could fail to open the Android system share sheet and show `Desktop bridge unavailable` instead.

### v0.3.4 — 2026-04-30
- Memory Foundation cleanup build.
- Improved diaries, weekly journals, memoirs, memory anchors, and cold archive.
- Improved Android compatibility for the new memory-generation endpoints.

### v0.3.2 — 2026-04-29
- Added in-game update checking.
- Improved update prompts and download-page guidance.

### v0.3.1 — 2026-04-29
- Replaced system dialogs with in-game style bubble dialogs.
- Consolidated several backpack, memory, and daily-event stability fixes.

### v0.3.0 — 2026-04-29
- Added the 24-dimensional personality system.
- Weekly journals became more prose-like.
- Adventure outcomes, care, absence, and return could leave longer-term traces.

### v0.2.8 — 2026-04-28
- Added test quota support for AI usage.
- Improved quota warnings and test settings layout.

### v0.2.7 — 2026-04-27
- Added cross-device save transfer and mobile backup sharing.
- Reorganised save, memory test, and reset options into settings.

### v0.2.0 stable-test — 2026-04-26
- Improved AI adventure stability and continuity.
- Backpack and diary records became more complete.
