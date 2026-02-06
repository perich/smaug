# Vercel Composition Patterns

**Source:** https://skills.sh/vercel-labs/agent-skills/vercel-composition-patterns

## Overview

React composition patterns for building flexible, maintainable React components. Avoid boolean prop proliferation by using compound components, lifting state, and composing internals. These patterns make codebases easier for both humans and AI agents to work with as they scale.

## When to Apply

Reference these guidelines when:
- Refactoring components with many boolean props
- Building reusable component libraries
- Designing flexible component APIs
- Reviewing component architecture
- Working with compound components or context providers

## Rule Categories by Priority

| Priority | Category | Impact | Prefix |
|----------|----------|--------|--------|
| 1 | Component Architecture | HIGH | `architecture-` |
| 2 | State Management | MEDIUM | `state-` |
| 3 | Implementation Patterns | MEDIUM | `patterns-` |
| 4 | React 19 APIs | MEDIUM | `react19-` |

## Quick Reference

### 1. Component Architecture (HIGH)
- `architecture-avoid-boolean-props` - Don't add boolean props to customize behavior; use composition
- `architecture-compound-components` - Structure complex components with shared context

### 2. State Management (MEDIUM)
- `state-decouple-implementation` - Provider is the only place that knows how state is managed
- `state-context-interface` - Define generic interface with state, actions, meta for dependency injection
- `state-lift-state` - Move state into provider components for sibling access

### 3. Implementation Patterns (MEDIUM)
- `patterns-explicit-variants` - Create explicit variants instead of boolean prop combinations
- `patterns-slots-composition` - Use slots and composition for component flexibility
- `patterns-render-props` - Use render props for advanced composition scenarios

### 4. React 19 APIs (MEDIUM)
- `react19-use-context-directive` - Use `use` directive for accessing context in client components
- `react19-actions` - Leverage actions for form submissions and mutations

## Key Principles

1. **Avoid Boolean Props Proliferation** - Each boolean prop doubles the complexity. Use composition instead.
2. **Compound Components** - Group related components using shared context for flexible composition.
3. **State Lifting** - Move state up to providers so sibling components can access the same state.
4. **Decoupled Implementation** - Only the provider knows how state is managed, children use generic interfaces.
5. **Explicit Variants** - Create explicit component variants instead of combining boolean flags.

## Benefits

- **Scalability** - Patterns work whether you have 2 or 200 component variations
- **Maintainability** - Clearer intent and easier to understand component relationships
- **Flexibility** - Easier to add new variations without changing component APIs
- **AI-Friendly** - Makes codebases more understandable to AI agents and humans alike
