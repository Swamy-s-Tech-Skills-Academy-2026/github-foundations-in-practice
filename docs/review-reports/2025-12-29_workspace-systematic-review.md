# Workspace Systematic Review Report

**Maintainer**: Swamy  
**Date**: 29 Dec 2025 (IST)  
**Repository**: `github-foundations-in-practice`

## Scope

Systematic review of repository structure + documentation content across:

- Root documentation files (`README.md`, `CONTRIBUTING.md`, `SECURITY.md`, `CODE_OF_CONDUCT.md`)
- Governance/config (`.github/`, `.cursor/`, `.copilot/`, markdownlint + lychee config)
- Learning content (`src/`)
- Planning + meetup material (`docs/`)
- Tooling (`tools/`)

## Method

- Verified current file inventory and directory contents.
- Ran automated checks via PowerShell scripts in `tools/psscripts/`:
  - `Get-RepoStats.ps1`
  - `Quick-HealthCheck.ps1`
  - `Find-DuplicateContent.ps1`

## Key Findings (High Priority)

### 1) Repository structure documentation was out-of-sync

- `docs/01_repository-structure.md` did not match the actual tree (missing `.github/`, `.cursor/`, `.copilot/`, `tools/`, and many file names).
- The same file also contained duplicated directory entries in the tree.

✅ Fixed as part of this review.

### 2) Broken links in `docs/` (now resolved)

- `docs/03_session-overview.md` and `docs/sessions/README.md` referenced a non-existent `templates/session-template.md`.
- Meetup session files referenced non-existent `docs/sessions/<session>/` directories.

✅ Fixed by linking to existing templates under `docs/templates/` and to relevant `src/` content.

### 3) `src/` folder READMEs listed files that do not exist

- `src/04_github-tools/README.md` listed Actions/Pages/Marketplace docs that aren’t present yet.
- `src/05_security-and-best-practices/README.md` listed several security docs that aren’t present yet.

✅ Fixed by separating **Currently available** vs **Planned**.

## Key Findings (Medium Priority)

### 4) Content gaps by domain

Current state:

- Domain 1 (`src/01_github-basics/`) is well populated.
- Collaboration (`src/03_collaboration/`) is populated.
- Modern Development (`src/04_github-tools/`) is currently a scaffold (README + `.gitkeep`).
- Security (`src/05_security-and-best-practices/`) has README + code scanning only.
- Working with Repositories (`src/02_working-with-repositories/`) is empty (only `.gitkeep`).
- Open Source & Community (`src/06_open-source-and-community/`) is empty (only `.gitkeep`).
- Labs (`src/labs/`) is empty (only `.gitkeep`).

Recommendation:

- Prioritize filling `src/02_working-with-repositories/` and `src/labs/` next, because they unlock hands-on practice and complete the core exam workflow.

### 5) Session/meetup numbering can be confusing

- `docs/03_session-overview.md` is explicitly the “single source of truth” for the learning-roadmap sessions.
- Meetup sessions (under `docs/meetup/`) don’t necessarily match the learning-roadmap numbering.

✅ Reduced confusion by removing hard-coded session numbers from the meetup files where they didn’t match the roadmap.

## Changes Applied During This Review

- Added PowerShell automation scripts:
  - `tools/psscripts/Get-RepoStats.ps1`
  - `tools/psscripts/Quick-HealthCheck.ps1`
  - `tools/psscripts/Get-FileStats.ps1`
  - `tools/psscripts/Get-MarkdownSummary.ps1`
  - `tools/psscripts/Compare-DocFiles.ps1`
  - `tools/psscripts/Find-DuplicateContent.ps1`
- Updated repository structure single source of truth:
  - `docs/01_repository-structure.md`
- Fixed broken doc links:
  - `docs/03_session-overview.md`
  - `docs/sessions/README.md`
  - `docs/meetup/01_...` through `04_...`
- Updated roadmap status for completed content:
  - `docs/03_session-overview.md` (Sessions 01 and 02 marked ✅ Complete)
- Updated/clarified `src` READMEs:
  - `src/01_github-basics/README.md`
  - `src/04_github-tools/README.md`
  - `src/05_security-and-best-practices/README.md`
- Refreshed dates in structure-related rule files:
  - `.github/copilot-instructions.md`
  - `.cursor/rules/02_repository-structure.mdc`

## How to Re-run Checks

From repo root:

```powershell
PowerShell -NoProfile -ExecutionPolicy Bypass -File .\tools\psscripts\Get-RepoStats.ps1
PowerShell -NoProfile -ExecutionPolicy Bypass -File .\tools\psscripts\Quick-HealthCheck.ps1
PowerShell -NoProfile -ExecutionPolicy Bypass -File .\tools\psscripts\Find-DuplicateContent.ps1 -MinOccurrences 5
```

## Recommended Next Actions (Backlog)

- Add initial content to `src/02_working-with-repositories/` (branching, commits, merges).
- Add at least one lab under `src/labs/` (e.g., PR workflow) and expand from there.
- Create the planned `src/04_github-tools/*` docs (Actions, Pages, Marketplace) or move them into a “Planned” section in the domain README until written.
- Create the planned `src/05_security-and-best-practices/*` docs (secrets, branch protection, permissions) or keep them explicitly planned.

---

**Reviewer**: GitHub Copilot (GPT-5.2)
