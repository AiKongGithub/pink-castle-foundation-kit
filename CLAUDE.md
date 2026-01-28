# CLAUDE.md

# Pink Castle Foundation Kit - Project Guide

> **Last Updated:** 2026-01-29
> **Version:** 1.0.0
> **Project:** Pink Castle Foundation Kit

---

## 🎯 Project Overview

**What:** A complete development toolkit for AI-assisted coding
**Why:** Help beginners start development with AI tools
**How:** Templates + Structure + Automation + Best Practices

**Target Users:**
- Beginners who want to learn AI-assisted development
- Small teams setting up projects
- Developers looking for best practices

---

## 🏗️ Project Structure

This project follows the **PRP Framework** (Pink Castle Foundation):

```
project-root/
├── CLAUDE.md           ← You are here (Project Guide)
├── prds/               ← Product Requirements
├── plans/              ← Project Plans
├── reports/            ← Status Reports
├── issues/             ← Issue Tracking
├── reviews/            ← Code & Design Reviews
└── spec-kit/           ← Specification Templates
```

---

## 📁 Folders Explained

### 1. prds/ (Product Requirements)
**Purpose:** Store all product requirement documents
**When to use:** Before starting any new feature
**Format:** Markdown (.md)

**Example files:**
- `feature-auth.md` - Authentication feature PRD
- `feature-api.md` - API design PRD
- `product-roadmap.md` - Overall product roadmap

### 2. plans/ (Project Plans)
**Purpose:** Track project timelines and milestones
**When to use:** At project start and sprint planning
**Format:** Markdown (.md) or YAML (.yml)

**Example files:**
- `sprint-2026-01.md` - January sprint plan
- `timeline.yml` - Project timeline
- `dependencies.md` - External dependencies

### 3. reports/ (Status Reports)
**Purpose:** Document progress and issues
**When to use:** Weekly or milestone-based
**Format:** Markdown (.md)

**Example files:**
- `weekly-2026-w04.md` - Week 4 report
- `milestone-v1.md` - Version 1.0 milestone report
- `retrospective-jan.md` - January retrospective

### 4. issues/ (Issue Tracking)
**Purpose:** Track bugs and feature requests
**When to use:** When problems arise
**Format:** Markdown (.md) with template

**Example files:**
- `bug-001-login.md` - Login bug report
- `feature-request-002.md` - Feature request
- `tech-debt-003.md` - Technical debt item

### 5. reviews/ (Code & Design Reviews)
**Purpose:** Document review feedback
**When to use:** After major code or design changes
**Format:** Markdown (.md)

**Example files:**
- `code-review-pr-42.md` - Pull request 42 review
- `design-review-ui.md` - UI design review
- `architecture-review.md` - Architecture review

---

## 🎨 Development Workflow

### For New Features:
```
1. Write PRD → prds/feature-name.md
2. Create Plan → plans/feature-plan.md
3. Implement & Test
4. Document Issues → issues/
5. Code Review → reviews/
6. Status Report → reports/
```

### For Bug Fixes:
```
1. Document Issue → issues/bug-NNN.md
2. Fix & Test
3. Update Report → reports/weekly-YYYY-WNN.md
```

### For Reviews:
```
1. Complete work
2. Create Review Doc → reviews/type-name.md
3. Get feedback
4. Address feedback
5. Document resolution
```

---

## 🤝 Working with AI

### When starting a conversation:
1. **Reference this file:** "Read CLAUDE.md first"
2. **Point to relevant docs:** "See prds/feature-x.md"
3. **Provide context:** Link to related issues/reviews

### Best Practices:
- ✅ Keep CLAUDE.md updated
- ✅ Write clear PRDs before coding
- ✅ Document decisions in reviews/
- ✅ Track all issues in issues/
- ✅ Weekly reports in reports/

### Don't:
- ❌ Start coding without a PRD
- ❌ Skip documentation
- ❌ Forget to update CLAUDE.md
- ❌ Leave issues undocumented

---

## 📚 Reference Documents

### Core Documents:
- `spec-kit/README.md` - Specification Kit Guide
- `spec-kit/templates/` - All templates
- `prds/README.md` - How to write PRDs
- `reviews/README.md` - Review guidelines

### External Links:
- [Pink Castle Foundation](https://notion.so/Pink-Castle-2f25dcbd48ac81bd8604e66a6318e98d) - Main project
- [Project Brief](https://notion.so/2f65dcbd48ac815fb864f36f8ae4992f) - Full guide
- [Day 1 Spec](https://notion.so/2f65dcbd48ac81ebbb07f5e4da1d8279) - Specifications

---

## 🔧 Tools & Integration

### AI Tools:
- **Claude (Opus/Sonnet):** Strategy & Planning
- **Claude Code:** Implementation
- **GitHub Copilot:** Code assistance

### Project Management:
- **Notion:** Documentation hub
- **GitHub:** Version control
- **n8n:** Automation workflows

### Communication:
- **Notion Comments:** Async discussions
- **README files:** Documentation
- **CLAUDE.md:** Central reference

---

## 🚀 Quick Start

### For New Team Members:
```bash
# 1. Read this file first
cat CLAUDE.md

# 2. Check project structure
ls -la

# 3. Read README in each folder
cat prds/README.md
cat plans/README.md
cat reports/README.md
cat issues/README.md
cat reviews/README.md

# 4. Check spec kit
cat spec-kit/README.md
```

### For AI Assistants:
```
1. Read CLAUDE.md (this file)
2. Understand folder structure
3. Read relevant docs in prds/ or issues/
4. Ask questions if unclear
5. Start working
```

---

## 📝 Update Log

### Version 1.0.0 (2026-01-29)
- Initial CLAUDE.md created
- Documented 5-folder structure
- Added workflow guidelines
- Integrated with spec-kit

---

## 🆘 Need Help?

### Common Questions:

**Q: Where do I start?**
A: Read this CLAUDE.md, then check prds/ for requirements

**Q: Where do I document a bug?**
A: Create a file in issues/ using the template

**Q: How do I request a review?**
A: Create a file in reviews/ and tag reviewers

**Q: What's the difference between prds/ and plans/?**
A: prds/ = WHAT to build, plans/ = WHEN to build it

### Contact:
- **Project Lead:** สามประสาน Team
- **Documentation:** Notion workspace
- **Issues:** GitHub Issues

---

**Remember:** This CLAUDE.md is a living document. Update it as the project evolves!

---

*Generated by: Pink Castle Foundation Kit*
*Framework: PRP (PRDs, Plans, Reports, Issues, Reviews)*
*Version: 1.0.0*
