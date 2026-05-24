# Faraazuddin Mohammed

I build open-source tools for token economics: measuring LLM cost accurately, reducing prompt waste deterministically, and routing work to the cheapest model that is still good enough.

The through-line is simple: model choice should be an engineering decision with evidence, not a default dropdown.

## Token Economics Stack

| Project | What it does | Role in the stack |
|---|---|---|
| [`tokenometer`](https://github.com/faraa2m/tokenometer) | Multi-provider token counts, USD cost, latency benchmarks, CI cost guardrails, VS Code/Cursor extension, and Claude Code skill. Live at [tokenometer.dev](https://tokenometer.dev). | Measure |
| [`llm-tokens-atlas`](https://github.com/faraa2m/llm-tokens-atlas) | Open benchmark for offline-vs-empirical tokenizer calibration across providers and prompt formats. Dataset on [Hugging Face](https://huggingface.co/datasets/faraa2m/llm-tokens-atlas). | Calibrate |
| [`promptc`](https://github.com/faraa2m/promptc) | Deterministic, LM-free prompt compiler with behavior-preserving cost-reduction passes. | Reduce |
| [`routerlab`](https://github.com/faraa2m/routerlab) | Cost-quality routing for LLM APIs with reproducible Pareto frontiers per task class. | Route |
| [`ast-ai-model-router`](https://github.com/faraa2m/ast-ai-model-router) | AST-aware Claude/Codex wrapper that picks models from task and code complexity signals. | Apply routing to coding agents |

## Start Here

- Use **Tokenometer** if you need a practical tool today: CLI, CI guardrail,
  GitHub Action, VS Code/Cursor extension, MCP server, and React components.
- Use **llm-tokens-atlas** if you need reproducible evidence about how far
  offline tokenizers drift from provider-empirical counts.
- Use **PromptC** if you want deterministic, LM-free prompt optimization with
  explicit pass semantics instead of opaque prompt rewriting.
- Use **RouterLab** if you want to make model choice a cost-quality frontier
  decision rather than a default model setting.
- Use **AST AI Model Router** if you want that routing idea applied to local
  Claude Code / Codex workflows.

## Current Focus

- Publishing empirical tokenizer calibration results that show where offline
  counters under-budget real provider cost.
- Turning prompt optimization into a compiler problem: typed IR, deterministic
  passes, and auditable behavior-preservation checks.
- Building practical model routers where cost, latency, and task quality are
  first-class inputs.
- Connecting local coding agents to the same economics: use smaller/faster
  models for simple work, stronger models for architecture and high-risk
  changes.

## Research Threads

- Tokenizer calibration: when proxy tokenizers are accurate, biased, or systematically unsafe for budgeting.
- Prompt compilers: deterministic transformations that reduce cost without asking another model to rewrite the prompt.
- Cost-quality frontiers: reproducible routing policies that choose models rationally per task class.
- Agent model selection: AST and repo signals that predict when a coding task needs stronger reasoning.

## Writing

- [HackerNoon — Faraazuddin Mohammed](https://hackernoon.com/u/faraa2m)

## Elsewhere

- [GitHub @faraa2m](https://github.com/faraa2m)
- [LinkedIn](https://www.linkedin.com/in/faraazuddin-mohammed/)
- [HackerNoon](https://hackernoon.com/u/faraa2m)
- [Tokenometer](https://tokenometer.dev)
