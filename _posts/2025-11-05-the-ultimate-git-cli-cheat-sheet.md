---
layout: post
title: "The Ultimate Git CLI Cheat Sheet: Master Version Control from Your Terminal"
date: 2025-11-05
categories: [development, git, cli, devtools]
author: "megatih"
description: "A comprehensive Git command-line reference for macOS, Linux, and Windows users. Learn configuration, branching, merging, and more with side-by-side examples."
tags: [git, devtools, productivity, cheatsheet]
---

# 🧭 The Ultimate Git CLI Cheat Sheet

Whether you're a solo developer or part of a large team, **Git** is the backbone of modern software collaboration. But remembering every command across platforms can be tricky. This guide compiles the most essential **Git CLI commands** — formatted for **macOS, Linux, and Windows** — so you can quickly configure, commit, branch, and merge like a pro.

---

## ⚙️ Configuration

|Command            |macOS|Linux|Windows|
|-------------------|------|------|------|
|Set username|`git config --global user.name "Your Name"`|`git config --global user.name "Your Name"`|`git config --global user.name "Your Name"`|
|Set email|`git config --global user.email "email@example.com"`|`git config --global user.email "email@example.com"`|`git config --global user.email "email@example.com"`|
|View config|`git config --list`|`git config --list`|`git config --list`|
|Set default editor|`git config --global core.editor "nano"`|`git config --global core.editor "nano"`|`git config --global core.editor "notepad"`|
|Enable color output|`git config --global color.ui auto`|`git config --global color.ui auto`|`git config --global color.ui auto`|

📝 **Tip:** Use `git config --global` for user-wide settings or omit `--global` to apply settings per project.

---

## 🪄 Creating & Cloning Repositories

Starting fresh or joining an existing project? Here’s how to get your repo ready.

|Command|macOS|Linux|Windows|
|-------|------|------|------|
|Initialize new repo|`git init`|`git init`|`git init`|
|Initialize bare repo|`git init --bare`|`git init --bare`|`git init --bare`|
|Clone remote repo|`git clone <url>`|`git clone <url>`|`git clone <url>`|
|Clone to folder|`git clone <url> <directory>`|`git clone <url> <directory>`|`git clone <url> <directory>`|
|Clone specific branch|`git clone -b <branch> <url>`|`git clone -b <branch> <url>`|`git clone -b <branch> <url>`|

💡 **Pro Tip:** Cloning a specific branch is handy when working in large repos with many active features.

---

## 📸 Basic Snapshotting

Committing is like saving checkpoints. These commands let you prepare and commit your work safely.

|Command|macOS|Linux|Windows|
|--------|------|------|------|
|Check status|`git status`|`git status`|`git status`|
|Stage files|`git add <file>`|`git add <file>`|`git add <file>`|
|Commit changes|`git commit -m "message"`|`git commit -m "message"`|`git commit -m "message"`|
|Amend last commit|`git commit --amend`|`git commit --amend`|`git commit --amend`|
|View differences|`git diff`|`git diff`|`git diff`|

---

## 🌿 Branching & Merging

Branches let you experiment safely without breaking your main codebase.

|Command|macOS|Linux|Windows|
|--------|------|------|------|
|List branches|`git branch`|`git branch`|`git branch`|
|Create branch|`git branch <name>`|`git branch <name>`|`git branch <name>`|
|Switch branch|`git switch <name>`|`git switch <name>`|`git switch <name>`|
|Merge branch|`git merge <branch>`|`git merge <branch>`|`git merge <branch>`|
|Abort merge|`git merge --abort`|`git merge --abort`|`git merge --abort`|

🚧 **Avoid merge hell:** Always pull the latest changes from your remote before merging.

---

## 🕰 Viewing History

Git keeps a complete timeline of your project. These commands help you navigate it.

|Command|macOS|Linux|Windows|
|--------|------|------|------|
|View log|`git log`|`git log`|`git log`|
|Compact log|`git log --oneline`|`git log --oneline`|`git log --oneline`|
|Graph view|`git log --graph --oneline`|`git log --graph --oneline`|`git log --graph --oneline`|

👀 **Visualize history:** Combine `--oneline` and `--graph` for clean, visual commit trees.

---

## 🔙 Undoing Changes

Made a mistake? No problem — Git lets you travel back in time.

|Command|macOS|Linux|Windows|
|--------|------|------|------|
|Discard file changes|`git restore <file>`|`git restore <file>`|`git restore <file>`|
|Undo last commit (keep changes)|`git reset --soft HEAD~1`|`git reset --soft HEAD~1`|`git reset --soft HEAD~1`|
|Undo last commit (discard changes)|`git reset --hard HEAD~1`|`git reset --hard HEAD~1`|`git reset --hard HEAD~1`|

⚠️ **Warning:** `--hard` permanently removes changes — use with caution.

---

## 🌐 Remote Repositories

Collaborate effectively by syncing with remote servers like GitHub or GitLab.

|Command|macOS|Linux|Windows|
|--------|------|------|------|
|Add remote|`git remote add origin <url>`|`git remote add origin <url>`|`git remote add origin <url>`|
|Push changes|`git push origin <branch>`|`git push origin <branch>`|`git push origin <branch>`|
|Pull updates|`git pull origin <branch>`|`git pull origin <branch>`|`git pull origin <branch>`|

🔗 **Set and forget:** Use `git push -u origin <branch>` to remember your upstream branch.

---

## 🧳 Stashing

Temporarily save your work without committing.

|Command|macOS|Linux|Windows|
|--------|------|------|------|
|Stash changes|`git stash`|`git stash`|`git stash`|
|List stashes|`git stash list`|`git stash list`|`git stash list`|
|Apply stash|`git stash apply`|`git stash apply`|`git stash apply`|
|Drop stash|`git stash drop stash@{n}`|`git stash drop stash@{n}`|`git stash drop stash@{n}`|

---

## 🏷 Tagging

Mark specific points in history — great for releases or milestones.

|Command|macOS|Linux|Windows|
|--------|------|------|------|
|List tags|`git tag`|`git tag`|`git tag`|
|Create annotated tag|`git tag -a v1.0 -m "Version 1.0"`|`git tag -a v1.0 -m "Version 1.0"`|`git tag -a v1.0 -m "Version 1.0"`|
|Push tag|`git push origin v1.0`|`git push origin v1.0`|`git push origin v1.0`|

---

## 🖥 Platform-Specific Differences

|Task|macOS|Linux|Windows|
|-----|------|------|------|
|Line endings|`git config --global core.autocrlf input`|`git config --global core.autocrlf input`|`git config --global core.autocrlf true`|
|Credential storage|`osxkeychain`|`cache`|`wincred`|

---

## ⚡ Useful Aliases

Speed up your workflow with handy shortcuts:

```bash
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.ci commit
git config --global alias.st status
git config --global alias.lg 'log --oneline --graph --decorate --all'


⸻

🔄 Common Workflows

Starting a New Project (Local)

cd /path/to/project
git init
git add .
git commit -m "Initial commit"

Working with Remote Repository

git clone <url>
cd <project>
git checkout -b feature-branch
git add .
git commit -m "Add new feature"
git push -u origin feature-branch


⸻

💡 Git Tips for Success
	•	Use git status often
	•	Commit frequently with meaningful messages
	•	Pull before you push
	•	Keep .gitignore tidy
	•	Never commit secrets or credentials

⸻

🚀 Wrapping Up

Mastering Git CLI isn’t about memorizing commands — it’s about understanding the flow of changes, commits, and collaboration. With this cheat sheet at hand, you’ll navigate repositories confidently and avoid common pitfalls that slow down your team.

⸻

If you found this guide helpful, share it with your teammates or bookmark it for later!

---