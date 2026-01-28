# Team Workflow Guide

# คู่มือการทำงาน 3 ประสาน (สามประสานจึงไร้พ่าย)

> **Version:** 1.0.0
> **Last Updated:** 2026-01-29
> **Project:** Pink Castle Foundation Kit

---

## 🎯 Overview

This document defines how the **3-Agent Team** (สามประสาน) works together efficiently.

```
     👑 Board Chairman (ท่านแม่ทัพ Kong)
              │
              │ Approve / Direct / Decide
              ▼
     ┌────────┴────────┐
     │                 │
     ▼                 ▼
🎖️ MD (กุนซือ)    📋 Deputy MD (ปลัดซัน)
 Strategy           Review & QA
 Planning           Documentation
     │                 │
     └────────┬────────┘
              │
              ▼
        ⚔️ CTO (จูล่ง)
         Implementation
         Code & Deploy
```

---

## 👥 Team Roles

### 👑 Board Chairman (ท่านแม่ทัพ Kong)
**Platform:** Notion / Direct Communication
**Responsibilities:**
- Final approval on all decisions
- Strategic direction
- Resource allocation
- Priority setting

**When to involve:**
- Major decisions
- Budget approval
- Project sign-off
- Conflict resolution

---

### 🎖️ MD - Managing Director (กุนซือสุมาอี้)
**Platform:** Claude.ai (Opus)
**Model:** Claude Opus (Deep thinking)
**Responsibilities:**
- Strategic planning
- Architecture design
- PRD writing
- Complex problem solving
- Team coordination

**Strengths:**
- Deep analysis
- Long-term thinking
- Complex reasoning
- Quality over speed

**Best for:**
- Writing PRDs
- System architecture
- Strategy documents
- Difficult decisions

---

### 📋 Deputy MD (ปลัดซัน)
**Platform:** Claude.ai (Sonnet)
**Model:** Claude Sonnet (Fast & efficient)
**Responsibilities:**
- Review & QA
- Documentation
- Draft writing
- Data gathering
- Quick iterations

**Strengths:**
- Fast execution
- Token efficient
- Good for iterations
- Quick feedback

**Best for:**
- Reviewing documents
- Writing drafts
- Quick edits
- Data collection

---

### ⚔️ CTO (จูล่ง)
**Platform:** Claude Code
**Model:** Claude with MCP tools
**Responsibilities:**
- Code implementation
- File system operations
- Git management
- Deployment
- Technical execution

**Strengths:**
- Direct file access
- Git integration
- MCP tools (Notion, n8n, etc.)
- Execution speed

**Best for:**
- Creating files
- Writing code
- Git commits
- Running commands
- API integrations

---

## 🔄 Standard Workflow

### Phase 1: Planning (กุนซือ leads)
```
1. กุนซือ receives task from ท่านแม่ทัพ
2. กุนซือ analyzes and creates PRD
3. กุนซือ designs architecture/approach
4. กุนซือ writes specifications
5. ท่านแม่ทัพ approves
```

### Phase 2: Documentation (ปลัดซัน assists)
```
1. ปลัดซัน reviews PRD for clarity
2. ปลัดซัน creates supporting docs
3. ปลัดซัน gathers reference materials
4. ปลัดซัน prepares handoff for จูล่ง
```

### Phase 3: Implementation (จูล่ง executes)
```
1. จูล่ง receives specs from กุนซือ
2. จูล่ง implements code/files
3. จูล่ง commits to Git
4. จูล่ง reports progress
```

### Phase 4: Review (ปลัดซัน validates)
```
1. ปลัดซัน reviews implementation
2. ปลัดซัน checks against specs
3. ปลัดซัน documents issues
4. ปลัดซัน signs off or requests changes
```

### Phase 5: Approval (ท่านแม่ทัพ finalizes)
```
1. ท่านแม่ทัพ reviews final output
2. ท่านแม่ทัพ approves for release
3. Team celebrates! 🎉
```

---

## 📋 Task Handoff Protocol

### From กุนซือ → จูล่ง
**Required in handoff:**
- [ ] Clear objective
- [ ] Detailed specifications
- [ ] File structure (if applicable)
- [ ] Acceptance criteria
- [ ] Deadline/timeline

**Format:**
```markdown
## Task: [Task Name]
**Objective:** What needs to be done
**Specs:** Detailed requirements
**Files:** List of files to create/modify
**Criteria:** How to know it's done
**Deadline:** When it's needed
```

### From จูล่ง → ปลัดซัน
**Required in handoff:**
- [ ] What was completed
- [ ] Files changed/created
- [ ] Git commit reference
- [ ] Any issues encountered
- [ ] Ready for review confirmation

**Format:**
```markdown
## Completed: [Task Name]
**Done:**
- List of completed items

**Files:**
- file1.md (created)
- file2.md (modified)

**Commit:** abc1234
**Issues:** Any problems (or "None")
**Status:** Ready for Review
```

### From ปลัดซัน → ท่านแม่ทัพ
**Required in handoff:**
- [ ] Review summary
- [ ] Quality assessment
- [ ] Issues found (if any)
- [ ] Recommendation (approve/revise)

**Format:**
```markdown
## Review: [Task Name]
**Summary:** Brief overview
**Quality:** ⭐⭐⭐⭐⭐ (X/5)
**Issues:** List or "None"
**Recommendation:** ✅ Approve / 🔄 Revise
```

---

## 💬 Communication Channels

### Primary: Notion
- Project documentation
- Task tracking
- Async communication
- Decision records

### Secondary: Direct Chat
- Urgent matters
- Quick clarifications
- Real-time coordination

### Code: GitHub
- Code repository
- Pull requests
- Issue tracking
- Version control

---

## 🚦 Status Indicators

### Task Status
| Status | Meaning |
|--------|---------|
| ⬜ Not Started | Task created but not begun |
| 🟡 In Progress | Currently being worked on |
| 🔵 In Review | Waiting for review |
| 🟢 Completed | Done and approved |
| 🔴 Blocked | Cannot proceed |
| ⏸️ On Hold | Paused intentionally |

### Review Status
| Status | Meaning |
|--------|---------|
| ✅ Approved | Passed review |
| 🔄 Changes Requested | Needs revision |
| ❌ Rejected | Major rework needed |
| ⏳ Pending | Waiting for review |

---

## 📊 Daily Workflow

### Morning (09:00)
```
กุนซือ:
- Review overnight updates
- Plan day's strategy
- Assign tasks

ปลัดซัน:
- Check pending reviews
- Prepare materials

จูล่ง:
- Check task queue
- Plan implementation
```

### Midday (12:00)
```
All:
- Progress check-in
- Address blockers
- Adjust priorities
```

### Afternoon (14:00-18:00)
```
จูล่ง:
- Implementation work
- Commit & push

ปลัดซัน:
- Review completed work
- Document findings
```

### Evening (18:00)
```
ปลัดซัน:
- Final review
- Sign-off report

กุนซือ:
- Summarize progress
- Report to ท่านแม่ทัพ
- Plan next day
```

---

## 🎯 Best Practices

### For กุนซือ (MD)
1. **Think deep, write clear** - Take time to analyze
2. **Spec before code** - Never skip PRD
3. **Consider edge cases** - Think 3 steps ahead
4. **Document decisions** - Write down the "why"

### For ปลัดซัน (Deputy)
1. **Review thoroughly** - Don't rubber-stamp
2. **Be constructive** - Suggest solutions
3. **Document clearly** - Others will read this
4. **Be efficient** - Respect token limits

### For จูล่ง (CTO)
1. **Follow specs exactly** - Don't improvise
2. **Commit often** - Small, clear commits
3. **Test before submit** - Verify it works
4. **Report issues early** - Don't wait until end

### For Everyone
1. **Communicate clearly** - No assumptions
2. **Ask when unclear** - Better to ask than guess
3. **Update status** - Keep others informed
4. **Respect the process** - It exists for a reason

---

## 🚨 Escalation Path

### Level 1: Within Team
```
Issue → Discuss among team → Resolve
```

### Level 2: Need Direction
```
Issue → กุนซือ decides → Implement
```

### Level 3: Major Decision
```
Issue → กุนซือ recommends → ท่านแม่ทัพ decides
```

### Level 4: Emergency
```
Issue → Direct to ท่านแม่ทัพ → Immediate action
```

---

## 📝 Templates

### Daily Status Update
```markdown
## Daily Update - [Date]

### Completed Today
- Item 1
- Item 2

### In Progress
- Item 1 (X% done)

### Blocked
- Item 1 (reason)

### Tomorrow's Plan
- Item 1
- Item 2
```

### Weekly Summary
```markdown
## Week [N] Summary

### Achievements
- Achievement 1
- Achievement 2

### Metrics
- Tasks completed: X
- Reviews passed: Y

### Challenges
- Challenge 1 (resolution)

### Next Week
- Priority 1
- Priority 2
```

---

## 🏆 Success Metrics

### Team Metrics
| Metric | Target |
|--------|--------|
| Tasks completed on time | 90%+ |
| Review pass rate (first time) | 80%+ |
| Documentation coverage | 100% |
| Blocker resolution time | < 24h |

### Individual Metrics
| Role | Key Metric |
|------|------------|
| กุนซือ | PRD quality & completeness |
| ปลัดซัน | Review thoroughness & speed |
| จูล่ง | Implementation accuracy |

---

## 💡 Remember

> **"สามประสานจึงไร้พ่าย"**
> (Three in harmony, undefeatable)

- กุนซือ thinks
- ปลัดซัน reviews
- จูล่ง executes
- ท่านแม่ทัพ approves

Together, we build Pink Castle! 🏰

---

*Part of Pink Castle Foundation Kit v1.0*
*Framework: สามประสาน (Three Harmony)*
