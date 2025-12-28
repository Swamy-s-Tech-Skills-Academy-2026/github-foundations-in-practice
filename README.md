# GitHub Foundations – Learning Journey

[![License](https://img.shields.io/badge/License-MIT-purple)](LICENSE)
[![Status](https://img.shields.io/badge/Status-Active-success)](https://github.com/Swamy-s-Tech-Skills-Academy-2026/github-foundations-in-practice)
[![GitHub Foundations](https://img.shields.io/badge/GitHub-Foundations-orange)](https://learn.microsoft.com/en-us/credentials/certifications/github-foundations/)
![Format](https://img.shields.io/badge/Format-30%20Minutes-yellow)
![Built with](https://img.shields.io/badge/Built%20with-AWS%20Bedrock-brown)
[![Maintainer](https://img.shields.io/badge/Maintainer-Viswanatha%20Swamy%20P%20K-blue)](https://github.com/Swamy-s-Tech-Skills-Academy-2026)

**Repository**: [github-foundations-in-practice](https://github.com/Swamy-s-Tech-Skills-Academy-2026/github-foundations-in-practice)

> **⚠️ IMPORTANT: This is NOT the official GitHub Foundations syllabus. This is Swamy's personal learning journey and study materials.**

This repository documents my structured learning journey toward the **GitHub Foundations Certification**.

The goal of this repo is not only exam preparation, but also to build **practical, working knowledge of GitHub** that can be applied in real-world projects and team collaboration.

---

## 📌 Disclaimer

This is **Swamy's personal learning** repository and reference workspace, not official course material or a packaged curriculum.

---

## 📑 Table of Contents

- [Disclaimer](#-disclaimer)
- [Objectives](#-objectives)
- [Exam Domains Covered](#-exam-domains-covered)
- [Learning Structure](#-learning-structure)
- [Repository Structure Overview](#-repository-structure-overview)
- [Milestones & Progress Tracking](#-milestones--progress-tracking)
- [Hands-On Labs](#-hands-on-labs)
- [Notes & Exam Tips](#-notes--exam-tips)
- [Resources](#-resources)
- [Status](#-status)
- [Development & Quality Assurance](#️-development--quality-assurance)
- [Contributing](#-contributing)
- [About & Community](#-about--community)
- [License](#-license)

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

Contributions are welcome and encouraged. You may contribute in the following ways:

- Bug fixes and corrections
- Documentation improvements
- New learning content or explanations
- Additional case studies, examples, or diagrams
- Curated learning resources
- Tooling, scripts, or automation enhancements

Please review [CONTRIBUTING.md](CONTRIBUTING.md) for detailed contribution guidelines.

---

## 📞 About & Community

### [Swamy's Tech Skills Academy](https://www.linkedin.com/company/swamy-s-tech-skills-academy) & [ShyvnTech](https://www.linkedin.com/company/shyvntech)

This repository is stewarded and supported by **Swamy's Tech Skills Academy** and **ShyvnTech**. It is focused on helping developers and engineers master GitHub fundamentals through structured learning and hands-on practice.

You can connect with the community to:

- Follow structured learning journeys and deep-dive content
- Participate in knowledge-sharing discussions
- Explore mentoring, workshops, and custom training opportunities
- Get certified in GitHub Foundations

---

## 📜 License

This project is licensed under the [MIT License](LICENSE). See the [LICENSE](LICENSE) file for details.

---

> 🎓 **GitHub Foundations Learning Journey** — Designed and maintained by `Viswanatha Swamy P K`
> Empowering developers to master GitHub and excel in collaborative software development.
> © 2025 Swamy's Tech Skills Academy, ShyvnTech & Srivari Software Solutions
