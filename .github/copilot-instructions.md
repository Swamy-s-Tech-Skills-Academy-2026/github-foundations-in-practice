# GitHub Copilot Instructions for GitHub Foundations Learning Journey

**Version**: 1.0  
**Last Updated**: December 24, 2025  
**Repository**: `github-foundations-in-practice`

---

## 🎯 Repository Purpose

**GitHub Foundations Learning Journey** is a personal learning repository documenting the structured journey toward the **GitHub Foundations Certification**.

### What This Repository Provides

- **GitHub Basics**: Core concepts, terminology, Git vs GitHub, repositories, Markdown
- **Working with Repositories**: Cloning, forking, commits, branching, merging, rebasing
- **Collaboration**: Pull requests, code reviews, issues, projects, discussions
- **GitHub Tools**: Actions, workflows, Marketplace, Pages
- **Security & Best Practices**: Permissions, roles, branch protection, secrets, code scanning
- **Open Source & Community**: OSS basics, licenses, contributing guidelines, code of conduct
- **Hands-On Labs**: Practical exercises for creating repos, PRs, workflows, and Pages
- **Exam Preparation**: Study notes, tips, common mistakes, glossary, practice questions

### Target Audience

- Swamy (personal learning journey)
- Developers preparing for GitHub Foundations Certification
- Engineers learning GitHub fundamentals
- Teams adopting GitHub best practices

### Business Value

- Structured exam preparation
- Practical GitHub knowledge
- Hands-on experience through labs
- Comprehensive coverage of all exam domains

---

## 📁 Repository Structure

> **📋 Single Source of Truth**: The complete and up-to-date repository structure is maintained in [`docs/01_repository-structure.md`](../docs/01_repository-structure.md). This file should be referenced for the authoritative structure. When the structure changes, update that file first, then update references here.

For the complete repository structure, see: **[docs/01_repository-structure.md](../docs/01_repository-structure.md)**

**Quick Overview**:

- `src/01_github-basics/` - Core GitHub concepts and terminology
- `src/02_working-with-repositories/` - Branching, commits, merges
- `src/03_collaboration/` - Pull requests, reviews, issues
- `src/04_github-tools/` - Actions, Pages, Marketplace
- `src/05_security-and-best-practices/` - Permissions, secrets, protection
- `src/06_open-source-and-community/` - Licenses, OSS workflows
- `src/labs/` - Hands-on exercises
- `src/notes/` - Exam tips, glossary, common mistakes
- `src/resources/` - Official links, practice questions, cheat sheets
- `src/progress/` - Milestones, study log, readiness tracking

---

## 🔧 Development Guidelines

### When Working with GitHub Foundations Content

1. **Follow Exam Domain Structure**: Content organized by GitHub Foundations exam domains
2. **Use Descriptive Names**: Files use clear, descriptive names (e.g., `concepts.md`, `pull-requests.md`)
3. **Keep Modular**: Recommended ≤150 lines per file (split if needed)
4. **Include Practical Examples**: Add real-world examples and use cases
5. **Lab Structure**: Each lab includes objective, steps, and expected outcome

### When Creating Educational Content

#### File Naming

- ✅ Use descriptive names: `concepts.md`, `pull-requests.md`, `github-actions.md`
- ✅ Domain folders use numbered prefixes: `src/01_github-basics/`, `src/02_working-with-repositories/`
- ✅ Lab files use numbered format: `lab-01-create-repo.md` (in `src/labs/`)

#### Content Structure

- ✅ Recommended ≤150 lines per file
- ✅ Split into multiple parts if content exceeds 150 lines
- ✅ Each part should be self-contained
- ✅ Include practical examples and use cases

### When Creating Labs

#### Standard Structure

Each lab should include:

- **Objective**: What the lab teaches
- **Prerequisites**: What you need before starting
- **Steps**: Detailed step-by-step instructions
- **Expected Outcome**: What you should see/achieve
- **Troubleshooting**: Common issues and solutions (optional)

### Security Best Practices

- ❌ **NEVER** commit API keys or secrets
- ✅ **ALWAYS** use environment variables or GitHub Secrets
- ✅ **ALWAYS** add sensitive files to `.gitignore`

---

## 📋 Code Quality Standards

### Markdown Files

- Use proper heading hierarchy (H1 → H2 → H3)
- Include code fence language specifications
- Follow markdownlint rules
- Use UTF-8 encoding
- Line length ~120 chars (tables/URLs may exceed)

### Code Examples

- Include GitHub CLI, Git commands, and workflow examples
- Use proper syntax highlighting
- Include comments explaining steps
- Keep examples simple and focused

---

## 🚀 Content Creation Workflow

### Learning-Focused Workflow

1. **Domain Coverage**: Ensure content covers all exam objectives for the domain
2. **Practical Examples**: Include real-world scenarios and use cases
3. **Hands-On Practice**: Create labs that reinforce concepts
4. **Cross-Reference**: Link related topics across domains
5. **Progress Tracking**: Update progress files as content is completed

### Quality Gate Questions

Before publishing any content:

1. ✅ Does this cover exam objectives for the domain?
2. ✅ Are practical examples included?
3. ✅ Is the content clear and easy to follow?
4. ✅ Does this fit naturally in the learning progression?
5. ✅ Are there hands-on exercises or labs for this topic?
6. ✅ Is this content within 150 lines for effective delivery?

---

## 📝 Local Quality Checks

Before committing changes:

### Markdown Linting

```bash
npx markdownlint-cli2 "**/*.md"
```

### Link Checking (Lychee via Docker)

```bash
docker run --rm -v "${PWD}:/input:ro" lycheeverse/lychee --config /input/lychee.toml "/input/**/*.md"
```

### Pre-Commit Checklist

- [ ] Run markdownlint and fix any issues
- [ ] Run Lychee link checker (if Docker available)
- [ ] Verify all file references point to existing files
- [ ] Check that code fences have language specifications
- [ ] Ensure proper blank lines around headings and lists
- [ ] Verify file naming follows conventions

---

## 🔗 Quick Links

- [Repository Structure](../docs/01_repository-structure.md)
- [Learning Path](../README.md)
- [Contributing](../CONTRIBUTING.md)

---

## 📞 Support

- **Issues**: Use GitHub Issues for questions or suggestions
- **Learning**: Follow the domain progression (01 → 06)
- **Labs**: Complete labs in order for best learning experience

---

## 🔄 Update Verification Protocol

**After ANY structural change, IMMEDIATELY update**:

1. ✅ **`docs/01_repository-structure.md`** - **UPDATE THIS FIRST** (Single source of truth)
2. ✅ `.github/copilot-instructions.md` - Reference to the repository structure doc (THIS FILE)
3. ✅ `README.md` - Reference to the repository structure doc
4. ✅ `.cursor/rules/02_repository-structure.mdc` - Reference to the repository structure doc
5. ✅ Relevant documentation files

**Self-Check Question**: "Did I update `docs/01_repository-structure.md` first?" - If no, STOP and do it NOW.
