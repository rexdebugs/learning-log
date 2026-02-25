# Phase 0 - Day 1 (Foundation install)

## What I did
- Ran Windows Update and rebooted until fully updated.
- Installed WSL2 and Ubuntu.
- Opened Ubuntu and created my Linux username.
- Ran: sudo apt update && sudo apt upgrade
- Created: ~/dev
- Confirmed I am working in: /home/rex

## Commands I ran
- sudo apt update && sudo apt upgrade
- mkdir -p ~/dev
- pwd
- ls -la ~

## Errors / weird stuff 
- none
 
## What I learned today
- WSL2 lets me use Linux on Windows.
- Ubuntu updates software via apt.
- My Linux home folder is /home/rex, and ~/dev is my dev workspace.

## Day 3 - Terminal survival skills

Favorite commands so far:
- pwd (where am I)
- ls -la (what's here, with details)
- cd .. / cd ~ / cd - (move around)
- mkdir -p (make nested folders)
- touch (make empty files)
- mv / cp (rename/move/copy)
- rm (delete files carefully)
- cat / less (read files)
- head / tail (peek at start/end)
- find . -name "*.txt" (find files)
- grep -R -n "TEXT" . (search inside files)
- | and tee (pipe output, save results)
