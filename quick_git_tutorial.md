# Quick Git Tutorial

## 1. Check Git Version

```bash
git --version
```

## 2. Configure Git First Time

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@gmail.com"
```

## 3. Create or Clone Project

### Create New Git Repo

```bash
mkdir my-project
cd my-project
git init
```

### Clone Existing GitHub Repo

```bash
git clone repo-url
cd repo-name
```

## 4. Check File Status

```bash
git status
```

## 5. Add Files to Staging

Add all files:

```bash
git add .
```

Add one file:

```bash
git add filename.java
```

## 6. Commit Changes

```bash
git commit -m "Initial commit"
```

## 7. Connect Local Repo to GitHub

```bash
git remote add origin https://github.com/username/repo-name.git
```

Check remote:

```bash
git remote -v
```

## 8. Push Code to GitHub

For `main` branch:

```bash
git push -u origin main
```

For `master` branch:

```bash
git push -u origin master
```

## 9. Pull Latest Code

```bash
git pull origin main
```

## 10. Branch Commands

Create new branch:

```bash
git checkout -b feature/login
```

Switch branch:

```bash
git checkout main
```

List branches:

```bash
git branch
```

Push branch:

```bash
git push -u origin feature/login
```

## 11. Merge Branch

Go to target branch:

```bash
git checkout main
```

Pull latest code:

```bash
git pull origin main
```

Merge feature branch:

```bash
git merge feature/login
```

Push merged changes:

```bash
git push origin main
```

## 12. Common Daily Workflow

```bash
git pull origin main
git checkout -b feature/my-task

# Make your changes

git status
git add .
git commit -m "Added my task"
git push -u origin feature/my-task
```

Then create a Pull Request on GitHub.

## 13. Undo Commands

Undo unstaged changes:

```bash
git checkout -- filename
```

Unstage file:

```bash
git reset filename
```

Undo last commit but keep changes:

```bash
git reset --soft HEAD~1
```

## 14. Most Used Git Commands

```bash
git status
git add .
git commit -m "message"
git pull
git push
git branch
git checkout -b branch-name
git merge branch-name
```

## Simple Git Flow

```text
Working Directory
      ↓
git add
      ↓
Staging Area
      ↓
git commit
      ↓
Local Repository
      ↓
git push
      ↓
GitHub
```

## Quick Meaning

| Command | Meaning |
|---|---|
| `git status` | Shows changed files |
| `git add .` | Adds all changed files |
| `git commit -m "msg"` | Saves changes locally |
| `git push` | Uploads changes to GitHub |
| `git pull` | Gets latest changes from GitHub |
| `git branch` | Shows branches |
| `git checkout -b branch` | Creates and switches to new branch |
| `git merge branch` | Merges one branch into current branch |
