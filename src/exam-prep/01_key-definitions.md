# Key Definitions for GitHub Foundations Exam

Essential definitions and terminology that frequently appear in exam questions.

---

## Git vs GitHub

**Git**: Distributed version control system (VCS) that tracks changes in files. Runs locally on your machine.

**GitHub**: Cloud-based hosting service for Git repositories. Provides collaboration features, web interface, and additional tools.

**Key Distinction**: Git is the tool, GitHub is the platform that hosts Git repositories.

---

## Repository Concepts

**Repository (Repo)**: A storage location for your project files and their version history.

**Default Branch**: The main branch in a repository (typically `main` or `master`). New repositories start with this branch.

**Commit**: A snapshot of your repository at a specific point in time. Commits are immutable and identified by a unique hash.

**Commit Hash**: A unique identifier (SHA-1) for each commit. Example: `a1b2c3d4e5f6...`

---

## Branching and Merging

**Branch**: A parallel version of your repository. Allows you to work on features without affecting the main branch.

**Fork**: A copy of someone else's repository in your GitHub account. Used for contributing to open source projects.

**Clone**: Creating a local copy of a remote repository on your machine.

**Merge**: Combining changes from one branch into another.

**Pull Request (PR)**: A request to merge changes from one branch into another. Includes code review and discussion.

---

## Collaboration Concepts

**Issue**: A way to track bugs, feature requests, or tasks in a repository.

**Pull Request Review**: Process where team members review code changes before merging.

**CODEOWNERS**: A file that defines who must review code in specific directories.

**Merge Conflict**: When Git cannot automatically merge changes because both branches modified the same lines.

---

## GitHub Tools

**GitHub Actions**: Automation platform for CI/CD workflows. Runs on events like push, pull request, etc.

**GitHub Pages**: Static site hosting service. Publishes websites directly from a repository.

**Workflow**: Automated process defined in YAML files (`.github/workflows/`).

**Event**: Trigger that starts a workflow (e.g., `push`, `pull_request`, `schedule`).

---

## Security Concepts

**Secrets**: Encrypted variables stored in GitHub. Used for sensitive data like API keys, passwords.

**Variables**: Non-sensitive configuration values stored in GitHub.

**Dependabot**: Automated tool that checks for dependency vulnerabilities and creates PRs to update them.

**Branch Protection**: Rules that prevent direct pushes to protected branches, requiring PRs and reviews.

---

## Open Source Concepts

**License**: Legal document that defines how others can use your code. Common licenses: MIT, Apache 2.0, GPL.

**CONTRIBUTING.md**: Guidelines for how to contribute to a project.

**Code of Conduct**: Standards for acceptable behavior in a project community.

**Fork and Pull Request Workflow**: Standard way to contribute to open source projects.

---

## Common Exam Traps

**Fork vs Clone**: Fork creates a copy in your GitHub account. Clone creates a local copy on your machine.

**Branch vs Fork**: Branch is within the same repository. Fork is a separate copy of the repository.

**Secrets vs Variables**: Secrets are encrypted and masked in logs. Variables are plain text.

**Actions vs Pages**: Actions is for automation/CI/CD. Pages is for static site hosting.

---

**Last Updated**: December 28, 2025

