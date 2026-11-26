# Fork features

Read this before merging upstream. Every item must still hold after the merge.

Branch: `main`. Base: `upstream/main` (arxhr007/Aliens_eye). Merge upstream in, never rebase. Last synced with upstream `932d751` (2.12.0).

## 1. No AGENTS.md

Upstream's `AGENTS.md` gives agents instructions for a Windows checkout (`.venv/Scripts/python.exe`) that contradict this fork's setup. Keep it deleted on every merge.

- Commits: this file's commit
- Files: `AGENTS.md` (deleted)
- Check: `git ls-files AGENTS.md` prints nothing. If upstream changed that file, the merge shows a modify/delete conflict; keep it deleted.

## Superseded

- `f3b0d9e` "fix: move to selectolax's lexbor backend" is now upstream as `8dd40ab`: `src/aliens_eye/core/analyzer.py` imports `LexborHTMLParser`, and `pyproject.toml` pins `selectolax>=0.3.21,<2`. Nothing to keep; take upstream's version.
