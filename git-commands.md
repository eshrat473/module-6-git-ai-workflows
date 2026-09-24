# Git Commands from Class Lectures

## 1. Configuration

| Command | Purpose |
|---------|---------|
| `git config --global user.name "Your Name"` | Set the username attached to commits |
| `git config --global user.email "your@email.com"` | Set the email attached to commits |
| `git config --list` | Show all current Git settings |

## 2. Starting a Repository

| Command | Purpose |
|---------|---------|
| `git init` | Create a new Git repository in the current folder |
| `git status` | Show changed, staged, and untracked files |

## 3. Staging and Committing

| Command | Purpose |
|---------|---------|
| `git add file.txt` | Stage one specific file |
| `git add .` | Stage all changed files |
| `git commit -m "Initial commit"` | Save staged changes with a message |
| `git commit -am "Updated project"` | Stage all tracked, modified files and commit in one step (does not include new files) |
| `git commit --amend` | Edit the last commit's message or add forgotten changes to it |
| `git log` | Show the full commit history |

## 4. Branching

| Command | Purpose |
|---------|---------|
| `git branch` | List all local branches |
| `git checkout new-feature` | Switch to an existing branch |
| `git checkout -b new-feature` | Create a new branch and switch to it |
| `git branch -D branch` | Force delete a local branch |
| `git push origin --delete branch` | Delete a branch from GitHub (remote) |

## 5. Stashing (Saving Work Temporarily)

| Command | Purpose |
|---------|---------|
| `git stash` | Save uncommitted changes and clean the working folder |
| `git stash list` | Show all saved stashes |
| `git stash show stash@{0}` | Show what changed in a specific stash |
| `git stash pop` | Restore the latest stash and remove it from the list |
| `git stash clear` | Delete all stashes |

## 6. Undoing Changes

| Command | Purpose |
|---------|---------|
| `git reset --hard 8822700` | Move back to a specific commit (by its ID) and discard everything after it |
| `git reset --hard HEAD~1` | Remove the last commit and its changes |

> **Warning:** `git reset --hard` and `git branch -D` permanently delete work. Use them carefully.

## Basic Workflow

1. `git status` to check changes
2. `git add .` to stage them
3. `git commit -m "Describe the change"` to save them
4. `git push` to upload to GitHub
