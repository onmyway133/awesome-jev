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
- **[Agent](https://github.com/AgentiLoop/Agent)** ![GitHub stars](https://img.shields.io/github/stars/AgentiLoop/Agent?style=flat) — Native macOS coding agent with a Jev-backed command-risk advisor that flags dangerous actions before they run.
- **[atomic](https://github.com/bastani-inc/atomic)** ![GitHub stars](https://img.shields.io/github/stars/bastani-inc/atomic?style=flat) — Coding-agent runtime that defines process stages, checks, and approval gates in natural language, verified in part by a Jev decision provider.
- **[celesto](https://github.com/CelestoAI/celesto)** ![GitHub stars](https://img.shields.io/github/stars/CelestoAI/celesto?style=flat) — PR-review example pairing a general model with Jev to double-check findings on the same candidate diffs.
- **[fast-jev-compaction](https://github.com/tamaratran/fast-jev-compaction)** ![GitHub stars](https://img.shields.io/github/stars/tamaratran/fast-jev-compaction?style=flat) — Claude Code plugin that replaces summarization-based context compaction with per-item Jev relevance scoring, dropping or truncating stale tool results.
- **[firstmate](https://github.com/kunchenguid/firstmate)** ![GitHub stars](https://img.shields.io/github/stars/kunchenguid/firstmate?style=flat) — Matches incoming task briefs to dispatch rules with Jev before local policy picks the final agent configuration.
- **[foreman](https://github.com/thruwire/foreman)** ![GitHub stars](https://img.shields.io/github/stars/thruwire/foreman?style=flat) — Software-factory layer above Codex workers where Jev independently judges whether an implementation is complete or needs a human.
- **[fx](https://github.com/vercel-labs/fx)** ![GitHub stars](https://img.shields.io/github/stars/vercel-labs/fx?style=flat) — Vercel Labs' terminal coding agent that routes permission decisions through a Jev-backed reviewer instead of an LLM call.
- **[grok-bot-jev](https://github.com/Bodila51/grok-bot-jev)** ![GitHub stars](https://img.shields.io/github/stars/Bodila51/grok-bot-jev?style=flat) — Wires a Jev decision layer into Grok Bot for cheap, gated tool usage with example skill templates.
- **[hermes-jev-skills](https://github.com/kerpopule/hermes-jev-skills)** ![GitHub stars](https://img.shields.io/github/stars/kerpopule/hermes-jev-skills?style=flat) — Skill pack adding Jev-driven model routing, memory compaction, and computer/browser-use decisions to Hermes, Claude Code, and Codex agents.
- **[interlinked-cli](https://github.com/QuentinCody/interlinked-cli)** ![GitHub stars](https://img.shields.io/github/stars/QuentinCody/interlinked-cli?style=flat) — CLI that adds Jev-backed judgment and evidence checks on top of local coding-agent verification steps.
- **[jev-codex-router](https://github.com/0xNatoshi/jev-codex-router)** ![GitHub stars](https://img.shields.io/github/stars/0xNatoshi/jev-codex-router?style=flat) — Classifies each Codex turn with Jev, then applies local rules to pick the model, reasoning effort, and speed mode.
- **[jev-dsh-decision](https://github.com/Devin-AXIS/jev-dsh-decision)** ![GitHub stars](https://img.shields.io/github/stars/Devin-AXIS/jev-dsh-decision?style=flat) — Structured decision layer for Agent Harness that recommends tools, skills, and agents with Jev-scored probabilities.
- **[jev-eval-agent](https://github.com/vinilana/jev-eval-agent)** ![GitHub stars](https://img.shields.io/github/stars/vinilana/jev-eval-agent?style=flat) — Benchmark harness comparing standard LLM tool selection against Jev-based routing across 100 mocked tools.
- **[jev-pruner](https://github.com/tamaratran/jev-pruner)** ![GitHub stars](https://img.shields.io/github/stars/tamaratran/jev-pruner?style=flat) — Claude Code plugin that trims noisy Bash output with Jev before it reaches the model's context.
- **[jev-review](https://github.com/devagrawal09/jev-review)** ![GitHub stars](https://img.shields.io/github/stars/devagrawal09/jev-review?style=flat) — Staged code-review workflow and local dashboard where each stage is gated by a Jev decision.
- **[jev-review](https://github.com/NiazMorshed2007/jev-review)** ![GitHub stars](https://img.shields.io/github/stars/NiazMorshed2007/jev-review?style=flat) — Local MCP server that reviews code quality and hands coding agents structured, Jev-scored feedback.
- **[jev-router](https://github.com/gargpratyush/jev-router)** ![GitHub stars](https://img.shields.io/github/stars/gargpratyush/jev-router?style=flat) — Routes Claude Code tasks to the cheapest capable model by asking Jev to choose among candidates.
- **[jev-shell-history](https://github.com/mrnugget/jev-shell-history)** ![GitHub stars](https://img.shields.io/github/stars/mrnugget/jev-shell-history?style=flat) — Zsh history suggester that ranks candidate shell commands with Jev instead of plain frequency.
- **[JevRouter](https://github.com/BillionsBobby/JevRouter)** ![GitHub stars](https://img.shields.io/github/stars/BillionsBobby/JevRouter?style=flat) — Routes a shared candidate set across models, subagents, skills, MCP tools, and CLIs using Jev.
- **[openchamber](https://github.com/openchamber/openchamber)** ![GitHub stars](https://img.shields.io/github/stars/openchamber/openchamber?style=flat) — AI chat client whose automatic model router asks Jev to classify each message before picking a model and reasoning level.
- **[openwork](https://github.com/different-ai/openwork)** ![GitHub stars](https://img.shields.io/github/stars/different-ai/openwork?style=flat) — Open-source Claude Cowork alternative (powered by opencode) that uses Jev as a verification judge in its evaluation testkit.
- **[orchestkit](https://github.com/yonatangross/orchestkit)** ![GitHub stars](https://img.shields.io/github/stars/yonatangross/orchestkit?style=flat) — Coding-session manager that can classify sessions with Jev and color-code them once confidence clears a threshold.
- **[pi-fabric](https://github.com/monotykamary/pi-fabric)** ![GitHub stars](https://img.shields.io/github/stars/monotykamary/pi-fabric?style=flat) — Programmable agent runtime for Pi with an optional Jev loop for observing state and running bounded actions.
- **[pi-jev](https://github.com/y0usaf/pi-jev)** ![GitHub stars](https://img.shields.io/github/stars/y0usaf/pi-jev?style=flat) — Adds a Jev-backed tool-call safety gate to the Pi coding agent, with a `jev_ask` tool for typed, calibrated answers.
- **[pi-warden](https://github.com/DevMortimer/pi-warden)** ![GitHub stars](https://img.shields.io/github/stars/DevMortimer/pi-warden?style=flat) — Guardrail layer for Pi agents that checks project rules, scope creep, repeated failures, and false completion claims.
- **[skillbox](https://github.com/kitze/skillbox)** ![GitHub stars](https://img.shields.io/github/stars/kitze/skillbox?style=flat) — Self-hosted, versioned skills library for AI agents with optional Jev-based skill recommendations.
- **[stanley-code](https://github.com/devagrawal09/stanley-code)** ![GitHub stars](https://img.shields.io/github/stars/devagrawal09/stanley-code?style=flat) — Bounded Jev decision workflows that keep coding-agent judgments typed instead of free-form.
- **[supercov](https://github.com/supercorp-ai/supercov)** ![GitHub stars](https://img.shields.io/github/stars/supercorp-ai/supercov?style=flat) — Scores code quality and coverage properties per file with Jev so coding agents know what to fix first.
- **[taskuary](https://github.com/ldbumble/taskuary)** ![GitHub stars](https://img.shields.io/github/stars/ldbumble/taskuary?style=flat) — Task-tracking tool with a Jev judgment module that checks user-defined conditions against task state.
- **[vexjoy-agent](https://github.com/notque/vexjoy-agent)** ![GitHub stars](https://img.shields.io/github/stars/notque/vexjoy-agent?style=flat) — Routes VexJoy requests to specialist agents, skills, and workflows via an optional Jev dispatch path.
- **[WrongStack](https://github.com/WrongStack/WrongStack)** ![GitHub stars](https://img.shields.io/github/stars/WrongStack/WrongStack?style=flat) — Dispatches incoming work to specialist agents using a Jev classifier instead of hardcoded rules.

## Browser & Computer-Use Automation

Browser and desktop agents that use Jev to pick the next click or action, reserving LLM calls for reading and planning.

- **[agent-desktop](https://github.com/lahfir/agent-desktop)** ![GitHub stars](https://img.shields.io/github/stars/lahfir/agent-desktop?style=flat) — Desktop agent skill that reads native accessibility data and lets Jev choose which control or action to trigger.
- **[fastbrowse](https://github.com/agent-labs-dev/fastbrowse)** ![GitHub stars](https://img.shields.io/github/stars/agent-labs-dev/fastbrowse?style=flat) — Browser agent where Jev picks each action from what's on the page while an LLM reads and plans, citing a quote for every claim.
- **[jev-browser](https://github.com/jkudish/jev-browser)** ![GitHub stars](https://img.shields.io/github/stars/jkudish/jev-browser?style=flat) — Drives a browser end-to-end with Jev choosing each step, pitched as a fast, cheap alternative to LLM-driven browsing.
- **[jev-browser](https://github.com/Ying-Kai-Liao/jev-browser)** ![GitHub stars](https://img.shields.io/github/stars/Ying-Kai-Liao/jev-browser?style=flat) — Browser library, CLI, and MCP server where callers supply a goal and Jev selects the actions to reach it.
- **[jev-browser-use](https://github.com/wy-coliney/jev-browser-use)** ![GitHub stars](https://img.shields.io/github/stars/wy-coliney/jev-browser-use?style=flat) — Codex browser-use skill where Jev handles navigation, clicks, and scrolling while Codex only supplies typed text.
- **[Jev-cu](https://github.com/Sac-Y/Jev-cu)** ![GitHub stars](https://img.shields.io/github/stars/Sac-Y/Jev-cu?style=flat) — Codex Computer Use loop that sends text candidates to Jev while desktop tools handle observation and execution.
- **[jev-desktop](https://github.com/yikangy873-gif/jev-desktop)** ![GitHub stars](https://img.shields.io/github/stars/yikangy873-gif/jev-desktop?style=flat) — Adds Jev-based action selection to Codex Computer Use for desktop control.
- **[jev-ultrafast](https://github.com/browser-use/jev-ultrafast)** ![GitHub stars](https://img.shields.io/github/stars/browser-use/jev-ultrafast?style=flat) — browser-use's ultrafast agent variant where Jev decides each click and an LLM is only invoked when text must be typed.
- **[jev-use](https://github.com/savka777/jev-use)** ![GitHub stars](https://img.shields.io/github/stars/savka777/jev-use?style=flat) — Voice-driven macOS computer use: you speak a goal, Jev picks the next on-screen action from the accessibility tree, no screenshots needed.
- **[jev-voice-browser](https://github.com/moritzkremb/jev-voice-browser)** ![GitHub stars](https://img.shields.io/github/stars/moritzkremb/jev-voice-browser?style=flat) — Drives a Playwright browser session from incremental speech transcripts routed through Jev.
- **[mobile-jev](https://github.com/droidrun/mobile-jev)** ![GitHub stars](https://img.shields.io/github/stars/droidrun/mobile-jev?style=flat) — Controls an Android phone through Mobilerun, with a web studio and CLI for inspecting each Jev decision.
- **[omg.dev](https://github.com/BennyKok/omg.dev)** ![GitHub stars](https://img.shields.io/github/stars/BennyKok/omg.dev?style=flat) — Mobile testing script that reads the accessibility tree and lets Jev choose the next interaction to test.
- **[typesafe-adblock](https://github.com/realZachi/typesafe-adblock)** ![GitHub stars](https://img.shields.io/github/stars/realZachi/typesafe-adblock?style=flat) — Chrome extension that asks Jev whether each DOM element is an ad before removing it, with no backend.
- **[typesafe-computer-use](https://github.com/awlevin/typesafe-computer-use)** ![GitHub stars](https://img.shields.io/github/stars/awlevin/typesafe-computer-use?style=flat) — Builds candidate actions from OCR and UI state so Jev can drive macOS directly, only calling a text model when typing is required.
- **[unclutter](https://github.com/kitze/unclutter)** ![GitHub stars](https://img.shields.io/github/stars/kitze/unclutter?style=flat) — Browser extension that asks Jev, per page element, whether it's clutter, removing it under reusable template rules.
- **[WindTunnel](https://github.com/nekuda-ai/WindTunnel)** ![GitHub stars](https://img.shields.io/github/stars/nekuda-ai/WindTunnel?style=flat) — Benchmark comparing WebMCP against other browser-agent interfaces, including a Jev-based configuration.

## Search, Retrieval & Data Labeling

Classification, reranking, and labeling pipelines that swap an LLM judge for a typed Jev decision.

- **[advocaat](https://github.com/pithings/advocaat)** ![GitHub stars](https://img.shields.io/github/stars/pithings/advocaat?style=flat) — Small, type-safe client for asking Jev questions about your own dataset.
- **[bluenoise](https://github.com/rokcso/bluenoise)** ![GitHub stars](https://img.shields.io/github/stars/rokcso/bluenoise?style=flat) — X/Twitter filtering extension that applies local rules first and falls back to Jev for replies that don't match.
- **[docjev](https://github.com/jerryjliu/docjev)** ![GitHub stars](https://img.shields.io/github/stars/jerryjliu/docjev?style=flat) — Fast document classifier and splitter that matches documents against natural-language category rules using Jev.
- **[hippo-memory](https://github.com/kitfunso/hippo-memory)** ![GitHub stars](https://img.shields.io/github/stars/kitfunso/hippo-memory?style=flat) — Biologically-inspired agent memory store with decay and consolidation, benchmarked with an opt-in Jev reranker.
- **[jev-align](https://github.com/sutro-sh/jev-align)** ![GitHub stars](https://img.shields.io/github/stars/sutro-sh/jev-align?style=flat) — Builds calibrated "AI functions" from human feedback by combining Jev decisions with GEPA optimization.
- **[jev-search](https://github.com/superagents-lab/jev-search)** ![GitHub stars](https://img.shields.io/github/stars/superagents-lab/jev-search?style=flat) — Reranks web search results by source selection, query understanding, and relevance using Jev.
- **[jev-semgrep](https://github.com/uehaj/jev-semgrep)** ![GitHub stars](https://img.shields.io/github/stars/uehaj/jev-semgrep?style=flat) — Greps across languages by meaning, scoring every line against a plain-language description with Jev.
- **[kody](https://github.com/kentcdodds/kody)** ![GitHub stars](https://img.shields.io/github/stars/kentcdodds/kody?style=flat) — Two-stage search that widens a hybrid retrieval pool, then reranks candidates with a Jev score.
- **[neo4jev](https://github.com/jexp/neo4jev)** ![GitHub stars](https://img.shields.io/github/stars/jexp/neo4jev?style=flat) — Walks a Neo4j graph one hop at a time, asking Jev which relationship to follow next.
- **[notra](https://github.com/usenotra/notra)** ![GitHub stars](https://img.shields.io/github/stars/usenotra/notra?style=flat) — Marketing-analytics platform whose brand-visibility classifiers can run on Jev instead of an LLM.
- **[tax-doc-classifier](https://github.com/kyotofin/tax-doc-classifier)** ![GitHub stars](https://img.shields.io/github/stars/kyotofin/tax-doc-classifier?style=flat) — Classifies scanned tax-document pages into IRS form categories using Jev.
- **[youtube-sponsor-detection](https://github.com/trungdq88/youtube-sponsor-detection)** ![GitHub stars](https://img.shields.io/github/stars/trungdq88/youtube-sponsor-detection?style=flat) — Browser extension that flags and skips sponsored YouTube segments by classifying live audio and transcripts with Jev.

## SDKs & Platform Integrations

Official and community SDKs, CLIs, and frameworks that expose Jev as a first-class inference type.

- **[agentgateway](https://github.com/agentgateway/agentgateway)** ![GitHub stars](https://img.shields.io/github/stars/agentgateway/agentgateway?style=flat) — AI gateway with a Jev guardrail example that inspects model requests and responses via webhook.
- **[ai](https://github.com/hackclub/ai)** ![GitHub stars](https://img.shields.io/github/stars/hackclub/ai?style=flat) — Hack Club's AI proxy that forwards requests to Jev while reusing its own auth, rate limits, and usage logging.
- **[ai-cli](https://github.com/vercel-labs/ai-cli)** ![GitHub stars](https://img.shields.io/github/stars/vercel-labs/ai-cli?style=flat) — Vercel Labs terminal tool that can run Jev as the evaluation model for its `evaluate` command.
- **[ai-python](https://github.com/vercel-labs/ai-python)** ![GitHub stars](https://img.shields.io/github/stars/vercel-labs/ai-python?style=flat) — Official Vercel AI SDK for Python, which exposes Jev through its evaluation API and gateway examples.
- **[ax](https://github.com/ax-llm/ax)** ![GitHub stars](https://img.shields.io/github/stars/ax-llm/ax?style=flat) — DSPy-style TypeScript framework with a TypeSafe integration for boolean and finite-class signatures answered natively by Jev.
- **[effect-agent](https://github.com/danieljvdm/effect-agent)** ![GitHub stars](https://img.shields.io/github/stars/danieljvdm/effect-agent?style=flat) — Effect-based agent framework with a TypeSafe decision provider for typed question sets and optional model selection.
- **[eve](https://github.com/vercel/eve)** ![GitHub stars](https://img.shields.io/github/stars/vercel/eve?style=flat) — Vercel's open agent framework that ships Jev as the default model for its experimental evaluate path.
- **[instructor-php](https://github.com/cognesy/instructor-php)** ![GitHub stars](https://img.shields.io/github/stars/cognesy/instructor-php?style=flat) — Structured-output PHP library whose Polyglot module includes a dedicated TypeSafe decision driver for Jev.
- **[jev-mcp](https://github.com/jkudish/jev-mcp)** ![GitHub stars](https://img.shields.io/github/stars/jkudish/jev-mcp?style=flat) — MCP server exposing Jev claim verification, content screening, and candidate ranking as standard tools.
- **[json-render](https://github.com/vercel-labs/json-render)** ![GitHub stars](https://img.shields.io/github/stars/vercel-labs/json-render?style=flat) — Generative UI framework that uses Jev in its compose path to decide which components and actions to render.
- **[latitude-llm](https://github.com/latitude-dev/latitude-llm)** ![GitHub stars](https://img.shields.io/github/stars/latitude-dev/latitude-llm?style=flat) — LLM engineering platform with an optional Jev preclassifier for conversation checks and prompt selection.
- **[neurolink](https://github.com/juspay/neurolink)** ![GitHub stars](https://img.shields.io/github/stars/juspay/neurolink?style=flat) — TypeScript interface over 40 AI providers with a first-class "decide" inference type backed by Jev, returning typed booleans, choices, and scores.
- **[openai-scala-client](https://github.com/cequence-io/openai-scala-client)** ![GitHub stars](https://img.shields.io/github/stars/cequence-io/openai-scala-client?style=flat) — Multi-provider Scala AI client with a dedicated TypeSafe module for calling Jev.
- **[pg-jev](https://github.com/realZachi/pg-jev)** ![GitHub stars](https://img.shields.io/github/stars/realZachi/pg-jev?style=flat) — Adds natural-language filtering, classification, and ranking of Postgres rows via Jev.
- **[pg_typesafe](https://github.com/giuliosmall/pg_typesafe)** ![GitHub stars](https://img.shields.io/github/stars/giuliosmall/pg_typesafe?style=flat) — Pre-alpha PostgreSQL C extension that calls Jev directly from SQL for classification, yes/no judgments, and scoring.
- **[req_llm](https://github.com/agentjido/req_llm)** ![GitHub stars](https://img.shields.io/github/stars/agentjido/req_llm?style=flat) — Elixir LLM client with a TypeSafe provider that routes evaluate calls to Jev.
- **[rig](https://github.com/0xPlaygrounds/rig)** ![GitHub stars](https://img.shields.io/github/stars/0xPlaygrounds/rig?style=flat) — Rust LLM application framework with an experimental TypeSafe crate for typed Jev questions and answers.
- **[runline](https://github.com/Michaelliv/runline)** ![GitHub stars](https://img.shields.io/github/stars/Michaelliv/runline?style=flat) — TypeSafe plugin for Runline that exposes Jev decisions as callable actions in agent JavaScript.
- **[skills](https://github.com/typesafe-ai/skills)** ![GitHub stars](https://img.shields.io/github/stars/typesafe-ai/skills?style=flat) — TypeSafe AI's official installable agent-skills package that teaches coding agents the Jev workflow.
- **[smithers](https://github.com/smithersai/smithers)** ![GitHub stars](https://img.shields.io/github/stars/smithersai/smithers?style=flat) — TypeScript agentic-workflow framework with a Jev session checker wired into its execution model.
- **[system-one-adapter-python](https://github.com/typesafe-ai/system-one-adapter-python)** ![GitHub stars](https://img.shields.io/github/stars/typesafe-ai/system-one-adapter-python?style=flat) — TypeSafe AI's official adapter for running and benchmarking Jev-style decisions against OpenAI- and Anthropic-compatible APIs.
- **[typesafe-mcp](https://github.com/itsmostafa/typesafe-mcp)** ![GitHub stars](https://img.shields.io/github/stars/itsmostafa/typesafe-mcp?style=flat) — MCP server that lets Claude Code, Claude Desktop, Codex, and Pi send typed questions straight to Jev.
- **[typesafe-sdk-js](https://github.com/typesafe-ai/typesafe-sdk-js)** ![GitHub stars](https://img.shields.io/github/stars/typesafe-ai/typesafe-sdk-js?style=flat) — TypeSafe AI's official JavaScript/TypeScript SDK for typed Jev requests and answers.
- **[typesafe-sdk-python](https://github.com/typesafe-ai/typesafe-sdk-python)** ![GitHub stars](https://img.shields.io/github/stars/typesafe-ai/typesafe-sdk-python?style=flat) — TypeSafe AI's official Python SDK, with sync and async clients plus typed question/answer models for Jev.
- **[vellum-assistant](https://github.com/vellum-ai/vellum-assistant)** ![GitHub stars](https://img.shields.io/github/stars/vellum-ai/vellum-assistant?style=flat) — AI-platform assistant with an optional Jev provider for sending conversation state and explicit questions to TypeSafe.

## Open-Source Jev Alternatives

Small, non-autoregressive decision models that replicate Jev's typed-output behavior and can be self-hosted.

- **[decider](https://github.com/Mapika/decider)** ![GitHub stars](https://img.shields.io/github/stars/Mapika/decider?style=flat) — Qwen3.5 fine-tune family reproducing the System One shape, emitting typed decisions with calibrated probabilities in one pass.
- **[jevbench](https://github.com/fstandhartinger/jevbench)** ![GitHub stars](https://img.shields.io/github/stars/fstandhartinger/jevbench?style=flat) — Benchmark suite for Jev-class typed decision models, scoring how smart, cheap, fast, and reliable open alternatives are.
- **[jevlike](https://github.com/vinnylarouge/jevlike)** ![GitHub stars](https://img.shields.io/github/stars/vinnylarouge/jevlike?style=flat) — Training library for models that score a changing list of text options in a single forward pass.
- **[kev](https://github.com/jaredpalmer/kev)** ![GitHub stars](https://img.shields.io/github/stars/jaredpalmer/kev?style=flat) — Family of small Jev-like decision models built on Qwen3.5 that you can train and run locally.
- **[laya](https://github.com/NandhaKishorM/laya)** ![GitHub stars](https://img.shields.io/github/stars/NandhaKishorM/laya?style=flat) — Non-autoregressive open decision model answering choice, score, and boolean questions with calibrated probabilities.
- **[laya-mlx](https://github.com/mizorewww/laya-mlx)** ![GitHub stars](https://img.shields.io/github/stars/mizorewww/laya-mlx?style=flat) — Native Apple Silicon MLX runtime for Laya, running short typed decisions locally with no PyTorch or cloud API.
- **[NanoJev](https://github.com/TianyuCodings/NanoJev)** ![GitHub stars](https://img.shields.io/github/stars/TianyuCodings/NanoJev?style=flat) — Nano replica of Jev with parallel decisions, dynamic candidates, and an end-to-end training pipeline.
- **[OpenDecision](https://github.com/deepanwadhwa/OpenDecision)** ![GitHub stars](https://img.shields.io/github/stars/deepanwadhwa/OpenDecision?style=flat) — Open-source semantic decision engine positioned as a local equivalent to Jev.
- **[openjev](https://github.com/razorback16/openjev)** ![GitHub stars](https://img.shields.io/github/stars/razorback16/openjev?style=flat) — Independently-run System One decision server compatible with Jev's API, backed by an open DiffusionGemma model.
- **[openJev-verdict-2.0](https://github.com/Heman10x-NGU/openJev-verdict-2.0)** ![GitHub stars](https://img.shields.io/github/stars/Heman10x-NGU/openJev-verdict-2.0?style=flat) — Calibrated 151M non-autoregressive decision engine reporting higher benchmark accuracy than Jev and Laya on typed-decision tasks.
- **[simple-jev](https://github.com/featherless-ai/simple-jev)** ![GitHub stars](https://img.shields.io/github/stars/featherless-ai/simple-jev?style=flat) — Adapter that turns any open LLM endpoint into a Jev-compatible classification service without training a separate head.
- **[von](https://github.com/wfzyx/von)** ![GitHub stars](https://img.shields.io/github/stars/wfzyx/von?style=flat) — Sub-15ms non-autoregressive model answering typed questions with calibrated probabilities as a local Jev drop-in.

## Applied Decisions: Games, Robotics, Finance & Productivity
- [Refix](https://refix.ai) - Growth: AI that helps your product grow faster on autopilot by running product experiments, SEO, content, and ads.

Domain-specific projects that put a Jev decision loop in front of a real task, from game-playing to trading.

- **[aiavatarkit](https://github.com/uezo/aiavatarkit)** ![GitHub stars](https://img.shields.io/github/stars/uezo/aiavatarkit?style=flat) — Voice-avatar toolkit that uses Jev to judge when a speaker's turn has actually ended.
- **[captaincore](https://github.com/CaptainCore/captaincore)** ![GitHub stars](https://img.shields.io/github/stars/CaptainCore/captaincore?style=flat) — WordPress management toolkit where Jev answers structured questions and prioritizes malware-scanner findings for review.
- **[jev-drone](https://github.com/RomanSlack/jev-drone)** ![GitHub stars](https://img.shields.io/github/stars/RomanSlack/jev-drone?style=flat) — Camera-only autonomous drone simulated in MuJoCo with a Jev judgment model in the control loop at 2.5Hz.
- **[jev-experiments](https://github.com/dabit3/jev-experiments)** ![GitHub stars](https://img.shields.io/github/stars/dabit3/jev-experiments?style=flat) — Collection of small, latency-focused Jev demo apps spanning shell guards, log monitoring, search, and reranking.
- **[jev-trade](https://github.com/aowang-ai/jev-trade)** ![GitHub stars](https://img.shields.io/github/stars/aowang-ai/jev-trade?style=flat) — Live crypto trading bot that asks Jev to choose long or short on Hyperliquid markets each round.
- **[jev-trader](https://github.com/jarrodwatts/jev-trader)** ![GitHub stars](https://img.shields.io/github/stars/jarrodwatts/jev-trader?style=flat) — Market-making experiment on Monad's Kuru MON-USDC book with optional per-block buy/sell decisions from Jev.
- **[Jev-X-Sentiment-Analysis](https://github.com/brainstormity/Jev-X-Sentiment-Analysis)** ![GitHub stars](https://img.shields.io/github/stars/brainstormity/Jev-X-Sentiment-Analysis?style=flat) — Turns crypto Twitter sentiment into Jev-generated trade decision cards without executing trades.
- **[jevmeter](https://github.com/ChetasLua/jevmeter)** ![GitHub stars](https://img.shields.io/github/stars/ChetasLua/jevmeter?style=flat) — Generates edited videos with on-screen score meters by having Jev rate transcript sentences against chosen rubrics.
- **[jevpilot](https://github.com/standardagents/jevpilot)** ![GitHub stars](https://img.shields.io/github/stars/standardagents/jevpilot?style=flat) — Browser-based driving simulator where Jev chooses among locally generated paths and speeds.
- **[killmyidea](https://github.com/monteduro/killmyidea)** ![GitHub stars](https://img.shields.io/github/stars/monteduro/killmyidea?style=flat) — Startup-idea evaluator that hands out KILL, FIX, or SHIP verdicts based on Jev scores.
- **[minutes](https://github.com/silverstein/minutes)** ![GitHub stars](https://img.shields.io/github/stars/silverstein/minutes?style=flat) — Local-first, open-source meeting-transcription app whose live voice pipeline runs evaluation through Jev.
- **[OpenWhisper](https://github.com/Knuckles92/OpenWhisper)** ![GitHub stars](https://img.shields.io/github/stars/Knuckles92/OpenWhisper?style=flat) — Dictation and meeting-notes app with optional Jev checks for topic changes and sensitive-text handling.
- **[prism-liquidity-agent](https://github.com/irfndi/prism-liquidity-agent)** ![GitHub stars](https://img.shields.io/github/stars/irfndi/prism-liquidity-agent?style=flat) — Solana liquidity agent that runs Jev judgments in shadow mode against its rule-based decisions.
- **[typesafe-mario](https://github.com/fhshaik/typesafe-mario)** ![GitHub stars](https://img.shields.io/github/stars/fhshaik/typesafe-mario?style=flat) — Jev agent that plays Super Mario Bros. by choosing actions from structured emulator state.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for inclusion criteria and how to submit a project.

## License

[MIT](LICENSE)
