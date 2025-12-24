# Repository Structure

**Version**: 1.0  
**Last Updated**: December 24, 2025  
**Purpose**: Single source of truth for repository structure

> **Note**: This document should be referenced from `.github/copilot-instructions.md`, `.cursor/rules/02_repository-structure.mdc`, `README.md`, and other documentation files. When the structure changes, update this file first, then update references.

---

## Complete Repository Structure

```text
github-foundations-in-practice/
│
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── .gitignore
├── lychee.toml
│
├── progress/
│   ├── milestones.md
│   ├── study-log.md
│   └── exam-readiness-checklist.md
│
├── 01_github-basics/
│   ├── README.md
│   ├── concepts.md
│   ├── git-vs-github.md
│   ├── repositories.md
│   └── markdown-basics.md
│
├── 02_working-with-repositories/
│   ├── README.md
│   ├── cloning-forking.md
│   ├── commits-history.md
│   ├── branching-strategies.md
│   └── merging-rebasing.md
│
├── 03_collaboration/
│   ├── README.md
│   ├── pull-requests.md
│   ├── code-reviews.md
│   ├── issues-projects.md
│   └── discussions.md
│
├── 04_github-tools/
│   ├── README.md
│   ├── github-actions.md
│   ├── workflows-basics.md
│   ├── marketplace.md
│   └── github-pages.md
│
├── 05_security-and-best-practices/
│   ├── README.md
│   ├── permissions-roles.md
│   ├── branch-protection.md
│   ├── secrets-management.md
│   └── code-scanning-overview.md
│
├── 06_open-source-and-community/
│   ├── README.md
│   ├── open-source-basics.md
│   ├── licenses.md
│   ├── contributing-guidelines.md
│   └── code-of-conduct.md
│
├── labs/
│   ├── lab-01-create-repo.md
│   ├── lab-02-pull-request.md
│   ├── lab-03-actions-workflow.md
│   └── lab-04-pages-deployment.md
│
├── notes/
│   ├── common-mistakes.md
│   ├── exam-tips.md
│   └── glossary.md
│
├── resources/
│   ├── official-links.md
│   ├── practice-questions.md
│   └── cheat-sheets.md
│
├── docs/
│   ├── 01_repository-structure.md (this file)
│   ├── images/
│   ├── meetup/
│   ├── review-reports/
│   └── sessions/
│
└── src/
    └── .gitkeep
```

---

## Key Structure Notes

### File Naming Conventions

- **Domain Folders** (`01_github-basics/` through `06_open-source-and-community/`):
  - ✅ Use zero-padded numeric prefixes: `01_`, `02_`, etc.
  - ✅ Use hyphens for multi-word names: `01_github-basics/`
  - ✅ Content files use descriptive names: `concepts.md`, `pull-requests.md`

- **Labs** (`labs/`):
  - ✅ Use numbered lab files: `lab-01-create-repo.md`
  - ✅ Each lab includes objective, steps, and expected outcome

- **Notes** (`notes/`):
  - ✅ Use descriptive names: `common-mistakes.md`, `exam-tips.md`, `glossary.md`

- **Resources** (`resources/`):
  - ✅ Use logical names: `official-links.md`, `practice-questions.md`, `cheat-sheets.md`

### Content Organization

1. **Learning Progression**: Content follows GitHub Foundations exam domains (01 → 06)
2. **Hands-On Practice**: Labs provide practical exercises
3. **Reference Materials**: Notes and resources support learning

### Special Directories

- **`progress/`**: Tracks learning milestones and exam readiness
- **`docs/`**: Additional documentation, images, and session notes
- **`src/`**: Placeholder directory (currently empty)

---

## Update Protocol

**When repository structure changes**:

1. ✅ **Update this file first** (`docs/01_repository-structure.md`)
2. ✅ **Update references** in:
   - `.github/copilot-instructions.md` - Reference this file
   - `.cursor/rules/02_repository-structure.mdc` - Reference this file
   - `README.md` - Reference this file
3. ✅ **Verify consistency** across all documentation

**Self-Check Question**: "Did I update `docs/01_repository-structure.md` first?" - If no, STOP and do it NOW.

---

## References

- **Repository Structure**: This file (`docs/01_repository-structure.md`)
- **Learning Path**: `README.md`
- **GitHub Copilot Instructions**: `.github/copilot-instructions.md`
