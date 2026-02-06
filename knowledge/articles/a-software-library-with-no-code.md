# A Software Library with No Code

**Source:** https://www.dbreunig.com/2026/01/08/a-software-library-with-no-code.html
**Author:** Drew Breunig
**Published:** January 8, 2026
**Tags:** OSS, AI, SPECS

## Summary

Drew Breunig releases `whenwords`, a multi-language relative time formatting library that contains **zero implementation code**. Instead, it distributes only specifications (SPEC.md), language-agnostic test cases (tests.yaml), and installation instructions directing users to prompt an AI agent with the specs.

## Key Insights

### The Experiment
- `whenwords` provides five functions: `timeago()`, `duration()`, `parse_duration()`, `human_date()`, `date_range()`
- Supports Ruby, Python, Rust, Elixir, Swift, PHP, and Bash (and likely others)
- Installation: Copy the simple spec prompt into Claude/Codex/Cursor, paste your language choice, and AI implements it in one shot
- Claude Opus 4.5 successfully implemented it in every tested language on first attempt

### Core Question
**"What does software engineering look like when coding is free?"**

With advanced AI coding agents crossing capability thresholds, the traditional model of language-specific library repositories may become obsolete for utility libraries. Instead, well-defined specifications + tests become the "source of truth," with implementations generated on-demand per language and project conventions.

### When This Model Works
- **Utility libraries** (not frameworks): Simple, well-defined functions
- **Clear standards:** Well-understood domains like Unix time
- **Low performance criticality:** Implementation inefficiency isn't a bottleneck
- **Manageable complexity:** Spec fits in ~500 lines or less

### When You Still Need Hardcoded Libraries

1. **Performance Matters:** Browser engines, real-time systems where optimization is critical
2. **Testing Complexity:** Multi-implementation testing becomes unwieldy; easier to maintain one reference implementation
3. **Historical Baggage:** Existing bugs, edge cases, compatibility quirks that live in code
4. **Ecosystem Integration:** Dependencies, build system integration, package manager presence
5. **Trust & Auditability:** Established track record vs. freshly generated code

## Implications for Software Development

- Well-defined specs (like those for HTML/CSS/JS) could enable spec-only tools, but practical concerns (performance, testing, real-world bugs) necessitate maintained implementations
- The threshold between "specify once, generate many" and "maintain one reference implementation" is shifting lower with better AI agents
- Simple utilities are the natural target; complex frameworks still require human engineering stewardship
- Opens questions about software licensing, attribution, and quality assurance for AI-generated implementations

## Related Concepts
- Spec-driven development
- Infrastructure as Code patterns
- Language-agnostic design
- Declarative vs. imperative programming
