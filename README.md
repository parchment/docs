# Template Usage Guide

This guide explains how to effectively use the project documentation templates to maintain consistent, high-quality project documentation across NextJS TypeScript projects deployed on Vercel.

## Template Overview

The documentation system consists of three interlocking templates:

- `README_template.md`: Project-level documentation focused on capabilities and architecture
- `ROADMAP_template.md`: Version-planned feature and capability development
- `PATCH_template.md`: Granular development steps within minor versions

## Core Philosophy

These templates enforce a structured approach to project documentation where:

1. The README describes WHAT the project does and WHY it matters
2. The ROADMAP describes WHEN features will be delivered
3. The PATCH notes describe HOW changes are implemented

## Using README_template.md

The README template creates a comprehensive project overview focusing on value proposition and architecture. When filling it out:

1. Start with the one-sentence description - this forces clarity about the project's purpose
2. Write the Overview section next - expand the core concept into concrete use cases
3. Design Principles should be immutable rules the system guarantees, not aspirational goals
4. Keep Components focused on distinct responsibilities with clear boundaries
5. Features should be concrete and specific, not abstract capabilities
6. Applications should demonstrate real-world usage scenarios

Common pitfalls to avoid:
- Mixing implementation details with architectural concepts
- Listing features without explaining their value
- Creating principles that cannot be technically enforced

## Using ROADMAP_template.md

The ROADMAP template creates a staged development plan. For effective use:

1. Version 0.1.0 should contain only critical path features needed for basic operation
2. Each minor version should deliver a cohesive set of related capabilities
3. Tests & Benchmarks must be specific and measurable
4. Resource limits should be based on production requirements
5. Security features should be explicit and verifiable

Tips for version planning:
- Group related features into minor versions
- Keep dependencies between versions minimal
- Include concrete performance targets
- Plan for security from the start

## Using PATCH_template.md

PATCH templates track granular changes within minor versions. For best results:

1. Each patch should focus on a single, atomic change
2. Deliverables must be specific and testable
3. Tasks should be actionable but not implementation-specific
4. Tests must have clear pass/fail criteria
5. Follow conventional commit format strictly

Best practices:
- Keep patches small and focused
- Write clear commit messages
- Update changelogs consistently
- Link patches to issues when relevant

## Directory Structure

Maintain a flat directory structure:

```
project/
├── README.md
├── ROADMAP.md
├── docs/
│   ├── minor01/
│   │   ├── patch01.md
│   │   └── patch02.md
│   └── minor02/
│       ├── patch01.md
│       └── patch02.md
└── components/
    └── README.md
```

## Version Control Integration

1. Use conventional commits consistently
2. Keep changesets atomic and focused
3. Link commits to patches explicitly
4. Track patch status in minor version files

## Template Maintenance

1. Review templates quarterly for relevance
2. Update templates based on project needs
3. Keep language consistent across documents
4. Remove unused sections rather than leaving them empty

## Common Antipatterns

Avoid these documentation mistakes:

1. Mixing architectural and implementation details
2. Writing vague or unmeasurable requirements
3. Creating dependencies between patches
4. Skipping changelog updates
5. Using inconsistent terminology

## NextJS/Vercel Specific Considerations

1. Document deployment constraints clearly
2. Specify Vercel-specific configuration
3. Note NextAuth integration requirements
4. Include Tanstack library versions
5. Document PSQL schema changes carefully

Remember: These templates are guides, not constraints. Adapt them to serve your project's needs while maintaining their core purpose of clear, consistent documentation.
