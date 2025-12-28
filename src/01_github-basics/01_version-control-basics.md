# Version Control Basics

**Session**: 01 - Introduction to Git and GitHub  
**Domain**: GitHub Fundamentals (20%)  
**Duration**: ~15 minutes

---

## Why Version Control Matters

Version control is the foundation of modern software development. It enables teams to:

* Track changes over time
* Collaborate without conflicts
* Revert to previous states
* Understand what changed and why
* Work on features in parallel

---

## The Evolution of Version Control

### Manual Backups (Pre-VCS)

* Copying files with timestamps
* No collaboration support
* High risk of losing work
* No way to track what changed

### Centralized Version Control (CVCS)

* Examples: CVS, Subversion (SVN)
* Single central server
* Requires network connection
* Single point of failure

### Distributed Version Control (DVCS)

* Examples: Git, Mercurial
* Every developer has a full copy
* Work offline
* No single point of failure
* Fast and efficient

---

## What is Git?

**Git** is a distributed version control system created by Linus Torvalds in 2005.

### Key Characteristics

* **Distributed**: Every clone is a full repository
* **Fast**: Most operations are local
* **Branching**: Easy to create and merge branches
* **Open Source**: Free and widely adopted

### Git vs GitHub

* **Git**: The version control tool (runs on your computer)
* **GitHub**: A hosting platform for Git repositories (cloud service)

---

## Real-World Scenarios

### Scenario 1: Feature Development

* Create a branch for a new feature
* Work on it independently
* Merge when ready
* No interference with main codebase

### Scenario 2: Bug Fixes

* Create a branch from the bug report
* Fix the issue
* Test the fix
* Merge back to main

### Scenario 3: Experimentation

* Try new approaches in branches
* Keep main branch stable
* Discard experiments easily
* Learn without risk

### Scenario 4: Collaboration

* Multiple developers work simultaneously
* Merge changes automatically
* Resolve conflicts when needed
* Maintain code history

---

## Key Concepts

### Repository (Repo)

A repository is a directory that contains your project files and the complete history of changes.

### Commit

A commit is a snapshot of your repository at a specific point in time. Each commit has:
* A unique identifier (hash)
* A message describing the change
* Author and timestamp
* Reference to previous commit(s)

### Branch

A branch is a parallel version of your code. It allows you to:
* Work on features independently
* Experiment safely
* Maintain multiple versions

### Merge

Merging combines changes from different branches into one.

---

## Benefits for Teams

* **Collaboration**: Multiple people can work on the same project
* **History**: Complete record of all changes
* **Accountability**: Know who changed what and when
* **Safety**: Easy to revert mistakes
* **Parallel Work**: Work on different features simultaneously

---

## Next Steps

* Learn Git commands in `02_git-essentials.md`
* Understand GitHub platform in `03_github-essentials.md`
* Practice GitHub Flow in `04_github-flow.md`

---

**Related Content**:
* Lab: `src/labs/lab-01-create-repo.md`
* Notes: `src/notes/common-mistakes.md`

