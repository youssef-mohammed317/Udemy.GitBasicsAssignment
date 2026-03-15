# Udemy.GitBasicsAssignment — Git Basics Assignment Practice Repo

This repository contains the **assignment work** I completed while following the Udemy course:
**“Git & GitHub – The Practical Guide”**.

It is intentionally simple because the goal of this repository is to practice the **basic Git workflow**:
creating a repository, making commits, working with branches, and merging feature work back into `main`.

---

## What I practiced here

- Creating an initial repository and first commit
- Adding multiple files and tracking changes
- Creating and switching to a `feature` branch
- Making changes in an isolated branch
- Merging the feature branch back into `main`
- Understanding a **fast-forward merge**
- Practicing a clean beginner-friendly Git workflow

---

## Repository structure

| Path | Purpose |
|------|---------|
| `instructions.txt` | Assignment instructions from the course |
| `file-1.txt` | First tracked file |
| `file-2.txt` | Second tracked file |
| `file-3.txt` | File added and updated in feature branch workflow |

---

## Key Git commands used (core set)

> Exact flags/options can vary, but these are the commands I used to perform the actions reflected in the reflog.

```bash
# init + first commit
git init
git status
git add .
git commit -m "first commit"

# branch workflow
git switch -c feature
git switch main

# feature work
git add .
git commit -m "create feature branch and add third file"
git commit -m "add Please add me to the master/main branch to the third file"

# merging
git merge feature

# history
git log --oneline --graph --decorate
git reflog
