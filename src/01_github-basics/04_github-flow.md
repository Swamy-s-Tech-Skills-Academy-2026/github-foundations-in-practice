# GitHub Flow

**Session**: 01 - Introduction to Git and GitHub  
**Domain**: GitHub Fundamentals (20%)  
**Duration**: ~10 minutes

---

## What is GitHub Flow?

**GitHub Flow** is a lightweight, branch-based workflow designed around deployments. It's simple, effective, and works well for teams of all sizes.

### Core Principles

* The `main` branch is always deployable
* Create branches for new work
* Use pull requests for collaboration
* Merge when ready
* Deploy immediately after merge

---

## The GitHub Flow Process

### 1. Create a Branch

```bash
# Create and switch to new branch
git checkout -b feature-name

# Or using newer Git syntax
git switch -c feature-name
```

**Branch Naming Conventions**:
* `feature/user-authentication`
* `fix/login-bug`
* `docs/update-readme`
* `refactor/code-cleanup`

### 2. Make Changes

* Edit files
* Add new files
* Delete files
* Test your changes

### 3. Commit Changes

```bash
# Stage changes
git add .

# Commit with message
git commit -m "Add user authentication feature"
```

### 4. Push to GitHub

```bash
# Push branch to remote
git push -u origin feature-name
```

### 5. Create Pull Request

* Go to repository on GitHub
* Click "Compare & pull request"
* Write description
* Request reviewers
* Link related issues
* Click "Create pull request"

### 6. Review and Discuss

* Team members review code
* Leave comments and suggestions
* Request changes if needed
* Approve when ready

### 7. Merge Pull Request

* Click "Merge pull request"
* Choose merge type:
  * **Create a merge commit**: Preserves full history
  * **Squash and merge**: Combines commits into one
  * **Rebase and merge**: Linear history
* Confirm merge

### 8. Deploy and Delete Branch

* Deploy merged changes
* Delete branch (GitHub offers this option)
* Update local repository:

```bash
# Switch to main
git checkout main

# Pull latest changes
git pull origin main

# Delete local branch
git branch -d feature-name
```

---

## Visual Workflow

```
main branch
    │
    ├─── feature-1 (branch)
    │    │
    │    └─── commits
    │         │
    │         └─── PR → merge ──┐
    │                           │
    ├─── feature-2 (branch)     │
    │    │                       │
    │    └─── commits            │
    │         │                  │
    │         └─── PR → merge ───┼──→ main (updated)
    │                            │
    └─── feature-3 (branch)      │
         │                       │
         └─── commits            │
              │                  │
              └─── PR → merge ───┘
```

---

## Pull Request Best Practices

### Writing Good PR Descriptions

* **What**: What does this PR do?
* **Why**: Why is this change needed?
* **How**: How was it implemented?
* **Testing**: How was it tested?
* **Screenshots**: Include if UI changes

### Example PR Description

```markdown
## What
Adds user authentication using OAuth2.

## Why
Users need to log in to access personalized features.

## How
- Integrated OAuth2 provider
- Added login/logout endpoints
- Created user session management

## Testing
- Tested login flow
- Verified session persistence
- Tested logout functionality

## Screenshots
[Include screenshots if applicable]
```

---

## Code Review Guidelines

### For Authors

* Keep PRs small and focused
* Write clear descriptions
* Respond to feedback promptly
* Fix issues before requesting re-review
* Thank reviewers

### For Reviewers

* Review promptly
* Be constructive and kind
* Explain reasoning
* Approve when ready
* Request changes when needed

---

## Merge Types Explained

### Create a Merge Commit

* Preserves complete history
* Shows branch structure
* Creates merge commit
* Best for: Feature branches

### Squash and Merge

* Combines all commits into one
* Cleaner main branch history
* Loses individual commit history
* Best for: Small fixes, documentation

### Rebase and Merge

* Linear history
* No merge commit
* Rewrites commit history
* Best for: Clean, linear history

---

## Handling Conflicts

### When Conflicts Occur

* Same file changed in both branches
* Git cannot automatically merge
* Requires manual resolution

### Resolving Conflicts

1. Update your branch:
   ```bash
   git checkout feature-name
   git pull origin main
   ```

2. Resolve conflicts in files
3. Stage resolved files:
   ```bash
   git add resolved-file.txt
   ```

4. Commit the merge:
   ```bash
   git commit -m "Merge main into feature-name"
   ```

5. Push updated branch:
   ```bash
   git push origin feature-name
   ```

---

## Common Workflows

### Feature Development

1. Create feature branch
2. Develop feature
3. Create PR
4. Get review
5. Merge to main
6. Deploy

### Bug Fixes

1. Create fix branch from main
2. Fix the bug
3. Create PR
4. Quick review
5. Merge to main
6. Deploy fix

### Hotfixes

1. Create hotfix branch from main
2. Fix critical issue
3. Create PR
4. Expedited review
5. Merge to main
6. Deploy immediately
7. Merge back to development branch

---

## Next Steps

* Practice with lab: `src/labs/lab-02-pull-request.md`
* Learn collaboration features: `src/03_collaboration/`
* Explore GitHub Actions: `src/04_github-tools/`

---

**Related Content**:
* Collaboration: `src/03_collaboration/pull-requests.md`
* Notes: `src/notes/common-mistakes.md`

