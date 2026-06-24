---
name: safe
description: "Conservative, non-breaking changes. Prioritize stability and backward compatibility. Use for production-safe updates with minimal risk."
user-invocable: true
---

# /safe - Safe & Conservative Changes

Make changes with minimal risk of breaking existing functionality.

## Quick Reference

- **No breaking changes**: Maintain compatibility
- **Isolated scope**: Change one thing
- **Test thoroughly**: Verify no side effects
- **Small PRs**: Easier to review and revert
- **Document clearly**: Explain the why

## When to Use

- Production deployments
- Dependency updates
- Refactoring
- Critical systems
- Stability-critical areas

## Safe Examples

- Documentation updates
- Comment improvements
- Type safety improvements
- Constants extraction
- Config tweaks with fallbacks
- Unused import cleanup

## Avoid

- Major version bumps
- API changes
- Component prop reorganization
- Architecture changes
- Global state restructuring
- Large refactors

## Common Tasks

```
/safe update dependencies
/safe clean up unused imports
/safe improve typescript types
/safe extract constants
/safe add safety comments
```
