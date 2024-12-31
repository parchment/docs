# Minor Version {X.Y} {Name of the minor version}

{Deliverable for the minor version}

## {X.Y.1} - {Feature Name}

**Deliverable**: {Single sentence describing specific, testable, user-visible outcome}

**Explanation**: {2-3 sentences explaining the deliverable in simple terms, its purpose, and its value to users}

**Tasks**:
- {Action one written in imperative}
- {Action two written in imperative}
- {Action three written in imperative}
- {Action four written in imperative}
- {Action five if needed}

**Tests**: 
- {Benchmark requirement with specific time/size constraint}
- {Validation requirement with clear pass/fail}
- {Integration requirement with measurable outcome}
- {Performance requirement if applicable}

Commit: `{type}: {imperative message}`

Changeset:
```markdown
---
"{package-scope}": patch
"{additional-package}": patch
---

{type}: {imperative message}

- {Change one matching commit scope}
- {Change two matching commit scope}
- {Change three matching commit scope}
- {Change four matching commit scope}
- {Change five if needed}
```

Notes:
- Each patch should focus on a single, atomic deliverable
- Tasks should be focused but not contain implementation details
- Tests should have clear, measurable success criteria
- Patches should build logically toward minor version goals
- Add a conventional commit after each patch (no scope needed)
- Add a changeset document after each patch