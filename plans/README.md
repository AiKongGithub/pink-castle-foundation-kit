# Plans (Project Plans & Timelines)

This folder contains project plans, timelines, and sprint schedules.

## Purpose

Plans define **WHEN** we're building things. They track milestones and dependencies.

## When to Create a Plan

- ✅ Starting a project
- ✅ Beginning a sprint
- ✅ Major milestone planning
- ✅ Resource allocation

## Plan Template

```markdown
# [Project/Sprint Name] Plan

## Timeline
**Start:** YYYY-MM-DD
**End:** YYYY-MM-DD
**Duration:** N weeks

## Milestones

| Milestone | Date | Status | Owner |
|-----------|------|--------|-------|
| M1: Kick-off | YYYY-MM-DD | ✅ Done | Team |
| M2: Feature complete | YYYY-MM-DD | 🟡 In Progress | Dev |
| M3: Testing done | YYYY-MM-DD | ⬜ Not Started | QA |
| M4: Launch | YYYY-MM-DD | ⬜ Not Started | All |

## Tasks

### Week 1
- [ ] Task 1 (Owner: X)
- [ ] Task 2 (Owner: Y)

### Week 2
- [ ] Task 3 (Owner: X)
- [ ] Task 4 (Owner: Z)

## Dependencies
- **External:** API from Team B (ETA: YYYY-MM-DD)
- **Internal:** Design assets (Owner: Designer)

## Risks

| Risk | Impact | Mitigation |
|------|--------|------------|
| API delay | High | Build mock first |
| Resource shortage | Medium | Adjust scope |

## Resources
- **Team:** 3 developers, 1 designer, 1 QA
- **Budget:** $XXX
- **Tools:** GitHub, Notion, n8n
```

## Examples

See `spec-kit/templates/plan-template.md` for full template.

## Best Practices

1. **Be realistic** - Buffer time for unknowns
2. **Track dependencies** - Don't block others
3. **Update regularly** - Keep status current
4. **Visualize timeline** - Use Gantt charts if helpful
5. **Review retrospectively** - Learn for next time

---

*For questions, see CLAUDE.md or ask the team.*
