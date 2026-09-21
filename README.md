# Awesome Jev

A curated list of open-source projects built with [Jev](https://typesafe.ai/blog/introducing-system-one-models-and-jev), TypeSafe AI's "System One Model" — a non-chat model that takes unstructured state plus a typed question (a boolean, a choice, or a score) and returns a calibrated typed decision instead of free text.

## Contents

- [Coding Agents & Dev Tooling](#coding-agents--dev-tooling)
- [Browser & Computer-Use Automation](#browser--computer-use-automation)
- [Search, Retrieval & Data Labeling](#search-retrieval--data-labeling)
- [SDKs & Platform Integrations](#sdks--platform-integrations)
- [Open-Source Jev Alternatives](#open-source-jev-alternatives)
- [Applied Decisions: Games, Robotics, Finance & Productivity](#applied-decisions-games-robotics-finance--productivity)

## Coding Agents & Dev Tooling

Coding-agent runtimes, plugins, and review workflows that use Jev to gate, route, or score agent actions instead of calling an LLM for every decision.

- **[abide](https://github.com/coldteadotai/abide)** ![GitHub stars](https://img.shields.io/github/stars/coldteadotai/abide?style=flat) — Reads every edit a coding agent makes and flags rule violations against project conventions using Jev.
- **[atomic](https://github.com/bastani-inc/atomic)** ![GitHub stars](https://img.shields.io/github/stars/bastani-inc/atomic?style=flat) — Coding-agent runtime that defines process stages, checks, and approval gates in natural language, verified in part by a Jev decision provider.
- **[fast-jev-compaction](https://github.com/tamaratran/fast-jev-compaction)** ![GitHub stars](https://img.shields.io/github/stars/tamaratran/fast-jev-compaction?style=flat) — Claude Code plugin that replaces summarization-based context compaction with per-item Jev relevance scoring, dropping or truncating stale tool results.
- **[foreman](https://github.com/thruwire/foreman)** ![GitHub stars](https://img.shields.io/github/stars/thruwire/foreman?style=flat) — Software-factory layer above Codex workers where Jev independently judges whether an implementation is complete or needs a human.
- **[fx](https://github.com/vercel-labs/fx)** ![GitHub stars](https://img.shields.io/github/stars/vercel-labs/fx?style=flat) — Vercel Labs' terminal coding agent that routes permission decisions through a Jev-backed reviewer instead of an LLM call.
- **[grok-bot-jev](https://github.com/Bodila51/grok-bot-jev)** ![GitHub stars](https://img.shields.io/github/stars/Bodila51/grok-bot-jev?style=flat) — Wires a Jev decision layer into Grok Bot for cheap, gated tool usage with example skill templates.
- **[jev-pruner](https://github.com/tamaratran/jev-pruner)** ![GitHub stars](https://img.shields.io/github/stars/tamaratran/jev-pruner?style=flat) — Claude Code plugin that trims noisy Bash output with Jev before it reaches the model's context.
- **[jev-review](https://github.com/devagrawal09/jev-review)** ![GitHub stars](https://img.shields.io/github/stars/devagrawal09/jev-review?style=flat) — Staged code-review workflow and local dashboard where each stage is gated by a Jev decision.
- **[jev-router](https://github.com/gargpratyush/jev-router)** ![GitHub stars](https://img.shields.io/github/stars/gargpratyush/jev-router?style=flat) — Routes Claude Code tasks to the cheapest capable model by asking Jev to choose among candidates.
- **[openwork](https://github.com/different-ai/openwork)** ![GitHub stars](https://img.shields.io/github/stars/different-ai/openwork?style=flat) — Open-source Claude Cowork alternative (powered by opencode) that uses Jev as a verification judge in its evaluation testkit.
- **[pi-jev](https://github.com/y0usaf/pi-jev)** ![GitHub stars](https://img.shields.io/github/stars/y0usaf/pi-jev?style=flat) — Adds a Jev-backed tool-call safety gate to the Pi coding agent, with a `jev_ask` tool for typed, calibrated answers.
- **[skillbox](https://github.com/kitze/skillbox)** ![GitHub stars](https://img.shields.io/github/stars/kitze/skillbox?style=flat) — Self-hosted, versioned skills library for AI agents with optional Jev-based skill recommendations.
- **[stanley-code](https://github.com/devagrawal09/stanley-code)** ![GitHub stars](https://img.shields.io/github/stars/devagrawal09/stanley-code?style=flat) — Bounded Jev decision workflows that keep coding-agent judgments typed instead of free-form.
- **[supercov](https://github.com/supercorp-ai/supercov)** ![GitHub stars](https://img.shields.io/github/stars/supercorp-ai/supercov?style=flat) — Scores code quality and coverage properties per file with Jev so coding agents know what to fix first.

## Browser & Computer-Use Automation

Browser and desktop agents that use Jev to pick the next click or action, reserving LLM calls for reading and planning.

- **[fastbrowse](https://github.com/agent-labs-dev/fastbrowse)** ![GitHub stars](https://img.shields.io/github/stars/agent-labs-dev/fastbrowse?style=flat) — Browser agent where Jev picks each action from what's on the page while an LLM reads and plans, citing a quote for every claim.
- **[jev-browser](https://github.com/jkudish/jev-browser)** ![GitHub stars](https://img.shields.io/github/stars/jkudish/jev-browser?style=flat) — Drives a browser end-to-end with Jev choosing each step, pitched as a fast, cheap alternative to LLM-driven browsing.
- **[jev-desktop](https://github.com/yikangy873-gif/jev-desktop)** ![GitHub stars](https://img.shields.io/github/stars/yikangy873-gif/jev-desktop?style=flat) — Adds Jev-based action selection to Codex Computer Use for desktop control.
- **[jev-ultrafast](https://github.com/browser-use/jev-ultrafast)** ![GitHub stars](https://img.shields.io/github/stars/browser-use/jev-ultrafast?style=flat) — browser-use's ultrafast agent variant where Jev decides each click and an LLM is only invoked when text must be typed.
- **[typesafe-adblock](https://github.com/realZachi/typesafe-adblock)** ![GitHub stars](https://img.shields.io/github/stars/realZachi/typesafe-adblock?style=flat) — Chrome extension that asks Jev whether each DOM element is an ad before removing it, with no backend.
- **[unclutter](https://github.com/kitze/unclutter)** ![GitHub stars](https://img.shields.io/github/stars/kitze/unclutter?style=flat) — Browser extension that asks Jev, per page element, whether it's clutter, removing it under reusable template rules.
- **[WindTunnel](https://github.com/nekuda-ai/WindTunnel)** ![GitHub stars](https://img.shields.io/github/stars/nekuda-ai/WindTunnel?style=flat) — Benchmark comparing WebMCP against other browser-agent interfaces, including a Jev-based configuration.

## Search, Retrieval & Data Labeling

Classification, reranking, and labeling pipelines that swap an LLM judge for a typed Jev decision.

- **[advocaat](https://github.com/pithings/advocaat)** ![GitHub stars](https://img.shields.io/github/stars/pithings/advocaat?style=flat) — Small, type-safe client for asking Jev questions about your own dataset.
- **[docjev](https://github.com/jerryjliu/docjev)** ![GitHub stars](https://img.shields.io/github/stars/jerryjliu/docjev?style=flat) — Fast document classifier and splitter that matches documents against natural-language category rules using Jev.
- **[hippo-memory](https://github.com/kitfunso/hippo-memory)** ![GitHub stars](https://img.shields.io/github/stars/kitfunso/hippo-memory?style=flat) — Biologically-inspired agent memory store with decay and consolidation, benchmarked with an opt-in Jev reranker.
- **[jev-align](https://github.com/sutro-sh/jev-align)** ![GitHub stars](https://img.shields.io/github/stars/sutro-sh/jev-align?style=flat) — Builds calibrated "AI functions" from human feedback by combining Jev decisions with GEPA optimization.
- **[jev-search](https://github.com/superagents-lab/jev-search)** ![GitHub stars](https://img.shields.io/github/stars/superagents-lab/jev-search?style=flat) — Reranks web search results by source selection, query understanding, and relevance using Jev.
- **[jev-semgrep](https://github.com/uehaj/jev-semgrep)** ![GitHub stars](https://img.shields.io/github/stars/uehaj/jev-semgrep?style=flat) — Greps across languages by meaning, scoring every line against a plain-language description with Jev.
- **[notra](https://github.com/usenotra/notra)** ![GitHub stars](https://img.shields.io/github/stars/usenotra/notra?style=flat) — Marketing-analytics platform whose brand-visibility classifiers can run on Jev instead of an LLM.

## SDKs & Platform Integrations

Official and community SDKs, CLIs, and frameworks that expose Jev as a first-class inference type.

- **[ai-cli](https://github.com/vercel-labs/ai-cli)** ![GitHub stars](https://img.shields.io/github/stars/vercel-labs/ai-cli?style=flat) — Vercel Labs terminal tool that can run Jev as the evaluation model for its `evaluate` command.
- **[ai-python](https://github.com/vercel-labs/ai-python)** ![GitHub stars](https://img.shields.io/github/stars/vercel-labs/ai-python?style=flat) — Official Vercel AI SDK for Python, which exposes Jev through its evaluation API and gateway examples.
- **[eve](https://github.com/vercel/eve)** ![GitHub stars](https://img.shields.io/github/stars/vercel/eve?style=flat) — Vercel's open agent framework that ships Jev as the default model for its experimental evaluate path.
- **[jev-mcp](https://github.com/jkudish/jev-mcp)** ![GitHub stars](https://img.shields.io/github/stars/jkudish/jev-mcp?style=flat) — MCP server exposing Jev claim verification, content screening, and candidate ranking as standard tools.
- **[json-render](https://github.com/vercel-labs/json-render)** ![GitHub stars](https://img.shields.io/github/stars/vercel-labs/json-render?style=flat) — Generative UI framework that uses Jev in its compose path to decide which components and actions to render.
- **[neurolink](https://github.com/juspay/neurolink)** ![GitHub stars](https://img.shields.io/github/stars/juspay/neurolink?style=flat) — TypeScript interface over 40 AI providers with a first-class "decide" inference type backed by Jev, returning typed booleans, choices, and scores.
- **[skills](https://github.com/typesafe-ai/skills)** ![GitHub stars](https://img.shields.io/github/stars/typesafe-ai/skills?style=flat) — TypeSafe AI's official installable agent-skills package that teaches coding agents the Jev workflow.
- **[smithers](https://github.com/smithersai/smithers)** ![GitHub stars](https://img.shields.io/github/stars/smithersai/smithers?style=flat) — TypeScript agentic-workflow framework with a Jev session checker wired into its execution model.
- **[system-one-adapter-python](https://github.com/typesafe-ai/system-one-adapter-python)** ![GitHub stars](https://img.shields.io/github/stars/typesafe-ai/system-one-adapter-python?style=flat) — TypeSafe AI's official adapter for running and benchmarking Jev-style decisions against OpenAI- and Anthropic-compatible APIs.

## Open-Source Jev Alternatives

Small, non-autoregressive decision models that replicate Jev's typed-output behavior and can be self-hosted.

- **[decider](https://github.com/Mapika/decider)** ![GitHub stars](https://img.shields.io/github/stars/Mapika/decider?style=flat) — Qwen3.5 fine-tune family reproducing the System One shape, emitting typed decisions with calibrated probabilities in one pass.
- **[jevlike](https://github.com/vinnylarouge/jevlike)** ![GitHub stars](https://img.shields.io/github/stars/vinnylarouge/jevlike?style=flat) — Training library for models that score a changing list of text options in a single forward pass.
- **[kev](https://github.com/jaredpalmer/kev)** ![GitHub stars](https://img.shields.io/github/stars/jaredpalmer/kev?style=flat) — Family of small Jev-like decision models built on Qwen3.5 that you can train and run locally.
- **[laya](https://github.com/NandhaKishorM/laya)** ![GitHub stars](https://img.shields.io/github/stars/NandhaKishorM/laya?style=flat) — Non-autoregressive open decision model answering choice, score, and boolean questions with calibrated probabilities.
- **[laya-mlx](https://github.com/mizorewww/laya-mlx)** ![GitHub stars](https://img.shields.io/github/stars/mizorewww/laya-mlx?style=flat) — Native Apple Silicon MLX runtime for Laya, running short typed decisions locally with no PyTorch or cloud API.
- **[NanoJev](https://github.com/TianyuCodings/NanoJev)** ![GitHub stars](https://img.shields.io/github/stars/TianyuCodings/NanoJev?style=flat) — Nano replica of Jev with parallel decisions, dynamic candidates, and an end-to-end training pipeline.
- **[openJev-verdict-2.0](https://github.com/Heman10x-NGU/openJev-verdict-2.0)** ![GitHub stars](https://img.shields.io/github/stars/Heman10x-NGU/openJev-verdict-2.0?style=flat) — Calibrated 151M non-autoregressive decision engine reporting higher benchmark accuracy than Jev and Laya on typed-decision tasks.
- **[OpenDecision](https://github.com/deepanwadhwa/OpenDecision)** ![GitHub stars](https://img.shields.io/github/stars/deepanwadhwa/OpenDecision?style=flat) — Open-source semantic decision engine positioned as a local equivalent to Jev.
- **[von](https://github.com/wfzyx/von)** ![GitHub stars](https://img.shields.io/github/stars/wfzyx/von?style=flat) — Sub-15ms non-autoregressive model answering typed questions with calibrated probabilities as a local Jev drop-in.

## Applied Decisions: Games, Robotics, Finance & Productivity

Domain-specific projects that put a Jev decision loop in front of a real task, from game-playing to trading.

- **[jev-drone](https://github.com/RomanSlack/jev-drone)** ![GitHub stars](https://img.shields.io/github/stars/RomanSlack/jev-drone?style=flat) — Camera-only autonomous drone simulated in MuJoCo with a Jev judgment model in the control loop at 2.5Hz.
- **[Jev-X-Sentiment-Analysis](https://github.com/brainstormity/Jev-X-Sentiment-Analysis)** ![GitHub stars](https://img.shields.io/github/stars/brainstormity/Jev-X-Sentiment-Analysis?style=flat) — Turns crypto Twitter sentiment into Jev-generated trade decision cards without executing trades.
- **[jev-experiments](https://github.com/dabit3/jev-experiments)** ![GitHub stars](https://img.shields.io/github/stars/dabit3/jev-experiments?style=flat) — Collection of small, latency-focused Jev demo apps spanning shell guards, log monitoring, search, and reranking.
- **[jev-trade](https://github.com/aowang-ai/jev-trade)** ![GitHub stars](https://img.shields.io/github/stars/aowang-ai/jev-trade?style=flat) — Live crypto trading bot that asks Jev to choose long or short on Hyperliquid markets each round.
- **[minutes](https://github.com/silverstein/minutes)** ![GitHub stars](https://img.shields.io/github/stars/silverstein/minutes?style=flat) — Local-first, open-source meeting-transcription app whose live voice pipeline runs evaluation through Jev.
- **[typesafe-mario](https://github.com/fhshaik/typesafe-mario)** ![GitHub stars](https://img.shields.io/github/stars/fhshaik/typesafe-mario?style=flat) — Jev agent that plays Super Mario Bros. by choosing actions from structured emulator state.

## Related Lists

- [awesome-typesafe-jev](https://github.com/AbdelStark/awesome-typesafe-jev) — A broader, source-backed field guide to the Jev ecosystem.
- [awesome-jev-by-typesafe](https://github.com/Anil-matcha/awesome-jev-by-typesafe) — Evidence-backed use cases and starter code for TypeSafe Jev.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for inclusion criteria and how to submit a project.

## License

[MIT](LICENSE)
