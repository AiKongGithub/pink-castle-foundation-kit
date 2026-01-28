# Reviews (Code & Design Reviews)

This folder contains feedback from code reviews, design reviews, and architecture reviews.

## Purpose

Reviews ensure **QUALITY** and **ALIGNMENT**. They catch issues early and share knowledge.

## When to Create a Review

- ✅ Pull request submitted
- ✅ Design completed
- ✅ Architecture proposed
- ✅ Major refactoring planned

## Review Templates

### Code Review

```markdown
# Code Review: [PR Title or Feature]

**PR Number:** #NNN
**Author:** Name
**Reviewer:** Name
**Date:** YYYY-MM-DD
**Status:** Approved/Changes Requested/Rejected

## Summary
Brief overview of what's being reviewed.

## Strengths ✅
- Good test coverage
- Clear variable names
- Well-documented functions

## Issues to Address 🔴

### Critical
1. Security issue in line X
2. Performance concern in function Y

### Major
1. Missing error handling in Z
2. Unclear logic in A

### Minor
1. Typo in comment
2. Could simplify this code

## Suggestions 💡
1. Consider using pattern X instead
2. Could extract this into a helper function
3. Might want to add integration test

## Questions ❓
1. Why did you choose approach X over Y?
2. Have you considered edge case Z?

## Testing
- [ ] Unit tests pass
- [ ] Integration tests pass
- [ ] Manual testing done
- [ ] Edge cases covered

## Decision
**Approved ✅** / **Changes Requested 🔄** / **Rejected ❌**

## Next Steps
- Author addresses issues
- Re-review after changes
- Merge when approved
```

### Design Review

```markdown
# Design Review: [Feature or Component]

**Designer:** Name
**Reviewer:** Name
**Date:** YYYY-MM-DD
**Status:** Approved/Needs Revision

## What's Being Reviewed
Brief description and links to designs.

## Evaluation Criteria

### User Experience ⭐⭐⭐⭐⭐
- Clear user flow
- Intuitive interface
- Accessible design

### Visual Design ⭐⭐⭐⭐⬜
- On-brand styling
- Consistent with design system
- Good use of whitespace

### Technical Feasibility ⭐⭐⭐⭐⭐
- Can be implemented
- Performance considerations
- Browser compatibility

## Feedback

### Positive
1. Love the clean layout
2. Great use of color
3. Clear call-to-actions

### Concerns
1. Button too small on mobile
2. Contrast issue with text
3. Animation might be too slow

### Questions
1. How does this work on tablet?
2. What happens when text is long?
3. Accessibility for screen readers?

## Recommendations
1. Increase button size to 44px minimum
2. Use darker text color (AAA contrast)
3. Speed up animation to 200ms

## Decision
**Approved ✅** / **Needs Revision 🔄**

## Next Steps
- Designer updates based on feedback
- Development can start / wait for revision
```

## Best Practices

1. **Be constructive** - Suggest solutions, not just problems
2. **Be specific** - Reference line numbers or elements
3. **Be timely** - Review within 24-48 hours
4. **Ask questions** - Understand before criticizing
5. **Appreciate good work** - Positive feedback matters

---

*For questions, see CLAUDE.md or ask the team.*
