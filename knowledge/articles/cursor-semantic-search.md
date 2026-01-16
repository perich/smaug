# Semantic Search in Large Codebases

## Overview
Cursor's analysis of semantic (vector) search superiority over traditional grep-based search for navigating large, complex codebases.

## Key Findings
- **Problem with grep:** Traditional grep fails to find related concepts in large codebases, especially with company-specific jargon
- **Example failure:** Searching for "utility that predicts the next prompt" would grep for `predict`, `next`, `prompt`, `utility` but miss "Suggestion Service" where `next` matched millions of irrelevant lines
- **Solution:** Semantic search understands conceptual relationships and finds the correct tool regardless of naming conventions
- **Validation:** A/B testing confirmed semantic search's advantage over traditional approaches

## Use Cases
- Navigating large corporate codebases with specialized terminology
- Finding related code concepts when exact naming is unknown
- Improving code discovery in multi-module systems

## Links
- **Article:** https://cursor.com/blog/semsearch
- **Reference:** https://x.com/jediahkatz/status/2009343675399131334

## Related Topics
- [[code-search]]
- [[large-codebases]]
- [[semantic-analysis]]
