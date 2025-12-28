# Trick Questions and Common Exam Traps

Common trick questions and ambiguity traps designed to test deep understanding rather than surface knowledge.

---

## Git vs GitHub Confusion

### Question Type: "What is the difference between Git and GitHub?"

**Trap**: Questions may ask about Git features but show GitHub UI, or vice versa.

**Key Points**:
- Git runs locally, GitHub is cloud-based
- Git commands work in terminal, GitHub has web interface
- Git tracks changes, GitHub provides collaboration features

---

## Fork vs Clone Ambiguity

### Question Type: "When should you fork vs clone?"

**Trap**: Questions may present scenarios where either could work, but one is more appropriate.

**Key Points**:
- **Fork**: When you want to contribute to someone else's project (creates copy in your GitHub account)
- **Clone**: When you want to work locally on a repository (creates local copy on your machine)
- **Fork + Clone**: Common workflow - fork first (to get your own copy), then clone (to work locally)

---

## Branch vs Fork Confusion

### Question Type: "What is the difference between a branch and a fork?"

**Trap**: Both create separate versions, but serve different purposes.

**Key Points**:
- **Branch**: Within the same repository, for feature development
- **Fork**: Separate copy of the repository, for contributing to others' projects
- Branch is temporary (usually merged), fork is permanent (your own copy)

---

## Actions Workflow Triggers

### Question Type: "When does a workflow run?"

**Trap**: Questions may test understanding of event triggers vs manual triggers.

**Key Points**:
- `on: push` - Runs on every push to specified branches
- `on: pull_request` - Runs when PR is opened/updated
- `on: schedule` - Runs on a cron schedule
- `workflow_dispatch` - Allows manual triggering

---

## Secrets vs Variables

### Question Type: "When should you use secrets vs variables?"

**Trap**: Both store values, but have different security characteristics.

**Key Points**:
- **Secrets**: Encrypted, masked in logs, for sensitive data (API keys, passwords)
- **Variables**: Plain text, visible in logs, for non-sensitive configuration
- Secrets are never exposed in workflow logs, variables are visible

---

## Branch Protection Rules

### Question Type: "What happens when branch protection is enabled?"

**Trap**: Questions may test understanding of what protection rules actually prevent.

**Key Points**:
- Prevents direct pushes to protected branch
- Requires pull requests for changes
- May require reviews, status checks, or both
- Does NOT prevent creating branches or working locally

---

## Commit Immutability

### Question Type: "Can you change a commit after it's pushed?"

**Trap**: Questions may test understanding of commit history immutability.

**Key Points**:
- Commits are immutable (cannot be changed)
- You can create new commits that undo changes
- `git revert` creates a new commit that undoes changes
- `git reset` rewrites history (dangerous for shared branches)

---

## Pull Request Workflow

### Question Type: "What is the correct workflow for contributing?"

**Trap**: Questions may test understanding of the complete PR lifecycle.

**Key Points**:
1. Create issue (optional but recommended)
2. Create branch from main
3. Make changes and commit
4. Push branch and create PR
5. Request reviews
6. Address feedback
7. Merge PR
8. Close related issue

---

## GitHub Pages Deployment

### Question Type: "How do you deploy a static site with GitHub Pages?"

**Trap**: Questions may test understanding of Pages vs Actions for deployment.

**Key Points**:
- **Pages**: Simple static site hosting, automatic deployment from branch
- **Actions**: More control, can build and deploy complex sites
- Pages is easier for simple sites, Actions for complex builds

---

## License Types

### Question Type: "What license should you use?"

**Trap**: Questions may test understanding of license implications.

**Key Points**:
- **MIT**: Permissive, allows commercial use, requires attribution
- **Apache 2.0**: Similar to MIT, includes patent grant
- **GPL**: Copyleft, requires derivative works to be GPL
- **No License**: All rights reserved, others cannot use your code

---

## Common Mistakes to Avoid

1. **Confusing Git commands with GitHub features**
   - Git: `git commit`, `git push`
   - GitHub: Pull requests, issues, Actions

2. **Mixing up fork and clone**
   - Fork = GitHub account copy
   - Clone = Local machine copy

3. **Not understanding branch protection**
   - Protection prevents direct pushes, not branch creation

4. **Confusing secrets and variables**
   - Secrets = encrypted, sensitive
   - Variables = plain text, non-sensitive

5. **Misunderstanding commit immutability**
   - Commits cannot be changed, only new commits can undo

---

**Last Updated**: December 28, 2025

