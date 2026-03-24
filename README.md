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
