---
title: "adversarial-spec - Multi-Model Specification Refinement Plugin"
type: tool
date_added: 2026-01-11
source: "https://github.com/zscole/adversarial-spec"
tags: [claude-code-plugin, specification-writing, product-development, multi-llm, llm-orchestration, consensus-building]
via: "Twitter bookmark from @0xzak"
---

adversarial-spec is a Claude Code plugin that iteratively refines product specifications (PRDs and tech specs) through multi-model debate until all LLMs reach consensus on a solid document.

## Core Insight

A single LLM reviewing a specification will miss gaps, gloss over vague requirements, and let edge cases slide. Multiple LLMs debating a spec catch what any one model would overlook. The result is a document that has survived rigorous adversarial review from multiple perspectives.

**Claude is an active participant**, not just an orchestrator. Claude provides independent critiques, challenges opponent models, and contributes substantive improvements alongside external models.

## How It Works

```
You describe product --> Claude drafts spec --> Multiple LLMs critique in parallel
        |                                              |
        |                                              v
        |                              Claude synthesizes + adds own critique
        |                                              |
        |                                              v
        |                              Revise and repeat until ALL agree
        |                                              |
        +--------------------------------------------->|
                                                       v
                                            User review period
                                                       |
                                                       v
                                            Final document output
```

1. Describe your product concept or provide an existing document
2. (Optional) Start with an in-depth interview to capture requirements
3. Claude drafts the initial document (PRD or tech spec)
4. Document is sent to opponent models (GPT, Gemini, Grok, etc.) for parallel critique
5. Claude provides independent critique alongside opponent feedback
6. Claude synthesizes all feedback and revises
7. Loop continues until ALL models AND Claude agree
8. User review period: request changes or run additional cycles
9. Final converged document is output

## Features

- **Interview Mode**: Optional deep-dive Q&A before drafting to capture requirements upfront
- **Early Agreement Checks**: If a model agrees too fast, it gets pressed to prove it actually read the doc
- **User Review Period**: After consensus, you can request changes or run another cycle
- **PRD to Tech Spec Flow**: Finish a PRD, then continue straight into a technical spec based on it
- **Telegram Integration**: Get notified on your phone, inject feedback from anywhere

## Supported Models

| Provider   | Env Var                | Example Models                               |
|------------|------------------------|----------------------------------------------|
| OpenAI     | `OPENAI_API_KEY`       | `gpt-4o`, `gpt-4-turbo`, `o1`                |
| Anthropic  | `ANTHROPIC_API_KEY`    | `claude-sonnet-4-20250514`, `claude-opus-4-20250514` |
| Google     | `GEMINI_API_KEY`       | `gemini/gemini-2.0-flash`, `gemini/gemini-pro` |
| xAI        | `XAI_API_KEY`          | `xai/grok-3`, `xai/grok-beta`                |
| Mistral    | `MISTRAL_API_KEY`      | `mistral/mistral-large`, `mistral/codestral` |
| Groq       | `GROQ_API_KEY`         | `groq/llama-3.3-70b-versatile`               |
| OpenRouter | `OPENROUTER_API_KEY`   | `openrouter/openai/gpt-4o`, `openrouter/anthropic/claude-3.5-sonnet` |
| Deepseek   | `DEEPSEEK_API_KEY`     | `deepseek/deepseek-chat`                     |

Also supports AWS Bedrock for enterprise deployments requiring all model calls to route through Bedrock.

## Benefits

- **Requirements Clarity**: Vague requirements get challenged from multiple angles
- **Error Handling Coverage**: Missing error handling gets flagged by different models
- **Security Gaps**: Security considerations surface from multiple model perspectives
- **Scope Management**: Scope creep gets caught during consensus-building process
- **Edge Case Coverage**: Multiple models asking "what about X?" ensures comprehensive coverage

## Quick Start

```bash
# 1. Add the marketplace and install the plugin
claude plugin marketplace add zscole/adversarial-spec
claude plugin install adversarial-spec

# 2. Set at least one API key
export OPENAI_API_KEY="sk-..."
# Or use OpenRouter for access to multiple providers with one key
export OPENROUTER_API_KEY="sk-or-..."

# 3. Run it
/adversarial-spec "Build a rate limiter service with Redis backend"
```

## Requirements

- Python 3.10+
- `litellm` package: `pip install litellm`
- API key for at least one LLM provider

## Use Cases

- Writing initial PRDs when requirements are unclear
- Pre-implementation tech spec creation to catch design flaws early
- Refining existing specs before team handoff
- Improving documentation quality through multi-perspective review
- Ensuring security and edge case coverage in system designs

## Links

- [GitHub Repository](https://github.com/zscole/adversarial-spec)
- [Original Tweet](https://x.com/0xzak/status/2010213382494798108)

