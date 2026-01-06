---
title: "ACIP - Advanced Cognitive Inoculation Prompt"
type: tool
date_added: 2026-01-05
source: "https://github.com/Dicklesworthstone/acip"
tags: [ai-security, prompt-injection, llm-safety, defense, prompt-engineering]
via: "Twitter bookmark from @doodlestein"
---

ACIP (Advanced Cognitive Inoculation Prompt) is a security framework designed by Jeffrey Emanuel to fortify Large Language Models against sophisticated prompt injection attacks. It works by "inoculating" LLMs through detailed explanatory guidance and explicit examples of malicious prompt strategies, similar to how cognitive/psychological inoculation works for humans.

Rather than attempting to build security into the model itself (which research shows is difficult), ACIP takes a pragmatic approach: protecting sensitive LLM deployments through careful prompting and behavioral guidance.

## How It Works

ACIP combines:
- **Cognitive Integrity Framework**: A foundational security directive set that the model follows
- **Categorized Examples**: Real-world injection examples organized by attack type
- **Semantic Isolation**: Techniques to help models recognize nuanced manipulation attempts
- **Transparent Rejection**: Standardized alert responses when malicious prompts are detected

## Key Concepts

### The Inoculation Analogy
Just as vaccines expose immune systems to weakened pathogens to build resistance, ACIP exposes LLMs to examples of injection attacks to help them recognize and resist similar real attacks.

### Pragmatic Security
Acknowledges that no solution offers perfect protection, but ACIP significantly reduces attack surface and casual intrusion attempts—like locking your front door even though someone could pick it.

## Versions

- **v1.0**: Original release
- **v1.2**: RAG/tool hardening, reduced oracle leakage
- **v1.3** (Recommended): Audit mode, balanced domain rubrics, refined framing

## Deployment Methods

1. **Direct Inclusion**: Prepend ACIP to every prompt (simpler, higher token cost)
2. **Checker Model Integration**: Use ACIP with a dedicated fast "checker model" to screen prompts before reaching primary model
3. **Hybrid Approach (v1.3+)**: Use ACIP with audit mode enabled for operator visibility without exposing refusals to attackers

## Use Cases

- Protecting personal AI assistants (Clawdbot, etc.) with access to email, messaging, file systems
- Defending agent-based systems against sophisticated social engineering
- Securing multi-tool orchestration systems where attackers could cause significant damage
- Reducing risk when LLMs control infrastructure or sensitive operations

## Limitations

- Does not offer perfect protection against sophisticated novel attacks
- Increases token usage and latency
- Effectiveness may diminish as attackers evolve techniques
- Most robust defense requires external monitoring (separate "audit model")

## Current Status (2026)

ACIP's importance has increased significantly with the rise of personal assistant projects like Clawdbot that voluntarily hook LLMs into highly sensitive areas of users' digital lives (emails, messaging, file systems). The potential for damage from a compromised agent is substantial, making ACIP increasingly relevant.

## Integration Example

With Clawdbot:
```bash
# One-liner to set up ACIP protection with Clawdbot
curl ... | bash
```

The setup uses more tokens and slightly increases latency but provides meaningful protection against prompt injection attacks.

## Links

- [GitHub Repository](https://github.com/Dicklesworthstone/acip)
- [Original Tweet Thread](https://x.com/doodlestein/status/2007996215892336924)
- [Related AI Alignment Article by Jeffrey Emanuel](https://github.com/Dicklesworthstone/some_thoughts_on_ai_alignment)
