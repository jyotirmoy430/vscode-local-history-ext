# Changelog

## 0.1.0 — 2026-10-30

Initial **preview** release — under active development, use at your own risk.

- **Local History window** (right-click a file → Local History): revision list + side-by-side/unified diff with word highlights, » chevrons to apply single changes, Revert, Label; opens in a floating window.

- Automatic, Git-free local history: save, external change, create, delete, rename (VS Code-initiated and external, linked by content).
- Local History view in the Explorer: file / folder / workspace scope, day grouping, event icons, line stats, inline labels, deleted files.
- Compare with current, with previous, or between any two revisions in the native diff editor; multi-file preview for folder and label restores.
- Restore whole files, deleted files, folders to a point in time, and labels (exact state). Safety snapshots before every write; restores bypass format-on-save.
- Labels (named checkpoints) for file, folder or workspace.
- SQLite metadata (`node:sqlite`, WASM fallback) + SHA-256 content-addressed, gzip-compressed snapshots outside the workspace. Atomic writes, quick_check on open, forward-only migrations, never deletes a corrupt database.
- Retention: change-day retention (5 days), optional per-file cap and size cap; pins and labels are protected.
- Default exclusions for noise and secrets; `.gitignore` opt-in; binary and large-file skipping. No network access.
