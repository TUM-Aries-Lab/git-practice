# Git Commands Basics

This guide covers the **essential Git commands** you need to know.  
Use it as a quick reference while learning version control.

---

## `git fetch`
Download changes from the remote repository (commits, branches, tags).  
Updates your local view of the remote (e.g., `origin/main`).  
Does **not** change your working files or current branch.  

👉 Think: *“Check what’s new online, but don’t touch my stuff yet.”*

---

## `git pull`
Does two things:  
1. `git fetch` – gets the latest changes  
2. `git merge` (or `rebase`) – applies them to your current branch  

👉 Think: *“Get the new stuff and put it into my branch now.”*

---

## `git add`
Stages changes (files you edited, added, or deleted) to be included in the next commit.  

👉 Think: *“Mark this file as ready to be saved.”*

Example:
```bash
git add myfile.py
```

---

## `git commit`
Saves a snapshot of the staged changes into the repository history.  

👉 Think: *“Take a photo of my project at this moment.”*

Example:
```bash
git commit -m "Add new feature"
```

---

## `git merge`
Combines another branch into your current branch.  
Creates a **merge commit** that shows both histories.  

👉 Think: *“Bring their work and mine together, keeping all history.”*

---

## `git rebase`
Moves (replays) your commits on top of another branch.  
Creates a **linear history** instead of a merge commit.  

👉 Think: *“Pretend I started my work from their latest code.”*

---

## `git stash`
Temporarily saves your uncommitted changes and cleans your working directory.  
Useful when you want to switch branches without committing.  

👉 Think: *“Put my messy desk into a drawer for now — I’ll come back to it later.”*

Examples:
```bash
git stash        # save changes
git stash pop    # reapply the stashed changes
```

---

## `git checkout`
Older command that can:
- Switch branches
- Restore files
- Move HEAD to another commit  

👉 Think: *“Go to this commit/branch/state.”*

Example:
```bash
git checkout main
```

---

## `git branch`
List, create, or delete branches.  

👉 Think: *“Show me my branches, or make a new one.”*

Examples:
```bash
git branch               # list
git branch feature-xyz   # create
git branch -d old-branch # delete
```

---

## `git switch`
Newer, simpler command (since Git 2.23) for switching branches.  
Safer and clearer than `git checkout`.  

👉 Think: *“Move to another branch cleanly.”*

Examples:
```bash
git switch main
git switch -c new-branch   # create and switch
```

---

## ✅ Quick Summary
- `fetch` = download updates  
- `pull` = download + apply updates  
- `add` = stage changes  
- `commit` = save snapshot  
- `merge` = combine branches (with merge commit)  
- `rebase` = replay commits for a clean history  
- `stash` = set aside uncommitted changes temporarily  
- `checkout` = switch branch/commit (old way)  
- `branch` = manage branches  
- `switch` = switch branches (new way, simpler)  

---

Completed Git Training
- Tony S.
- Huimin
- Nathalie
- Luka M.
