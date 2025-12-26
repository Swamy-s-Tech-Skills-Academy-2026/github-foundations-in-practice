# GitHub Foundations – Learning Journey

![License](https://img.shields.io/badge/License-MIT-blue.svg)
![Status](https://img.shields.io/badge/Status-Educational-green.svg)
![GitHub Foundations](https://img.shields.io/badge/GitHub-Foundations-orange.svg)
![Maintainer](https://img.shields.io/badge/Maintainer-Viswanatha%20Swamy%20P%20K-blue)

> **⚠️ IMPORTANT: This is NOT the official GitHub Foundations syllabus. This is Swamy's personal learning journey and study materials.**

This repository documents my structured learning journey toward the **GitHub Foundations Certification**.

The goal of this repo is not only exam preparation, but also to build **practical, working knowledge of GitHub** that can be applied in real-world projects and team collaboration.

---

## 🎯 Objectives

- Understand GitHub concepts, workflows, and terminology
- Practice core GitHub features hands-on
- Build confidence for the GitHub Foundations exam
- Maintain a reusable reference for future projects

---

## 📘 Exam Domains Covered

| Domain | Coverage |
|------|---------|
| GitHub Basics | ✅ |
| Working with Repositories | ✅ |
| Collaboration | ✅ |
| GitHub Tools | ✅ |
| Security & Best Practices | ✅ |
| Open Source & Community | ✅ |

---

## 🧭 Learning Structure

Each domain contains:

- Concept explanations
- Practical examples
- Focused notes aligned to exam objectives

Hands-on labs are maintained separately under `src/labs/`.

---

## 🗂 Repository Structure Overview

> **📋 Single Source of Truth**: The complete and up-to-date repository structure is maintained in [`docs/01_repository-structure.md`](docs/01_repository-structure.md). This file should be referenced for the authoritative structure.

For the complete repository structure with all file names and details, see: **[`docs/01_repository-structure.md`](docs/01_repository-structure.md)**

---

## 📍 Milestones & Progress Tracking

Progress is tracked in detail here:

- [`src/progress/milestones.md`](src/progress/milestones.md)
- [`src/progress/study-log.md`](src/progress/study-log.md)
- [`src/progress/exam-readiness-checklist.md`](src/progress/exam-readiness-checklist.md)

### High-Level Status

| Milestone | Status |
|---------|--------|
| GitHub Basics | ⬜ Not Started |
| Working with Repositories | ⬜ Not Started |
| Collaboration | ⬜ Not Started |
| GitHub Tools | ⬜ Not Started |
| Security & Best Practices | ⬜ Not Started |
| Open Source & Community | ⬜ Not Started |
| Full Revision | ⬜ Not Started |

> **Note**: For practice questions and exam registration, please visit the [official certification page](https://learn.microsoft.com/en-us/credentials/certifications/github-foundations/?practice-assessment-type=certification) or see [`src/resources/official-links.md`](src/resources/official-links.md) for all official resources.

---

## 🧪 Hands-On Labs

- Create and manage repositories
- Raise and review pull requests
- Configure a basic GitHub Actions workflow
- Publish a site using GitHub Pages

Each lab includes:

- Objective
- Steps
- Expected outcome

---

## 📝 Notes & Exam Tips

Key takeaways, common mistakes, and exam-focused insights are maintained under `src/notes/`.

---

## 🔗 Resources

Official documentation and curated references are listed under `src/resources/`.

### Official Certification Link

For practice questions, exam registration, and official study materials, visit:

**[GitHub Foundations Certification - Microsoft Learn](https://learn.microsoft.com/en-us/credentials/certifications/github-foundations/?practice-assessment-type=certification)**

See [`src/resources/official-links.md`](src/resources/official-links.md) for complete list of official resources.

---

## 🚧 Status

This repository is **actively evolving** as I progress through the certification.

---

## 📌 Disclaimer

This is a **personal learning repository**, not official GitHub material.

---

## 🛠️ Development & Quality Assurance

### Documentation Quality Checks (Local)

Run Markdown lint against README and all documentation before opening a PR:

```bash
# From repo root - lint all markdown files
npx --yes markdownlint-cli2 "README.md" "docs/**/*.md" ".github/**/*.md"
```

This uses the repository's `.markdownlint.json` configuration automatically.

### Link Validation (Lychee)

Run link checker to validate all links in documentation:

```bash
# Validate all links (recommended; matches CI behavior)
docker run --rm -w /input -v "${PWD}:/input" lycheeverse/lychee:latest --config lychee.toml --no-progress README.md docs/**/*.md .github/**/*.md
```

### Pre-Commit Checklist

Before committing changes:

- [ ] Run markdownlint and fix any issues
- [ ] Run Lychee link checker (if Docker available)
- [ ] Verify all file references point to existing files
- [ ] Check that code fences have language specifications
- [ ] Ensure proper blank lines around headings and lists

---

## 🤝 Contributing

We welcome contributions! Whether it's:

- 🐛 Bug fixes
- 📝 Documentation improvements
- 💡 New learning content
- 🎯 Additional practice exercises
- 📚 Additional learning resources

Please see [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

## 📞 About & Get In Touch

### Swamy's Tech Skills Academy 2026

Ready to master GitHub Foundations? Let's begin your transformation! 🚀

Ready to take your GitHub skills to the next level? Join our learning community!

- 🌐 Visit our website for more courses
- 📧 Contact us for custom training programs
- 🏆 Get certified in GitHub Foundations
- 👥 Join our learning community

Happy Learning! 🎓✨

---
