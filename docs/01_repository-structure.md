# Repository Structure

**Version**: 2.0  
**Last Updated**: December 24, 2025  
**Purpose**: Single source of truth for repository structure

> **Note**: This document should be referenced from `.github/copilot-instructions.md`, `.cursor/rules/02_repository-structure.mdc`, `README.md`, and other documentation files. When the structure changes, update this file first, then update references.

---

## Complete Repository Structure

```text
github-foundations-journey/
│
├── README.md
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
└── resources/
    ├── official-links.md
    ├── practice-questions.md
    └── cheat-sheets.md
```

---

## Key Structure Notes

### File Naming Conventions

- **Educational Content** (`src/01_introduction/` through `src/08_failures/`):
  - ✅ Use zero-padded numeric prefixes: `01_`, `02_`, etc.
  - ❌ **NEVER** use `00_` prefix - **NO EXCEPTIONS**
  - ✅ Use hyphens for multi-word names: `01_modern-system-design.md`
  - ✅ Split files use: `topic-slug-part1.md`, `topic-slug-part2.md` (avoid `A/B/C`)

- **Case Studies** (`src/07_case-studies/`):
  - ✅ Can use numbered files: `01_requirements.md`, `02_back-of-envelope.md`, etc.
  - ✅ Or use standard names: `requirements.md`, `high-level-design.md`, etc.
  - ✅ Diagrams co-located in `diagrams/` folder within each case study

- **References** (`src/references/`):
  - ✅ Logical names: `books.md`, `papers.md`, `tools.md`
  - ⚠️ No numbering required

### Content Organization

1. **Learning Progression**: Content follows logical learning order (01 → 08)
2. **Split Files**: Files exceeding 150 lines are split into parts (e.g., `03_databases-part1.md`, `03_databases-part2.md`)
3. **Case Study Structure**: Each case study includes:
   - Requirements, Back-of-Envelope, HLD, LLD, Scalability, Observability, Security, Trade-offs
   - Diagrams folder with C4 and sequence diagrams

### Special Directories

- **`source-material/`**: Staging area for source content (git-ignored)
  - Raw source materials placed here before migration
  - Files are transformed and migrated to `src/` following zero-copy policy
  - Source files remain after migration (user deletes manually)

- **`docs/review-reports/`**: Review and migration verification reports
  - Date-based naming: `DDMonYYYY-description.md`
  - Documents migration status, rule compliance, and content quality

---

## Update Protocol

**When repository structure changes**:

1. ✅ **Update this file first** (`docs/02_repository-structure.md`)
2. ✅ **Update references** in:
   - `.github/copilot-instructions.md` - Reference this file
   - `.cursor/rules/02_repository-structure.mdc` - Reference this file
   - `README.md` - Reference this file
3. ✅ **Verify consistency** across all documentation

**Self-Check Question**: "Did I update `docs/02_repository-structure.md` first?" - If no, STOP and do it NOW.

---

## References

- **Repository Structure**: This file (`docs/02_repository-structure.md`)
- **Content Rules**: `.cursor/rules/01_educational-content-rules.mdc`
- **Learning Path**: `docs/ROADMAP.md`
- **Content Index**: `src/CONTENT_INDEX.md`
- **GitHub Copilot Instructions**: `.github/copilot-instructions.md`
