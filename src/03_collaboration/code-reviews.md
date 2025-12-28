# Code Reviews

**Session**: 02 - GitHub for Teams  
**Domain**: Collaboration Features (30%)  
**Duration**: ~10 minutes

---

## Understanding Code Reviews

Code review is the process where team members examine proposed code changes before they're merged. It's a collaborative practice that improves code quality, shares knowledge, and catches issues early.

### Why Code Reviews Matter

* **Quality**: Catch bugs before production
* **Learning**: Share knowledge across team
* **Consistency**: Maintain coding standards
* **Security**: Identify security vulnerabilities
* **Documentation**: Ensure code is understandable

---

## The Review Process

### Step-by-Step Review Flow

1. **Author Creates PR**: Proposes changes via pull request
2. **Reviewer Assigned**: Team member assigned to review
3. **Reviewer Examines**: Reads code, tests if possible
4. **Feedback Provided**: Comments, suggestions, questions
5. **Author Responds**: Addresses feedback
6. **Iteration**: Back-and-forth until satisfied
7. **Approval**: Reviewer approves when ready
8. **Merge**: Changes merged into codebase

### Review Checklist

When reviewing code, consider:

* **Functionality**: Does it work as intended?
* **Readability**: Is the code easy to understand?
* **Performance**: Are there efficiency concerns?
* **Security**: Any security vulnerabilities?
* **Testing**: Is it adequately tested?
* **Documentation**: Is it well-documented?
* **Standards**: Follows team conventions?

---

## Types of Review Feedback

### General Comments

* Overall feedback on the PR
* High-level suggestions
* Architecture or design concerns
* General questions

### Line-Specific Comments

* Comments on specific lines of code
* Point out issues or improvements
* Suggest alternative approaches
* Ask clarifying questions

### Code Suggestions

* Proposed code changes
* Can be applied directly
* Shows exact replacement
* Saves time for author

### Questions

* Seek clarification
* Understand intent
* Explore alternatives
* Learn from author

---

## Review Actions

### Approve

* Code looks good
* Ready to merge
* No blocking issues
* Meets quality standards

### Request Changes

* Issues need addressing
* Blocking merge
* Must be fixed
* Re-review required

### Comment

* General feedback
* Non-blocking suggestions
* Questions or observations
* No approval needed

---

## Best Practices for Reviewers

### Be Constructive

* Focus on improvement
* Explain reasoning
* Suggest solutions
* Be respectful

### Review Promptly

* Don't let PRs sit
* Review within 24-48 hours
* Communicate if delayed
* Set expectations

### Test When Possible

* Run code locally
* Verify functionality
* Check edge cases
* Test integration

### Ask Questions

* Seek clarification
* Understand context
* Learn from others
* Don't assume

---

## Best Practices for Authors

### Prepare Your PR

* Write clear description
* Keep PRs focused
* Test before submitting
* Link related issues

### Respond to Feedback

* Acknowledge comments
* Thank reviewers
* Address concerns
* Ask for clarification if needed

### Update PR

* Make requested changes
* Push updates
* Request re-review
* Mark conversations resolved

### Learn from Reviews

* View as learning opportunity
* Understand different perspectives
* Improve coding skills
* Share knowledge

---

## CODEOWNERS File

### What is CODEOWNERS?

A `CODEOWNERS` file specifies who must review code in specific parts of a repository. It ensures the right people review changes.

### How It Works

* File in repository root or `.github/` directory
* Lists file patterns and owners
* Automatically requests reviews
* Enforces review requirements

### Example CODEOWNERS

```
# Global owners
* @team-leads

# Frontend code
/src/frontend/ @frontend-team

# Backend code
/src/backend/ @backend-team

# Documentation
/docs/ @docs-team

# Configuration
*.config.js @devops-team
```

### Benefits

* **Automatic Assignment**: Right reviewers automatically
* **Enforcement**: Required reviews before merge
* **Ownership**: Clear responsibility
* **Efficiency**: Saves time

---

## Review Requirements

### Required Reviews

* Minimum number of approvals
* Can require specific reviewers
* Can require CODEOWNER approval
* Enforced by branch protection

### Dismissing Reviews

* Stale reviews can be dismissed
* When code changes significantly
* Requires new review
* Maintains quality

### Review Assignment

* Assign specific reviewers
* Request reviews from teams
* Use CODEOWNERS for automatic
* Rotate reviewers

---

## Common Review Scenarios

### Scenario 1: Simple Fix

* Quick review
* Minor changes
* Low risk
* Fast approval

### Scenario 2: Complex Feature

* Thorough review
* Multiple reviewers
* Architecture discussion
* Extended review time

### Scenario 3: Security Change

* Security-focused review
* Careful examination
* May require security team
* High priority

### Scenario 4: Refactoring

* Focus on structure
* Ensure no behavior change
* Check test coverage
* Verify functionality

---

## Review Tools and Features

### Review Interface

* Side-by-side diff view
* Inline commenting
* Code suggestions
* Conversation threads

### Review Filters

* Filter by reviewer
* Filter by status
* Filter by file
* Filter by comment type

### Review Notifications

* Email notifications
* In-app notifications
* Team mentions
* Status updates

---

## Handling Disagreements

### When Opinions Differ

* Discuss respectfully
* Explain reasoning
* Consider alternatives
* Seek consensus

### Escalation

* Involve team lead if needed
* Get additional opinions
* Document decision
* Learn from experience

---

## Next Steps

* Learn about issues: `issues-projects.md`
* Practice with PRs: `pull-requests.md`
* Explore workflows: `../01_github-basics/04_github-flow.md`

---

**Related Content**:
* Pull Requests: `pull-requests.md`
* Issues: `issues-projects.md`
* Labs: `../labs/lab-02-pull-request.md`

