# Cyber Doggo v0.3.0 Release Notes

## Release tag

```text
v0.3.0
```

## Suggested release title

```text
Cyber Doggo v0.3.0 — Personality, Memory Trace and Daily Life
```

## Assets to upload

```text
cyber-doggo-android-v0.3.0.apk
cyber-doggo-windows-v0.3.0.exe
```

The download page points to these two asset names under the `v0.3.0` GitHub Release.

## Release body

### Main changes
- Added the 24-dimensional personality system, with base, growth, temporary and effective personality layers.
- Added cleanliness as a daily status, including adventure cleanliness cost and bath recovery.
- Added careTrace, so repeated care, absence and return can slowly shape personality.
- Upgraded weekly journals into prose-like weekly memories with hidden memoryTrace compression.
- Added recentMotifTrace to help the AI distinguish active threads, resolved stories, recurring motifs and motifs to avoid as defaults.
- Changed adventure settlement language from rewards to effects / changes, allowing status and relationship values to move up or down naturally.
- Improved text completeness checks, adventure summary cleanup and item synchronization between story text and inventory fields.
- Added a test-only 24-dimensional personality view at the bottom of Settings.

### Test quota note
- 经过内部测试人员组同意，将测试版的 API 额度下调至 1 元。
- Legacy quota pools are migrated once to the v0.3.0 test quota rule and marked with a quota pool version, so future launches will not repeatedly compress the quota.

### Install note
Install directly over the previous test version to keep the local save. Do not uninstall unless the save has already been backed up.
