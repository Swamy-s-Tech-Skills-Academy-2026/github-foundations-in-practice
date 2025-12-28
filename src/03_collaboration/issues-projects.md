# Issues and Projects

**Session**: 02 - GitHub for Teams  
**Domain**: Collaboration Features (30%) + Project Management (7%)  
**Duration**: ~15 minutes

---

## Understanding Issues

Issues are GitHub's way to track bugs, feature requests, tasks, and discussions. They help teams organize work, prioritize tasks, and maintain project health.

### What Issues Are Used For

* **Bug Reports**: Track and fix problems
* **Feature Requests**: Propose new functionality
* **Tasks**: Track work items
* **Questions**: Ask for help or clarification
* **Documentation**: Track documentation needs

---

## Creating and Managing Issues

### Creating an Issue

1. Navigate to repository
2. Click "Issues" tab
3. Click "New issue"
4. Choose issue type (if templates exist)
5. Write title and description
6. Add labels
7. Assign to team member
8. Link to milestone or project
9. Submit issue

### Issue Best Practices

**Clear Title**:
* Descriptive and specific
* Action-oriented when possible
* Include context if needed

**Detailed Description**:
* What is the issue?
* Why is it important?
* How to reproduce (for bugs)?
* Expected vs actual behavior
* Screenshots if applicable

### Issue Templates

* Standardize issue creation
* Ensure required information
* Guide users
* Save time

Example template structure:
* Description
* Steps to reproduce
* Expected behavior
* Actual behavior
* Environment details

---

## Issue Workflow

### Standard Workflow

```
New Issue → In Progress → In Review → Done → Closed
```

### Issue States

* **Open**: Active issue, needs attention
* **Closed**: Resolved or no longer relevant
* **Reopened**: Issue closed but needs more work

### Linking Issues to PRs

* Link PR to issue in description
* Use keywords: "Fixes #123" or "Closes #123"
* Issue auto-closes when PR merges
* Maintains traceability

---

## Labels and Organization

### Using Labels

Labels help categorize and prioritize issues:

**Type Labels**:
* `bug`: Something isn't working
* `feature`: New feature request
* `documentation`: Documentation improvements
* `question`: Further information needed

**Priority Labels**:
* `priority: high`: Urgent
* `priority: medium`: Important
* `priority: low`: Nice to have

**Status Labels**:
* `in progress`: Being worked on
* `needs review`: Ready for review
* `blocked`: Cannot proceed

### Label Best Practices

* Use consistent naming
* Limit number of labels
* Use colors for visual organization
* Document label meanings

---

## Milestones

### What Are Milestones?

Milestones group related issues and track progress toward a specific goal or release.

### Using Milestones

* **Release Planning**: Track features for release
* **Sprint Planning**: Organize work by sprint
* **Goal Tracking**: Measure progress
* **Deadline Management**: Track time-bound work

### Milestone Features

* Due date
* Progress tracking
* Issue grouping
* Release notes generation

---

## GitHub Projects

### What Are Projects?

Projects are flexible boards for planning and tracking work. They provide a visual way to organize issues and pull requests.

### Project Views

**Board View**:
* Kanban-style columns
* Drag and drop issues
* Visual workflow
* Status at a glance

**Table View**:
* Spreadsheet-like interface
* Sortable columns
* Filterable data
* Bulk operations

### Project Workflow

1. Create project
2. Add issues and PRs
3. Organize in columns
4. Track progress
5. Update status

---

## Project Boards

### Board Structure

Typical columns:
* **Backlog**: Future work
* **To Do**: Ready to start
* **In Progress**: Currently working
* **In Review**: Awaiting review
* **Done**: Completed

### Customizing Boards

* Add custom columns
* Define workflows
* Set automation rules
* Filter by labels, assignees, milestones

---

## Project Automation

### Automated Workflows

* Move issues when PR created
* Move issues when PR merged
* Move issues based on labels
* Update status automatically

### Automation Benefits

* Saves manual work
* Keeps boards current
* Reduces errors
* Improves visibility

---

## Best Practices

### For Issue Management

* **Create Issues Early**: Don't wait
* **Be Specific**: Clear descriptions
* **Use Labels**: Organize effectively
* **Link Related**: Connect related issues
* **Close When Done**: Keep clean

### For Project Management

* **Keep Boards Updated**: Reflect reality
* **Use Automation**: Reduce manual work
* **Regular Reviews**: Check progress
* **Clear Workflows**: Define process
* **Team Visibility**: Everyone sees status

---

## Integration with Workflow

### Issues → Branches → PRs → Merge

1. **Create Issue**: Document need
2. **Create Branch**: Work on solution
3. **Create PR**: Propose solution
4. **Link PR to Issue**: Connect work
5. **Merge PR**: Implement solution
6. **Close Issue**: Mark complete

This creates traceability from problem to solution.

---

## Common Patterns

### Bug Report Pattern

1. User reports bug
2. Issue created
3. Bug reproduced
4. Fix developed
5. PR created and linked
6. Fix merged
7. Issue closed

### Feature Request Pattern

1. Feature requested
2. Issue created
3. Discussion and planning
4. Implementation
5. PR created
6. Review and merge
7. Issue closed

### Task Tracking Pattern

1. Task identified
2. Issue created
3. Assigned to team member
4. Work completed
5. Verified
6. Issue closed

---

## Next Steps

* Learn about discussions: `discussions.md`
* Practice with labs: `../labs/`
* Explore collaboration: `pull-requests.md`

---

**Related Content**:
* Pull Requests: `pull-requests.md`
* Code Reviews: `code-reviews.md`
* Discussions: `discussions.md`
* Labs: `../labs/`

