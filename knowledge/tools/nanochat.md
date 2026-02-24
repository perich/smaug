---
title: "nanochat - Simple LLM Training Harness"
type: tool
date_added: 2026-02-11
source: "https://github.com/karpathy/nanochat"
tags: ["LLM", "Machine Learning", "Training", "PyTorch", "AI", "Open Source"]
via: "Twitter bookmark from @karpathy"
---

nanochat is the simplest experimental harness for training large language models (LLMs). It is designed to run on a single GPU node with minimal, hackable code that covers all major LLM stages: tokenization, pretraining, finetuning, evaluation, inference, and a chat UI.

The project demonstrates remarkable efficiency - you can train your own GPT-2 capability LLM for only $72 (~3 hours on an 8XH100 GPU node), compared to ~$43,000 in 2019. On spot instances, the total cost can be as low as ~$20. The entire pipeline is contained in a single shell script that handles training and deployment.

nanochat is configured out of the box with a "complexity dial" via the `--depth` parameter (number of transformer layers). All other hyperparameters (width, heads, learning rate, training duration, weight decay, etc.) are calculated automatically in an optimal way. This compute-optimal approach allows training a full miniseries of models by adjusting just one parameter.

## Key Features

- Single GPU node deployment with hackable, minimal code
- Complete pipeline: tokenization, pretraining, finetuning, evaluation, inference, chat UI
- Compute-optimal training through automatic hyperparameter calculation
- Configurable via single `--depth` parameter for transformer layers
- ChatGPT-like web interface for interacting with trained models
- Time-to-GPT-2 leaderboard tracking training efficiency improvements
- Supports mixed precision training (fp8) for faster training
- Works on Ampere (A100) and Hopper (H100) GPU architectures

## Links

- [GitHub](https://github.com/karpathy/nanochat)
- [Original Tweet](https://x.com/karpathy/status/2021633574089416993)
- [DeepWiki Documentation](https://deepwiki.com/karpathy/nanochat)
