---
title: "Claude Code UI/UX Enhancement Prompt"
type: article
date_added: 2026-01-05
source: "https://x.com/doodlestein/status/2007194101448573036"
author: "Jeffrey Emanuel (@doodlestein)"
tags: [claude-code, ui-ux, prompt-engineering, design, iterative-improvement]
via: "Twitter bookmark from @doodlestein"
---

A detailed prompt engineering guide for iteratively improving web application UI/UX using Claude Code and Opus 4.5. The approach emphasizes separate desktop/mobile optimization through progressive refinement with extended thinking.

## The Prompt

```
I still think there are strong opportunities to enhance the UI/UX look and feel and to make everything work better and be more intuitive, user-friendly, visually appealing, polished, slick, and world class in terms of following UI/UX best practices like those used by Stripe, don't you agree? And I want you to carefully consider desktop UI/UX and mobile UI/UX separately while doing this and hyper-optimize for both separately to play to the specifics of each modality. I'm looking for true world-class visual appeal, polish, slickness, etc. that makes people gasp at how stunning and perfect it is in every way. Use ultrathink.
```

## Key Principles

1. **Frame as Agreement** - Phrasing that asks for model agreement motivates better polish
2. **Separate Modalities** - Consider desktop vs mobile UI/UX separately for optimal results
3. **Iterative Refinement** - Run many passes (10+ iterations typical) to accumulate improvements
4. **Incremental Changes** - Each pass makes small improvements that compound over time
5. **Extended Thinking** - Use `ultrathink` for deeper analysis and better outcomes

## Best Practices

- **Use Case Specificity** - This prompt works best when your site/app already functions well and looks decent
- **Target State** - Optimize for "world-class visual appeal, polish, slickness" inspired by companies like Stripe
- **Multiple Agents** - Can run with multiple agents simultaneously for faster iteration
- **Stream Deck Automation** - Author uses this frequently enough to have created a Stream Deck button

## Works With

- NextJS 16
- React 19
- Tailwind 4
- Framer Motion
- Other modern web frameworks and libraries (generic approach)

## When to Use vs When Not To

**Use This Prompt When:**
- Your app already works and looks decent
- You want incremental improvements to UI/UX quality
- You're optimizing for visual appeal and polish

**Use Different Prompt When:**
- Your app looks bad and needs complete overhaul
- You're starting from a poor visual foundation

## Results

The iterative approach of running multiple passes yields compounding improvements:
- Pass 1: Minor improvements
- Pass 2-3: Noticeable refinements
- Pass 5-10: Significant visual and UX enhancements
- Pass 10+: Approaching world-class quality

## Tools & Models

- **Primary:** Claude Code with Opus 4.5
- **Extended Thinking:** Enables deeper analysis per iteration
- **Framework Agnostic:** Generic enough to work with most modern web stacks

## Author Notes

Jeffrey Emanuel uses this prompt frequently enough that it appears as a button on his Stream Deck workflow automation. The approach is particularly effective for progressive enhancement when combined with Claude Code's iterative capabilities.

## Links

- [Original Tweet](https://x.com/doodlestein/status/2007194101448573036)
- [Author: Jeffrey Emanuel](https://x.com/doodlestein)
