# What I installed

I installed Visual Studio Code and the WSL extension so I can open Linux folders from WSL in VS Code.
- WSL
- Ubuntu in WSL
- Visual Studio Code
- VS Code WSL extension

# Useful terminal commands

- `pwd` shows my current directory
- `ls` lists files and folders
- `cd` changes directories
- `mkdir` creates a folder
- `code .` opens the current folder in VS Code
- `touch` creates an empty file
- `cp` copies a file or folder
- `mv` moves or renames a file or folder
- `rm` deletes a file
- `rmdir` deletes an empty folder

# Common Git commands

I will fill this section in later when I start learning Git.

# Mistakes I made and how I fixed them

I will write down errors, confusion, and the fix so I can learn from them.
- I forgot that `mv` is used for both moving and renaming.
- I learned that `rmdir` only works on empty folders.
- I learned to use `pwd` and `ls` when I feel confused.
1. I forgot where I was in the terminal.
2. I mixed up copying and moving.
3. I tried to remove a folder before it was empty.
1. I used `pwd` to check my current directory and `ls` to inspect what was there.
2. I reminded myself that `cp` copies and `mv` moves or renames.
3. I deleted the files inside the folder first, then used `rmdir` for an empty folder.

# Terminal habits that save time

- I can use the Up Arrow key to reuse recent commands.
- I can use Tab to complete file and folder names and avoid typos.
- I should not retype long paths when my current directory already makes a shorter command possible.
- I can use `history` to review commands I ran earlier.
- Reusing and editing commands is usually faster than typing everything again.

 # 10 terminal commands I used

- `pwd` shows my current directory
- `ls` lists files and folders
- `ls -la` shows a detailed list including hidden files
- `cd` changes directories
- `mkdir` creates a folder
- `touch` creates an empty file
- `cp` copies a file or folder
- `mv` moves or renames a file or folder
- `rm` removes a file
- `rmdir` removes an empty folder

# Week 1 Reflection

## What still feels scary

- I still worry about deleting the wrong thing with `rm`.
- I still need to think carefully about paths.
- I sometimes feel slow when typing commands.

## What already feels easier

- Opening WSL feels more normal now.
- I understand that directories are folders.
- I can move around with `cd`, `..`, and `~`.
- I can create files and folders from the terminal.
- I understand better where my development files live in WSL.

# How I configured Git

I checked that Git was installed with `git --version`.

I set my global Git identity with:
- `git config --global user.name "Your Name"`
- `git config --global user.email "you@example.com"`

I checked my settings with:
- `git config --global --list`

Global config affects all repos on this machine.

# Git username vs GitHub login

The Git username in `git config` is the name stored in commits.

The GitHub login is the username I use to sign into GitHub.

They are related, but they are not the same thing.

# Learning Log

This repository contains my learning notes and setup progress.

I am learning WSL, Linux terminal basics, VS Code, and Git.

# Day 10 Notes

## What each Git command means

- `git init` creates a new Git repository in the current folder.
- `git status` shows what Git sees right now.
- `git add README.md` stages README.md for the next commit.
- `git commit -m "Add initial learning log README"` creates a commit with a message.
- `git log --oneline` shows a short version of commit history.

## What I learned

A repo is a project folder that Git tracks.

The staging area is where I prepare changes before committing them.

A commit is a saved checkpoint in the history of the repo.

I pushed this repository from my local WSL Git repo to GitHub.

# Day 11 Notes

- A local repo lives on my computer.
- A remote repo lives on GitHub.
- `git remote add origin <url>` connects my local repo to GitHub.
- `git push -u origin main` publishes my local main branch to GitHub and sets upstream tracking.
- After upstream is set, I can often use just `git push`.

# Clone and pull

clone = downloading a full repo with history

pull = getting new changes into an existing local repo

# What I learned about remotes

- A local repo lives on my machine.
- A remote repo lives on GitHub.
- `origin` is the default name for the remote a repo was cloned from.
- `git remote -v` shows which remote URLs a repo is connected to.

I practiced making small commits on Day 13.

- `git status` shows what changed and what is staged.

Small commits are easier to understand than huge commits.

## Commit habits

- Small commits are easier to understand.
- `git status` tells me what changed and what is staged.
- Good commit messages describe what changed.
- `git add .` stages current changes in the current directory.

## Day 16 Notes — First Merge

### What I changed on the branch
On the `add-command-notes` branch, I added a small README section with notes about Git commands.

### How merge worked
I switched back to `main` with `git switch main`, then ran `git merge add-command-notes`. Git brought the committed changes from my branch into `main`.

### What confused me
At first, I had to remember that `git merge branch-name` merges into the branch I am currently on, not the other way around.

## Day 18 Notes

### Uncommitted bad change
An uncommitted bad change is a change I made to a file in my working directory that I do not want and have not saved in a commit.

### How git restore helped
I used `git restore mistakes-demo.txt` to throw away the unwanted uncommitted edit and return the file to its last committed version.

## Day 19 Notes — Reverting a Bad Commit

### What revert means
`git revert` does not erase history.

### How it works
It makes a new commit that undoes the effect of an earlier commit.

### Why it feels safe
This is beginner-safe because the old commit is still visible in history, so I can clearly see what happened.

## Day 21 — Week 3 Review

### How to create and merge a branch
1. Create and switch to a branch with `git switch -c review-branch`
2. Edit a file
3. Stage it with `git add`
4. Commit it with `git commit -m "message"`
5. Switch back to main with `git switch main`
6. Merge with `git merge review-branch`

### How to undo a bad change
- If the bad change is not committed yet, use `git restore <file>`
- If the bad change is already committed, use `git revert <commit-id>`

### Git mistakes I made this week
- Forgetting to check which branch I was on
- Mixing up `restore` and `revert`
- Forgetting that merge goes into the branch I am currently on
- Not checking `git status` before doing the next step

This repo was opened from the terminal as part of Day 22 practice. 

## Day 24 — Command-line help

I do not need to memorize every flag.

I need to know help exists and how to search notes.

Today I practiced using:
- `git --help`
- `git status --help`
- `ls --help`

My goal is not to remember everything. My goal is to know how to look things up when I need them.

# learning-log

## What I installed

- WSL2 with Ubuntu
- VS Code
- VS Code WSL extension
- Git
- GitHub account
- Python 3 in WSL (if available)

## WSL setup notes

- WSL lets me use Linux command-line tools on Windows.
- My projects live under `~/projects`.
- I usually start work by opening WSL and using `cd` to go to a repo.
- I use `code .` to open the current repo in VS Code.
- If I feel lost, I use `pwd` and `ls`.

## Useful terminal commands

- `pwd` — show current folder
- `ls` — list files in current folder
- `cd <folder>` — move into a folder
- `cd ..` — move up one folder
- `cd ~` — go to home folder
- `mkdir -p <folder>` — create folder and parent folders
- `touch <file>` — create an empty file
- `cat <file>` — print a file to terminal
- `code .` — open current folder in VS Code
- `bash <script.sh>` — run a shell script
- `python3 <file.py>` — run a Python file
- `clear` — clear terminal screen

## Common Git commands

- `git status` — show repo state
- `git add <file>` — stage a file
- `git commit -m "message"` — create a commit
- `git push` — send commits to GitHub
- `git pull` — bring changes from GitHub to local
- `git branch` — show branches
- `git switch <branch>` — switch branches
- `git switch -c <branch>` — create and switch to a new branch
- `git merge <branch>` — merge a branch into the current branch
- `git log --oneline` — show compact commit history
- `git diff` — show file changes
- `git restore <file>` — undo an uncommitted change
- `git revert <commit-id>` — undo a bad commit safely
- `git --help` — show Git help

## Repo workflow

1. Open WSL
2. Go to the repo with `cd`
3. Use `pwd` and `ls` if needed
4. Open repo with `code .`
5. Edit files
6. Run `git status`
7. Run `git add <file>`
8. Run `git commit -m "message"`
9. Run `git push`

## Branching workflow

1. Start on `main`
2. Run `git switch -c branch-name`
3. Edit files on the branch
4. Run `git status`
5. Run `git add <file>`
6. Run `git commit -m "message"`
7. Run `git switch main`
8. Run `git merge branch-name`
9. Run `git push`

Important: `git merge branch-name` merges that branch into the branch I am currently on.

## How to undo mistakes

### Bad uncommitted change
- Run `git status`
- Run `git diff`
- Run `git restore <file>` if I want to discard the change

### Bad committed change
- Run `git log --oneline`
- Find the bad commit ID
- Run `git revert <commit-id>`

### Reminder
- `restore` = uncommitted file change
- `revert` = committed change

## Mistakes I made and how I fixed them

1. I was in the wrong folder.
   - Fix: I checked `pwd` and used `cd` to go to the right repo.

2. I forgot to save a file before checking Git.
   - Fix: I saved the file and ran `git status` again.

3. I tried to merge while on the wrong branch.
   - Fix: I checked `git branch`, switched to `main`, then merged.

4. I mixed up `git restore` and `git revert`.
   - Fix: I remembered that `restore` is for uncommitted changes and `revert` is for committed ones.

5. I treated forgetting as failure.
   - Fix: I used `--help` and searched my notes instead of panicking.

## Things that still confuse me

- I still want more practice with Git history
- I still want more confidence reading help pages
- I still want more repetition with branching
- I still want more confidence running scripts
- I still sometimes forget which branch I am on

## Things I can do now that I could not do in Week 1

- Open WSL and navigate to repos from terminal
- Use `pwd`, `ls`, and `cd`
- Open a repo with `code .`
- Create repos and push them to GitHub
- Make commits
- Create and merge branches
- Undo uncommitted mistakes
- Undo committed mistakes
- Pull changes from GitHub
- Run simple scripts from WSL
