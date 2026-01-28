# [ISSUE-001] PRP-Plan Command Adaptation for Non-Code Projects

> **Type:** Enhancement / Documentation
> **Priority:** P2 (Medium)
> **Status:** Open
> **Reporter:** จูล่ง (CTO)
> **Assignee:** กุนซือสุมาอี้
> **Date Created:** 2026-01-28
> **Date Updated:** 2026-01-28

---

## Summary

The `/prp-plan` command is designed primarily for code implementation projects (TypeScript, Python, etc.). When used for non-code projects like content production pipelines, significant adaptation is required.

---

## Problem Statement

During Day 3 testing, we used `/prp-plan` for the "Content 15,300 Pieces" project. The command template assumes:

1. **Code-centric workflow** - References to TypeScript, npm, linting
2. **File-based outputs** - CREATE/UPDATE specific code files
3. **Validation via CLI** - `npx tsc`, `npm test`, etc.
4. **Git-based version control** - For code commits

For content production projects, these don't apply directly.

---

## Observed Issues

### 1. Patterns Section Not Applicable
The "Patterns to Mirror" section expects code snippets:
```typescript
// SOURCE: src/features/example/service.ts:10-15
// COPY THIS PATTERN:
export function createThing() { ... }
```

For content projects, there are no code patterns to mirror.

### 2. Validation Commands Not Applicable
The 6-level validation assumes:
- Level 1: Linting (npm run lint)
- Level 2: Unit tests
- Level 3: Full test suite

Content projects need different validation:
- Content quality review
- Format compliance
- Tracking accuracy

### 3. File Structure Assumptions
The template assumes:
```
src/features/new/
├── models.ts
├── schemas.ts
├── service.ts
└── tests/
```

Content projects have different structures:
```
outputs/
├── audio/
├── video/
├── reports/
└── tracking/
```

---

## Proposed Solutions

### Option A: Create Content-Specific Template
Create a new command `/prp-plan-content` with:
- Content-specific sections
- QC-based validation
- Platform-centric file structure
- Non-code task definitions

### Option B: Add Conditional Sections
Modify `/prp-plan` to detect project type and:
- Include/exclude sections dynamically
- Provide alternative examples
- Adapt validation levels

### Option C: Documentation + Manual Adaptation (Current)
Document how to adapt `/prp-plan` for non-code projects:
- Skip code-specific sections
- Replace with appropriate alternatives
- Provide examples for common non-code project types

---

## Current Workaround

For Content 15,300 project, we manually adapted:
1. Replaced "Patterns to Mirror" with "Templates to Use"
2. Changed validation to content-specific checks
3. Modified task structure for content workflow
4. Added QC checkpoints instead of unit tests

---

## Impact Assessment

### Who is affected?
- [ ] All users
- [x] Specific users: Teams using PRP for non-code projects
- [ ] Internal team only
- [ ] No one yet (preventive)

### Business Impact
- **Revenue:** Low
- **User Experience:** Medium - limits PRP Framework adoption
- **Operations:** Low

---

## Related Items

### Related PRDs
- `prds/content-15300-pieces.md`

### Related Plans
- `.claude/PRPs/plans/content-15300-pieces.plan.md`

---

## Discussion / Notes

**จูล่ง (2026-01-28):**
The /prp-plan command is excellent for code projects. For Pink Castle Foundation Kit which will be used by various project types (code, content, marketing, etc.), we should consider providing guidance on adaptation.

Recommend: Start with Option C (documentation), then consider Option A if demand grows.

---

## Change Log

| Date | Author | Change |
|------|--------|--------|
| 2026-01-28 | จูล่ง | Created issue during Day 3 testing |

---

*Template from Pink Castle Foundation Kit v1.0*
