# Faraazuddin Mohammed

I build open-source tools for token economics: measuring LLM cost accurately, reducing prompt waste deterministically, and routing work to the cheapest model that is still good enough.

The through-line is simple: model choice should be an engineering decision with evidence, not a default dropdown.

## Links

- [Portfolio / Resume](https://faraazuddin-mohammed.com)
- [Project Showcase](https://faraazuddin-mohammed.dev)
- [Domain Chooser](https://faraazuddin-mohammed.io)
- [LinkedIn](https://www.linkedin.com/in/faraazuddin-mohammed/)
- [HackerNoon](https://hackernoon.com/u/faraa2m)

## Token Economics Stack

| Project | What it does | Role in the stack |
|---|---|---|
| [`tokenometer`](https://github.com/faraa2m/tokenometer) | Multi-provider token counts, USD cost, latency benchmarks, CI cost guardrails, VS Code/Cursor extension, and Claude Code skill. Live at [tokenometer.dev](https://tokenometer.dev). | Measure |
| [`llm-tokens-atlas`](https://github.com/faraa2m/llm-tokens-atlas) | Open benchmark for offline-vs-empirical tokenizer calibration across providers and prompt formats. Dataset on [Hugging Face](https://huggingface.co/datasets/faraa2m/llm-tokens-atlas). | Calibrate |
| [`promptc`](https://github.com/faraa2m/promptc) | Deterministic, LM-free prompt compiler with behavior-preserving cost-reduction passes. | Reduce |
| [`routerlab`](https://github.com/faraa2m/routerlab) | Cost-quality routing for LLM APIs with reproducible Pareto frontiers per task class. | Route |
| [`ast-ai-model-router`](https://github.com/faraa2m/ast-ai-model-router) | AST-aware Claude/Codex wrapper that picks models from task and code complexity signals. | Apply routing to coding agents |
| [`suture`](https://github.com/faraa2m/suture) | Filesystem-first `.ai/` scaffold for local coding-agent orchestration across Claude Code, Codex, Gemini, Cursor, Windsurf, and similar harnesses. | Orchestrate local agents |
| [`farm`](https://github.com/faraa2m/farm) | One skill installed into Claude Code, Codex, and Grok CLI: whichever agent you are talking to triages the request, briefs the other two headlessly, and verifies what comes back. | Delegate across agents |
| [`commerce-api-starter`](https://github.com/faraa2m/commerce-api-starter) | TypeScript Express commerce API starter with OpenAPI docs, tests, Docker, and LLM cost-guardrail examples. | Demonstrate |

## Start Here

- Use **Tokenometer** if you need a practical tool today: CLI, CI guardrail,
  GitHub Action, VS Code/Cursor extension, MCP server, and web playground.
- Use **llm-tokens-atlas** if you need reproducible evidence about how far
  offline tokenizers drift from provider-empirical counts.
- Use **PromptC** if you want deterministic, LM-free prompt optimization with
  explicit pass semantics instead of opaque prompt rewriting.
- Use **RouterLab** if you want to make model choice a cost-quality frontier
  decision rather than a default model setting.
- Use **AST AI Model Router** if you want that routing idea applied to local
  Claude Code / Codex workflows.
- Use **Suture** if you want a drop-in `.ai/` control plane that keeps router
  policy, memory, hooks, model-role config, and external skill mounts in plain
  files.
- Use **Farm** if you run more than one local coding agent and want the one
  you are talking to decide what to hand off to the others, in parallel, with
  results on disk instead of copy-paste between terminals.
- Use **Commerce API Starter** if you want a compact TypeScript API starter that shows
  tests, OpenAPI-style docs, Docker, and Tokenometer cost-guardrail examples in
  a normal application repo.

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
- Turning local agent orchestration into filesystem state instead of chat
  transcript bloat.
- Letting heterogeneous coding agents delegate to each other: a shared triage
  protocol for what is worth farming out, and headless dispatch to whichever
  harness is cheapest and best suited for the slice.

## Research Threads

- Tokenizer calibration: when proxy tokenizers are accurate, biased, or systematically unsafe for budgeting.
- Prompt compilers: deterministic transformations that reduce cost without asking another model to rewrite the prompt.
- Cost-quality frontiers: reproducible routing policies that choose models rationally per task class.
- Agent model selection: AST and repo signals that predict when a coding task needs stronger reasoning.
- Filesystem-first agent orchestration: Markdown memory, shell hooks, and
  cross-harness skill mounts as a local control plane.

## Writing

- [HackerNoon — Faraazuddin Mohammed](https://hackernoon.com/u/faraa2m)

## Elsewhere

- [GitHub @faraa2m](https://github.com/faraa2m)
- [Portfolio / Resume](https://faraazuddin-mohammed.com)
- [Project Showcase](https://faraazuddin-mohammed.dev)
- [LinkedIn](https://www.linkedin.com/in/faraazuddin-mohammed/)
- [HackerNoon](https://hackernoon.com/u/faraa2m)
- [Tokenometer](https://tokenometer.dev)
- [Suture](https://github.com/faraa2m/suture)
