# Repository Structure

**Version**: 2.0  
**Last Updated**: December 29, 2025  
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
├── SECURITY.md
├── CODE_OF_CONDUCT.md
├── .gitignore
├── lychee.toml
├── .markdownlint-cli2.yaml
├── .markdownlint.json
├── .markdownlintignore
│
├── .copilot/
│   └── settings.json
│
├── .cursor/
│   └── rules/
│       ├── 01_educational-content-rules.mdc
│       ├── 02_repository-structure.mdc
│       ├── 03_quality-assurance.mdc
│       ├── 04_markdown-standards.mdc
│       ├── 05_primary-directives.mdc
│       ├── 06_cross-domain-integration.mdc
│       ├── 07_file-naming-conventions.mdc
│       └── README.md
│
├── .github/
│   ├── copilot-instructions.md
│   ├── pull_request_template.md
│   └── ISSUE_TEMPLATE/
│       ├── bug_report.md
│       ├── config.yml
│       ├── content_suggestion.md
│       └── question.md
│
├── docs/
│   ├── 01_repository-structure.md (this file)
│   ├── 02_master-plan.md
│   ├── 03_session-overview.md
│   ├── images/
│   │   └── .gitkeep
│   ├── meetup/
│   │   ├── .gitkeep
│   │   ├── 01_meetup-introduction-git-github.md
│   │   ├── 02_meetup-github-for-teams.md
│   │   ├── 03_meetup-introduction-to-github-products.md
│   │   ├── 04_meetup-configure-code-scanning.md
│   │   └── sessions.md
│   ├── review-reports/
│   │   └── .gitkeep
│   ├── sessions/
│   │   ├── .gitkeep
│   │   └── README.md
│   └── templates/
│       ├── .gitkeep
│       ├── facilitator-notes-template.md
│       ├── meetup-session-template.md
│       └── src-content-template.md
│
├── source-material/
│   └── README.md
│
├── src/
│   ├── .gitkeep
│   ├── 01_github-basics/
│   │   ├── .gitkeep
│   │   ├── 01_version-control-basics.md
│   │   ├── 02_git-essentials.md
│   │   ├── 03_github-essentials.md
│   │   ├── 04_github-flow.md
│   │   ├── 05_github-platform-overview.md
│   │   ├── 06_accounts-and-plans.md
│   │   ├── 07_billing-and-usage.md
│   │   ├── 08_github-desktop-mobile.md
│   │   └── README.md
│   ├── 02_working-with-repositories/
│   │   └── .gitkeep
│   ├── 03_collaboration/
│   │   ├── .gitkeep
│   │   ├── code-reviews.md
│   │   ├── discussions.md
│   │   ├── issues-projects.md
│   │   ├── pull-requests.md
│   │   └── README.md
│   ├── 04_github-tools/
│   │   ├── .gitkeep
│   │   └── README.md
│   ├── 05_security-and-best-practices/
│   │   ├── .gitkeep
│   │   ├── code-scanning-overview.md
│   │   └── README.md
│   ├── 06_open-source-and-community/
│   │   └── .gitkeep
│   ├── exam-prep/
│   │   ├── 01_key-definitions.md
│   │   ├── 02_trick-questions.md
│   │   ├── 03_exam-mindset.md
│   │   └── README.md
│   ├── labs/
│   │   └── .gitkeep
│   ├── notes/
│   │   ├── .gitkeep
│   │   ├── common-mistakes.md
│   │   ├── exam-tips.md
│   │   └── glossary.md
│   ├── progress/
│   │   ├── .gitkeep
│   │   ├── exam-readiness-checklist.md
│   │   ├── milestones.md
│   │   └── study-log.md
│   └── resources/
│       ├── .gitkeep
│       ├── cheat-sheets.md
│       ├── official-links.md
│       └── practice-questions.md
│
└── tools/
  └── psscripts/
    ├── .gitkeep
    ├── Compare-DocFiles.ps1
    ├── Find-DuplicateContent.ps1
    ├── Get-FileStats.ps1
    ├── Get-MarkdownSummary.ps1
    ├── Get-RepoStats.ps1
    └── Quick-HealthCheck.ps1
```

---

## Key Structure Notes

### File Naming Conventions

- **Domain Folders** (`src/01_github-basics/` through `src/06_open-source-and-community/`):
  - ✅ Use zero-padded numeric prefixes: `01_`, `02_`, etc.
  - ✅ Use hyphens for multi-word names: `01_github-basics/`
  - ✅ Content files use descriptive names: `concepts.md`, `pull-requests.md`

- **Labs** (`src/labs/`):
  - ✅ Use numbered lab files: `lab-01-create-repo.md`
  - ✅ Each lab includes objective, steps, and expected outcome

- **Notes** (`src/notes/`):
  - ✅ Use descriptive names: `common-mistakes.md`, `exam-tips.md`, `glossary.md`

- **Resources** (`src/resources/`):
  - ✅ Use logical names: `official-links.md`, `practice-questions.md`, `cheat-sheets.md`

### Content Organization

1. **Learning Progression**: Content follows GitHub Foundations exam domains (01 → 06)
2. **Hands-On Practice**: Labs provide practical exercises
3. **Reference Materials**: Notes and resources support learning
4. **All Content Under `src/`**: All learning materials, labs, notes, progress, and resources are organized under the `src/` directory

### Special Directories

- **`src/progress/`**: Tracks learning milestones and exam readiness
- **`docs/`**: Additional documentation, images, and session notes
- **`tools/psscripts/`**: PowerShell automation scripts for repo analysis and maintenance
- **`source-material/`**: Staging area for source content (git-ignored)
  - Raw source materials placed here before migration
  - Files are transformed and migrated to `src/` following content rules
  - Source files remain after migration (user deletes manually)

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
