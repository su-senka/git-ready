# Changelog

## [v1.0.0] - 2025-09-06

### Added
- Initial release of `git-ready`.
- Rebases current branch onto an integration branch (default: `dev`).
- Supports interactive and autosquash rebases.
- Optionally force-pushes with lease after rebase.
- Handles dirty working trees with `--stash` or `--allow-dirty`.
- Supports dry-run mode for safe preview.
- Provides `continue` and `abort` modes for rebase sequences.
- Colorful, user-friendly output and