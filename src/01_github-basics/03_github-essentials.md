# GitHub Essentials

**Session**: 01 - Introduction to Git and GitHub  
**Domain**: GitHub Fundamentals (20%)  
**Duration**: ~15 minutes

---

## What is GitHub?

**GitHub** is a cloud-based hosting platform for Git repositories. It provides:

* Remote repository hosting
* Collaboration tools (Issues, Pull Requests, Discussions)
* Project management features
* CI/CD automation (GitHub Actions)
* Security features
* Community features

---

## GitHub vs Git

| Git | GitHub |
|-----|--------|
| Version control tool | Hosting platform |
| Runs on your computer | Cloud service |
| Local repositories | Remote repositories |
| Command-line interface | Web interface + CLI |
| Free and open source | Free for public repos |

---

## Creating a GitHub Account

### Sign Up Process

1. Go to [github.com](https://github.com)
2. Click "Sign up"
3. Choose username (cannot be changed easily)
4. Enter email address
5. Create password
6. Verify email address

### Setting Up Your Profile

* Add profile picture
* Write a bio
* Add location and website
* Link social media accounts
* Pin important repositories

---

## Repository Visibility

### Public Repositories

* Visible to everyone
* Anyone can view code
* Free for unlimited public repos
* Great for open source
* Can be cloned by anyone

### Private Repositories

* Only visible to you and collaborators
* Requires paid plan (or free for individuals)
* Control who can access
* Suitable for proprietary code
* Can be made public later

### Internal Repositories (Enterprise)

* Visible to organization members
* Not accessible to public
* Requires GitHub Enterprise

---

## Forking vs Cloning

### Forking

* Creates a copy on your GitHub account
* Maintains connection to original
* Used for contributing to others' projects
* You own the fork
* Can create pull requests to original

**When to Fork**:
* Contributing to open source projects
* Experimenting with someone else's code
* Creating your own version

### Cloning

* Downloads repository to your computer
* Creates local copy
* Used for working on your own projects
* No connection to original (unless you set up remote)

**When to Clone**:
* Working on your own repositories
* Setting up local development environment
* Getting a copy to work on locally

---

## Exploring Repositories

### Key Areas

* **Code**: Source files and directory structure
* **Issues**: Bug reports and feature requests
* **Pull Requests**: Proposed changes
* **Discussions**: Community conversations
* **Actions**: CI/CD workflows
* **Projects**: Project management boards
* **Wiki**: Documentation
* **Security**: Security advisories
* **Insights**: Analytics and graphs

### Repository Structure

```
repository-name/
├── README.md          # Project description
├── .gitignore         # Files to ignore
├── LICENSE            # License file
├── src/               # Source code
├── docs/              # Documentation
└── tests/             # Test files
```

---

## Basic GitHub Operations

### Creating a Repository

1. Click "+" icon → "New repository"
2. Enter repository name
3. Choose visibility (public/private)
4. Initialize with README (optional)
5. Add .gitignore (optional)
6. Choose license (optional)
7. Click "Create repository"

### Pushing Local Repository to GitHub

```bash
# Add remote repository
git remote add origin https://github.com/username/repo-name.git

# Push to GitHub
git push -u origin main
```

### Cloning a Repository

```bash
# Clone via HTTPS
git clone https://github.com/username/repo-name.git

# Clone via SSH
git clone git@github.com:username/repo-name.git
```

---

## GitHub Features Overview

### Issues

* Track bugs and feature requests
* Assign to team members
* Use labels for organization
* Link to pull requests
* Close automatically with keywords

### Pull Requests

* Propose changes to codebase
* Request code review
* Discuss changes before merging
* Run automated checks
* Merge when approved

### Discussions

* Community Q&A
* Announcements
* General conversations
* Separate from code issues

### Actions

* Automate workflows
* Run CI/CD pipelines
* Deploy applications
* Run tests automatically

---

## Best Practices

### README Files

* Always include a README.md
* Explain what the project does
* Include installation instructions
* Add usage examples
* Link to documentation

### Repository Organization

* Use clear naming conventions
* Organize files logically
* Keep repositories focused
* Use branches for features
* Tag releases

### Collaboration

* Use issues for tracking
* Create pull requests for changes
* Write clear commit messages
* Respond to reviews promptly
* Follow code of conduct

---

## Next Steps

* Learn GitHub Flow: `04_github-flow.md`
* Practice with labs: `src/labs/lab-01-create-repo.md`
* Explore collaboration: `src/03_collaboration/`

---

**Related Content**:
* Resources: `src/resources/official-links.md`
* Notes: `src/notes/glossary.md`

