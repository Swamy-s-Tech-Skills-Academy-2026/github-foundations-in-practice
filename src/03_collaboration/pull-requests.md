# Pull Requests

**Session**: 02 - GitHub for Teams  
**Domain**: Collaboration Features (30%)  
**Duration**: ~15 minutes

---

## What is a Pull Request?

A **Pull Request (PR)** is a proposal to merge changes from one branch into another. It's the primary mechanism for:

* Proposing code changes
* Requesting code review
* Discussing changes before merging
* Running automated checks
* Collaborating on code

---

## The Pull Request Workflow

### Standard Workflow

1. **Create Branch**: Work on feature in separate branch
2. **Make Changes**: Edit files and commit
3. **Push Branch**: Push branch to GitHub
4. **Create PR**: Open pull request on GitHub
5. **Review**: Team members review code
6. **Discuss**: Address feedback and questions
7. **Approve**: Get approval from reviewers
8. **Merge**: Merge into target branch
9. **Delete Branch**: Clean up merged branch

---

## Creating a Pull Request

### From GitHub Web Interface

1. Navigate to repository
2. Click "Compare & pull request" (appears after pushing branch)
3. Or click "Pull requests" tab → "New pull request"
4. Select base branch (usually `main`)
5. Select compare branch (your feature branch)
6. Review changes
7. Write description
8. Add reviewers
9. Link related issues
10. Click "Create pull request"

### PR Description Best Practices

* **What**: What does this PR do?
* **Why**: Why is this change needed?
* **How**: How was it implemented?
* **Testing**: How was it tested?
* **Screenshots**: Include if UI changes
* **Checklist**: List of tasks completed

### Example PR Description

```markdown
## What
Adds user authentication using OAuth2.

## Why
Users need to log in to access personalized features. This implements
the authentication flow required for user-specific content.

## How
- Integrated OAuth2 provider (Google)
- Added login/logout endpoints
- Created user session management
- Added authentication middleware

## Testing
- [x] Tested login flow
- [x] Verified session persistence
- [x] Tested logout functionality
- [x] Tested error handling

## Screenshots
[Include screenshots of login UI]

## Related Issues
Closes #123
```

---

## Reviewing Pull Requests

### As a Reviewer

* **Read the Description**: Understand the change
* **Review the Code**: Check for issues
* **Test if Possible**: Run the code locally
* **Leave Comments**: Provide constructive feedback
* **Approve or Request Changes**: Make decision

### Types of Comments

* **General Comments**: Overall feedback
* **Line Comments**: Specific code suggestions
* **Suggestions**: Proposed code changes
* **Questions**: Clarifications needed

### Review Actions

* **Approve**: Code looks good, ready to merge
* **Request Changes**: Issues need to be addressed
* **Comment**: General feedback, no approval needed

---

## PR Status and Checks

### Status Indicators

* **Draft**: Work in progress, not ready for review
* **Open**: Ready for review
* **Approved**: Has required approvals
* **Changes Requested**: Needs updates
* **Merged**: Successfully merged
* **Closed**: Not merged (rejected or abandoned)

### Automated Checks

* **CI/CD**: Automated tests run
* **Code Quality**: Linting and formatting checks
* **Security**: Security scanning
* **Status Checks**: Must pass before merging

---

## Merge Types

### Create a Merge Commit

* Preserves complete history
* Shows branch structure
* Creates merge commit
* **Best for**: Feature branches

### Squash and Merge

* Combines all commits into one
* Cleaner main branch history
* Loses individual commit history
* **Best for**: Small fixes, documentation

### Rebase and Merge

* Linear history
* No merge commit
* Rewrites commit history
* **Best for**: Clean, linear history

---

## Best Practices

### For Authors

* **Keep PRs Small**: Focused, single-purpose changes
* **Write Clear Descriptions**: Explain what and why
* **Link Related Issues**: Connect to issue tracking
* **Respond Promptly**: Address feedback quickly
* **Update PR**: Keep branch up to date with base
* **Test Before Submitting**: Ensure code works

### For Reviewers

* **Review Promptly**: Don't let PRs sit
* **Be Constructive**: Provide helpful feedback
* **Explain Reasoning**: Why changes are needed
* **Approve When Ready**: Don't block unnecessarily
* **Test if Possible**: Verify changes work

### PR Size Guidelines

* **Small**: < 200 lines (ideal)
* **Medium**: 200-500 lines (acceptable)
* **Large**: 500-1000 lines (consider splitting)
* **Very Large**: > 1000 lines (split into multiple PRs)

---

## Handling Feedback

### Responding to Comments

* **Acknowledge**: Thank reviewers
* **Clarify**: Explain if misunderstood
* **Fix**: Address valid concerns
* **Discuss**: Engage in conversation

### Updating PR

1. Make requested changes
2. Commit changes
3. Push to same branch
4. PR updates automatically
5. Request re-review if needed

### Resolving Conversations

* Mark resolved when addressed
* Continue discussion if needed
* Close when satisfied

---

## Advanced PR Features

### Draft Pull Requests

* Mark as draft when not ready
* Prevents accidental merging
* Can convert to ready when done
* Good for early feedback

### PR Templates

* Standardize PR descriptions
* Include required information
* Ensure consistency
* Save time

### Auto-merge

* Automatically merge when conditions met
* Requires approvals
* Requires passing checks
* Useful for CI/CD workflows

### PR Reviews

* Required reviewers
* Code owner reviews
* Review assignment
* Review notifications

---

## Common Workflows

### Feature Development

1. Create feature branch
2. Develop feature
3. Create draft PR
4. Get early feedback
5. Mark as ready
6. Get approvals
7. Merge to main

### Bug Fixes

1. Create fix branch
2. Fix the bug
3. Create PR
4. Quick review
5. Merge to main

### Hotfixes

1. Create hotfix branch
2. Fix critical issue
3. Create PR
4. Expedited review
5. Merge immediately
6. Deploy fix

---

## Next Steps

* Learn about code reviews: `code-reviews.md`
* Explore issues: `issues-projects.md`
* Practice with lab: `src/labs/lab-02-pull-request.md`

---

**Related Content**:
* Code Reviews: `code-reviews.md`
* GitHub Flow: `../01_github-basics/04_github-flow.md`
* Labs: `../labs/lab-02-pull-request.md`

