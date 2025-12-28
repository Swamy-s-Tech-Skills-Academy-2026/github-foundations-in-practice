# Git Essentials

**Session**: 01 - Introduction to Git and GitHub  
**Domain**: GitHub Fundamentals (20%)  
**Duration**: ~20 minutes

---

## Installing and Configuring Git

### Installation

* **Windows**: Download from [git-scm.com](https://git-scm.com/download/win)
* **macOS**: `brew install git` or download from git-scm.com
* **Linux**: `sudo apt-get install git` (Ubuntu/Debian) or use package manager

### Initial Configuration

```bash
# Set your name
git config --global user.name "Your Name"

# Set your email
git config --global user.email "your.email@example.com"

# Verify configuration
git config --list
```

---

## The Three States of Git

### 1. Working Directory

* Your files as you see them in your file system
* Modified files that haven't been staged
* Untracked files

### 2. Staging Area (Index)

* Files prepared for the next commit
* Intermediate area between working directory and repository
* Allows you to review changes before committing

### 3. Repository

* Committed snapshots stored permanently
* Complete history of your project
* Local `.git` directory contains all repository data

---

## Essential Git Commands

### Initializing a Repository

```bash
# Create a new repository
git init

# Initialize in existing directory
cd my-project
git init
```

### Checking Status

```bash
# See current status
git status

# Short status format
git status -s
```

### Staging Changes

```bash
# Stage a specific file
git add filename.txt

# Stage all changes
git add .

# Stage all files of a type
git add *.js
```

### Committing Changes

```bash
# Commit with message
git commit -m "Add new feature"

# Commit with detailed message
git commit -m "Add new feature" -m "This feature implements user authentication"

# Amend last commit
git commit --amend
```

### Viewing History

```bash
# View commit history
git log

# One-line format
git log --oneline

# Graph view
git log --graph --oneline --all

# Last N commits
git log -n 5
```

---

## Tracking Changes

### Understanding File States

* **Untracked**: File not in Git's index
* **Modified**: File changed but not staged
* **Staged**: File ready to be committed
* **Committed**: File saved in repository

### Viewing Differences

```bash
# See unstaged changes
git diff

# See staged changes
git diff --staged

# See changes in a file
git diff filename.txt
```

---

## Recovering from Mistakes

### Undoing Changes

```bash
# Discard changes in working directory
git checkout -- filename.txt

# Unstage a file (keep changes)
git reset HEAD filename.txt

# Discard all uncommitted changes
git reset --hard HEAD
```

### Reverting Commits

```bash
# Revert a commit (creates new commit)
git revert <commit-hash>

# Reset to previous commit (destructive)
git reset --hard <commit-hash>
```

### Viewing Previous Versions

```bash
# View file from previous commit
git checkout <commit-hash> -- filename.txt

# View previous version temporarily
git show <commit-hash>:filename.txt
```

---

## Common Workflows

### Daily Workflow

1. Check status: `git status`
2. Make changes to files
3. Stage changes: `git add .`
4. Commit: `git commit -m "Description"`
5. View history: `git log`

### Branching Workflow

```bash
# Create a new branch
git branch feature-name

# Switch to branch
git checkout feature-name

# Create and switch in one command
git checkout -b feature-name

# List branches
git branch

# Merge branch
git checkout main
git merge feature-name
```

---

## Best Practices

### Commit Messages

* Write clear, descriptive messages
* Use present tense: "Add feature" not "Added feature"
* Keep first line under 50 characters
* Add detailed description if needed

### Commit Frequency

* Commit often (small, logical changes)
* Don't commit broken code
* One logical change per commit

### .gitignore

Create a `.gitignore` file to exclude files:

```
# Compiled files
*.class
*.exe

# Dependencies
node_modules/
vendor/

# IDE files
.idea/
.vscode/

# OS files
.DS_Store
Thumbs.db
```

---

## Next Steps

* Learn about GitHub platform: `03_github-essentials.md`
* Practice GitHub Flow: `04_github-flow.md`
* Try hands-on lab: `src/labs/lab-01-create-repo.md`

---

**Related Content**:
* Notes: `src/notes/common-mistakes.md`
* Resources: `src/resources/cheat-sheets.md`

