## git ready

Rebase current branch onto an integration branch (default: dev) and optionally push with force-with-lease.

### Install (macOS/Linux)
```bash
mv git-ready ~/.local/bin/git-ready
chmod +x ~/.local/bin/git-ready
```
Ensure `~/.local/bin` is in PATH.

### Install (Windows PowerShell)
Place `git-ready.ps1` in a directory on PATH (optionally add a `git-ready.cmd` shim invoking pwsh).

### Usage
```bash
git ready                     # update base, rebase, push
git ready --onto main         # use main
git ready --no-push           # skip push
git ready --autosquash        # interactive autosquash
git ready --stash             # stash/pop around rebase
git ready continue            # continue rebase then push
git ready abort               # abort rebase
```

### Options
```
--branch / --onto <name>   Base branch (default dev)
--remote <name>            Remote (default origin)
--no-fetch                 Skip fetch
--no-push                  Skip push
--yes                      Skip confirmation
--autosquash               Interactive autosquash
--stash                    Stash & pop
--allow-dirty              Allow dirty tree
--dry-run                  Show actions
```

### Uninstall
```bash
rm -f ~/.local/bin/git-ready
```
