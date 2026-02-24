---
title: "Prompt Repetition Improves Non-Reasoning LLMs"
type: article
date_added: 2026-02-17
source: "https://arxiv.org/pdf/2512.14982"
author: "Yaniv Leviathan, Matan Kalman, Yossi Matias"
tags: [llm, prompt-engineering, language-models, efficiency]
via: "Twitter bookmark from @burkov"
---

This research paper demonstrates a simple yet effective technique for improving LLM accuracy without additional computational cost. By repeating the entire prompt input twice in sequence, models gain the ability to attend bidirectionally to all input tokens on the second pass.

## Key Takeaways

- Prompt repetition improves accuracy across seven different benchmarks and multiple model families (Gemini, ChatGPT, Claude, DeepSeek)
- No increase in output token count or meaningful latency increase due to parallel hardware processing
- Accuracy improvements vary from modest to dramatic (one task improved from 21% to 97%)
- No new losses, finetuning, or complex prompt engineering required
- Addresses fundamental asymmetry in left-to-right token processing architecture
- Particularly effective for tasks involving searching, filtering, and precise information retrieval

## Links

- [Article](https://arxiv.org/pdf/2512.14982)
- [Original Tweet](https://x.com/burkov/status/2023822767284490263)
