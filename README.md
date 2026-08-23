# Awesome Pi Agent [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated slice of the π ecosystem — the pi coding agent, its extensions,
> skills, frontends, forks, and everything else in orbit.

[pi](https://github.com/earendil-works/pi) is a minimal, hackable, self-extensible
coding agent by Mario Zechner ([@badlogic](https://github.com/badlogic)) and
[Earendil Works](https://github.com/earendil-works). It began life as
"the shitty coding agent" — [shittycodingagent.ai](https://shittycodingagent.ai)
still redirects — and like its namesake constant, the ecosystem turned out to be
irrational and never-ending. This list tries to keep up.

Every link below was alive, unarchived, and pi-relevant when added.
Entries are alphabetical within sections; π doesn't play favorites with its digits.

## Contents

- [The Mothership](#the-mothership)
- [Learning π](#learning-π)
- [Distros, Forks & Things Built on π](#distros-forks--things-built-on-π)
- [Frontends](#frontends)
- [Extension Packs](#extension-packs)
- [Subagents & Multi-Agent](#subagents--multi-agent)
- [Context, Memory & Compaction](#context-memory--compaction)
- [Workflow & Autonomy](#workflow--autonomy)
- [UI & Interaction](#ui--interaction)
- [Safety & Permissions](#safety--permissions)
- [Notifications & Chat Bridges](#notifications--chat-bridges)
- [Skills](#skills)
- [Providers & Model Access](#providers--model-access)
- [MCP, ACP & Code Intelligence](#mcp-acp--code-intelligence)
- [Sandboxes & Isolation](#sandboxes--isolation)
- [Sessions, Observability & Cost](#sessions-observability--cost)
- [Review & QA](#review--qa)
- [Toys & Eye Candy](#toys--eye-candy)
- [Setups & Dotfiles](#setups--dotfiles)
- [Friends of π](#friends-of-π)
- [Lore](#lore)
- [Contributing](#contributing)

## The Mothership

The official project and its immediate family.

- [pi](https://github.com/earendil-works/pi) — The monorepo: unified LLM API (`pi-ai`), agent runtime (`pi-agent-core`), TUI library (`pi-tui`), and the coding agent CLI itself.
- [pi.dev](https://pi.dev) — Project website with demos; docs live at [pi.dev/docs](https://pi.dev/docs/latest).
- [pi-chat](https://github.com/earendil-works/pi-chat) — Sibling project for Slack/chat automation and workflows.
- [pi-skills](https://github.com/badlogic/pi-skills) — The author's skills collection: browser automation, Gmail/GCal/GDrive CLIs, transcription, and more (Claude Code and Codex compatible).
- [absurd](https://github.com/earendil-works/absurd) — "An experiment in durability" from the same lab; durable execution for agent workloads.
- [Discord](https://discord.com/invite/3cU7Bz4UPx) — Where the ecosystem actually happens; half the repos on this list were announced there first.

## Learning π

- [Official docs](https://pi.dev/docs/latest) — CLI, SDK, sessions, compaction, themes, extensions. You can also just ask the agent to explain itself.
- [Extensions guide](https://github.com/earendil-works/pi/blob/main/packages/coding-agent/docs/extensions.md) — The unified extensions API: hooks, tools, events, UI.
- [Examples directory](https://github.com/earendil-works/pi/tree/main/packages/coding-agent/examples) — Working examples for extensions and SDK usage.
- [pi-book](https://github.com/ZhangHanDong/pi-book) — Community-written book on the pi monorepo (Chinese).
- [pi-tutorial](https://github.com/earendil-works/pi-tutorial) — Experimental interactive tutorial mode for pi.
- [mariozechner.at](https://mariozechner.at) — The author's blog; design rationale straight from the source.
- [mpr: pi coding agent notes](https://github.com/crossjam/mpr/blob/main/content/pi_coding_agent.md) — Community writeup and context.

## Distros, Forks & Things Built on π

- [oh-my-pi](https://github.com/can1357/oh-my-pi) — The heavyweight distro: hash-anchored edits, optimized tool harness, LSP, Python, browser, subagents, and more.
- [pi-rs](https://github.com/jshachm/pi-rs) — Lightweight Rust reimplementation of pi.
- [pix-mono](https://github.com/xynogen/pix-mono) — Pix, a distro of the pi coding agent.
- [rho](https://github.com/mikeyobrien/rho) — An always-on personal agent built on pi: remembers across sessions and checks in on its own.
- [senpi](https://github.com/code-yeongyu/senpi) — Opinionated extension-first fork; the README alone is worth the click.

### The oh-my-pi Orbit

- [harness-remote](https://github.com/giuliastro/harness-remote) — Control coding-agent harnesses from phone or desktop (OMP, pi, OpenCode, Claude Code).
- [oh-my-singularity](https://github.com/DeprecatedLuke/oh-my-singularity) — Task-based orchestration TUI for highly parallel agentic development.
- [omp-deck](https://github.com/mcbarlowe/omp-deck) — Cockpit web UI: multi-session chat, kanban, cron routines, Telegram bridge.
- [t4-code](https://github.com/LycaonLLC/t4-code) — Open-source desktop app for oh-my-pi.

## Frontends

Web, desktop, mobile, and editor faces for the same agent.

- [agent-desktop](https://github.com/BaLaurent/agent-desktop) — Desktop application with native UI.
- [pi-coding-agent (Emacs)](https://github.com/dnouri/pi-coding-agent) — Emacs frontend, because of course there's an Emacs frontend.
- [pi-desktop](https://github.com/gustavonline/pi-desktop) — Native desktop shell (Tauri + Lit), extension-first and multi-session aware.
- [pi-gui](https://github.com/minghinmatthewlam/pi-gui) — Electron GUI app for the pi runtime.
- [pi-gui (VVander)](https://github.com/VVander/pi-gui) — GUI extension providing a visual interface.
- [pi-mobile](https://github.com/ayagmar/pi-mobile) — Android client with session management over Tailscale.
- [pi-vscode](https://github.com/pithings/pi-vscode) — Minimal VS Code extension.
- [pi-web](https://github.com/agegr/pi-web) — Web UI: session browsing, real-time chat, skill management, file preview.
- [pi-web (jmfederico)](https://github.com/jmfederico/pi-web) — Web UI that keeps sessions alive in real workspaces.
- [piclaw](https://github.com/rcarmo/piclaw) — "pi coding agent in a technicolor web trenchcoat."

## Extension Packs

Multi-extension collections; many of the best single ideas live inside these.

- [agent-stuff](https://github.com/mitsuhiko/agent-stuff) — Armin Ronacher's skills and extensions: answer, review, loop, todos, and more.
- [agents (michalvavra)](https://github.com/michalvavra/agents) — Includes filter-output (redact secrets from tool results) and bash command security.
- [dot314](https://github.com/w-winter/dot314) — Pi extensions. The name alone earns the entry.
- [pi-extensions (aliou)](https://github.com/aliou/pi-extensions) — Debugging and utility extensions: debug, meta, processes.
- [pi-extensions (kcosr)](https://github.com/kcosr/pi-extensions) — Includes toolwatch, a tool-call audit and approval system with SQLite logging.
- [pi-extensions (MattDevy)](https://github.com/MattDevy/pi-extensions) — Includes pi-continuous-learning for a self-improving setup.
- [pi-extensions (narumiruna)](https://github.com/narumiruna/pi-extensions) — Automation, planning, language tooling, browser control, git workflows.
- [pi-extensions (ogulcancelik)](https://github.com/ogulcancelik/pi-extensions) — Includes ghostty-theme-sync and a browser sketch pad.
- [pi-extensions (owainlewis)](https://github.com/owainlewis/pi-extensions) — Context-isolated workflow automation.
- [pi-extensions (richardgill)](https://github.com/richardgill/pi-extensions) — Files browser, skill-task routing, isolated task-tool subprocesses.
- [pi-extensions (tmustier)](https://github.com/tmustier/pi-extensions) — Delightful set: ralph-wiggum long-running loops, usage dashboard, arcade.
- [pi-hooks](https://github.com/prateekmedia/pi-hooks) — Minimal reference extensions: git checkpoint, LSP diagnostics, layered permissions.
- [pi-mono-extensions](https://github.com/emanuelcasco/pi-mono-extensions) — Collection of pi-mono extensions.
- [pi-packages](https://github.com/ben-vargas/pi-packages) — Extensions, skills, prompt templates, and themes in one repo.
- [pi-stuffed](https://github.com/raunovillberg/pi-stuffed) — Grab bag including Reddit integration.
- [rhubarb-pi](https://github.com/qualisero/rhubarb-pi) — Small delights: background-notify, session-emoji, session-color, safe-git.
- [shitty-extensions](https://github.com/hjanuschka/shitty-extensions) — Honors the original name: cost-tracker, handoff, oracle, plan-mode, ultrathink.

## Subagents & Multi-Agent

- [PiSwarm](https://github.com/lsj5031/PiSwarm) — Parallel GitHub issue/PR processing with git worktrees.
- [pi-boomerang](https://github.com/nicobailon/pi-boomerang) — Token-efficient autonomous task execution with context collapse.
- [pi-foreground-chains](https://github.com/nicobailon/pi-foreground-chains) — Multi-agent workflow orchestration with file-based handoff.
- [pi-intercom](https://github.com/nicobailon/pi-intercom) — Inter-session communication.
- [pi-messenger](https://github.com/nicobailon/pi-messenger) — Multi-agent communication between pi instances.
- [pi-side-chat](https://github.com/nicobailon/pi-side-chat) — Fork the conversation into an independent side chat while the main agent keeps working.
- [pi-subagents](https://github.com/nicobailon/pi-subagents) — Async subagent delegation with truncation, artifacts, and session sharing.
- [roach-pi](https://github.com/tmdgusya/roach-pi) — Strict engineering discipline and multi-agent orchestration.
- [task-factory](https://github.com/patleeman/task-factory) — Queue-first work orchestrator with planning, execution skills, and a web UI.

## Context, Memory & Compaction

- [pi-custom-compaction](https://github.com/nicobailon/pi-custom-compaction) — Take control of how context gets compacted.
- [pi-hermes-memory](https://github.com/chandra447/pi-hermes-memory) — Hermes-style persistent memory and learning loop.
- [pi-memory-workbench](https://github.com/nicobailon/pi-memory-workbench) — Durable, session-safe Markdown memory.
- [pi-rtk-optimizer](https://github.com/MasuRii/pi-rtk-optimizer) — Command rewriting and tool-output compaction to save tokens.

## Workflow & Autonomy

- [pi-autoresearch](https://github.com/nicobailon/pi-autoresearch) — Autonomous experiment loop.
- [pi-interactive-shell](https://github.com/nicobailon/pi-interactive-shell) — The agent drives interactive CLIs in an observable PTY overlay; you can take over anytime.
- [pi-model-switch](https://github.com/nicobailon/pi-model-switch) — Let the agent switch models on its own.
- [pi-prompt-template-model](https://github.com/nicobailon/pi-prompt-template-model) — Model/skill/thinking frontmatter in prompt templates with auto-restore.

## UI & Interaction

- [pi-annotate](https://github.com/nicobailon/pi-annotate) — Visual feedback from browser to agent: click elements, add comments, fix code.
- [pi-canvas](https://github.com/jyaunches/pi-canvas) — Interactive TUI canvases (calendar, document, flights) rendered inline.
- [pi-design-deck](https://github.com/nicobailon/pi-design-deck) — Present multi-slide design options with high-fidelity previews.
- [pi-interview-tool](https://github.com/nicobailon/pi-interview-tool) — Interactive forms with keyboard navigation, themes, and image attachments.
- [pi-powerline-footer](https://github.com/nicobailon/pi-powerline-footer) — Powerline status bar with git integration and token intelligence.
- [pi-screenshots-picker](https://github.com/Graffioh/pi-screenshots-picker) — Better screenshot selection.
- [pi-skill-palette](https://github.com/nicobailon/pi-skill-palette) — VS Code-style command palette for skills.
- [pi-super-curl](https://github.com/Graffioh/pi-super-curl) — curl requests with coding-agent superpowers.
- [pi-tool-display](https://github.com/MasuRii/pi-tool-display) — Compact tool-call rendering, diff visualization, output truncation.

## Safety & Permissions

- [pi-permission-system](https://github.com/MasuRii/pi-permission-system) — Permission enforcement extension.
- [pi-rewind-hook](https://github.com/nicobailon/pi-rewind-hook) — Rewind file changes with git-based checkpoints and conversation branching.
- [pi-ssh-remote](https://github.com/cv/pi-ssh-remote) — Redirect all file operations and commands to a remote host via SSH.

## Notifications & Chat Bridges

- [pi-discord](https://github.com/nicobailon/pi-discord) — Discord bot routing mentions, DMs, and slash commands to persistent pi sessions.
- [pi-notification-extension](https://github.com/lsj5031/pi-notification-extension) — Telegram/bell alerts when the agent finishes and waits.
- [pi-notify](https://github.com/ferologics/pi-notify) — Native desktop notifications via OSC 777.
- [pi-notify-pp](https://github.com/kim0/pi-notify-pp) — Rich notifications with tool stats and error tracking.
- [pi-telegram](https://github.com/badlogic/pi-telegram) — Telegram DM bridge from the author.

## Skills

- [pi-agent-codebase-workflows](https://github.com/PriNova/pi-agent-codebase-workflows) — Codebase reconstruction, architecture-aware review, safe changes.
- [pi-amplike](https://github.com/pasky/pi-amplike) — Replicate the AmpCode experience: handoffs, modes, permissions, web access.
- [pi-skills (badlogic)](https://github.com/badlogic/pi-skills) — The canonical collection; see [The Mothership](#the-mothership).
- [pi-skills (ferologics)](https://github.com/ferologics/pi-skills) — Personal skill collection.
- [pi-skills (PSPDFKit-labs)](https://github.com/PSPDFKit-labs/pi-skills) — Nutrient's collection of custom tools and workflows.

## Providers & Model Access

- [groq-anthropic-bridge](https://github.com/badlogic/groq-anthropic-bridge) — Anthropic-API-to-Groq/OpenAI bridge for Kimi K2 and friends.
- [meridian](https://github.com/rynfar/meridian) — Use a Claude Max subscription with pi, OpenCode, Droid, Aider, and more.
- [pi-anthropic-auth](https://github.com/gotgenes/pi-anthropic-auth) — Anthropic OAuth compatibility.
- [pi-gitlab-duo](https://github.com/badlogic/pi-gitlab-duo) — GitLab Duo provider extension.
- [pi-llama-cpp](https://github.com/gsanhueza/pi-llama-cpp) — llama.cpp integration for local models.
- [pi-synthetic](https://github.com/aliou/pi-synthetic) — Provider for Synthetic (open-source models via Anthropic-compatible API).

## MCP, ACP & Code Intelligence

- [aft](https://github.com/cortexkit/aft) — Symbol-aware edits, semantic search, fast grep/glob, PTY, background tasks (OpenCode + pi).
- [mcp-to-pi-tools](https://github.com/nicobailon/mcp-to-pi-tools) — Convert MCP servers into native pi tools.
- [pi-acp](https://github.com/svkozak/pi-acp) — ACP adapter; plug pi into Zed and other ACP clients.
- [pi-agent-scip](https://github.com/austinm911/pi-agent-scip) — SCIP code-intelligence tools.
- [pi-codeindex](https://github.com/akaza21/pi-codeindex) — Call graphs, structural search, and SCIP support for pi agents and the CLI.
- [pi-gitnexus](https://github.com/tintinweb/pi-gitnexus) — GitNexus knowledge-graph integration.
- [pi-mcp-adapter](https://github.com/nicobailon/pi-mcp-adapter) — Token-efficient MCP adapter.

## Sandboxes & Isolation

- [gondolin](https://github.com/earendil-works/gondolin) — Linux micro-VM sandbox with a TypeScript control plane, from the pi lab itself.
- [gondolin-nix](https://github.com/luizribeiro/gondolin-nix) — Gondolin configured with Nix for reproducible environments.
- [nono](https://github.com/nolabs-ai/nono) — Kernel-enforced capability sandbox (Landlock on Linux, Seatbelt on macOS).
- [pi-coding-agent-container](https://github.com/gni/pi-coding-agent-container) — Docker Compose setup.
- [pi-less-yolo](https://github.com/cjermain/pi-less-yolo) — "Slightly less YOLO": pi in a Docker container sandbox.

## Sessions, Observability & Cost

- [claude-tap](https://github.com/liaohch3/claude-tap) — Intercept and inspect agent API traffic in a local trace viewer (pi supported).
- [CodexBar](https://github.com/steipete/CodexBar) — macOS menu bar usage stats across AI coding tools.
- [pi-cost-dashboard](https://github.com/mrexodia/pi-cost-dashboard) — Interactive web dashboard for API costs.
- [pi-session-manager](https://github.com/Dwsy/pi-session-manager) — Browse, search, and resume pi sessions.
- [pi-share-hf](https://github.com/badlogic/pi-share-hf) — Collect, review, and upload redacted session files to a Hugging Face dataset.
- [pi-sub](https://github.com/marckrenn/pi-sub) — Usage-tracking extensions with a shared core and footer widget.

- [pisesh](https://github.com/Blue-B/pisesh) — Bookmark, star, rename, and resume pi sessions from a keyboard-driven TUI; switches sessions in-process via `ctx.switchSession()`.
## Review & QA

- [pi-diff-review](https://github.com/badlogic/pi-diff-review) — Diff review from the author.
- [pi-review](https://github.com/earendil-works/pi-review) — Official review extension.
- [pi-review-loop](https://github.com/earendil-works/pi-review-loop) — Persistent incremental diff-review loop.
- [pi-review-loop (nicobailon)](https://github.com/nicobailon/pi-review-loop) — Automated code-review loop extension.
- [pi-terminal-bench](https://github.com/badlogic/pi-terminal-bench) — Harbor adapter for running Terminal-Bench evaluations.

## Toys & Eye Candy

- [pi-doom](https://github.com/badlogic/pi-doom) — Play DOOM in your terminal with pi. Yes, it runs DOOM.
- [pi-dosbox](https://github.com/badlogic/pi-dosbox) — Run DOS programs with agent interaction.
- [voipi](https://github.com/badlogic/voipi) — Give your agent a voice: zero-dependency text-to-speech.

## Setups & Dotfiles

Real-world configurations worth stealing from.

- [.agents](https://github.com/ivanrvpereira/.agents) — Agent configurations and template examples.
- [dotfiles (zenobi-us)](https://github.com/zenobi-us/dotfiles) — Dotfiles with a well-tended pi setup.
- [LazyPi](https://github.com/robzolkos/LazyPi) — Pi setup for the lazy.
- [monopi](https://github.com/ifiokjr/monopi) — One-click setup: extensions, themes, prompts, skills. "Like oh-my-zsh for pi."
- [pi-config (HazAT)](https://github.com/HazAT/pi-config) — Personal configuration with skills and extensions.
- [pi-config (vtemian)](https://github.com/vtemian/pi-config) — Project config example.
- [pi-setup](https://github.com/abhinand5/pi-setup) — Personal pi setup.

## Friends of π

Cross-agent tools with explicit pi support.

- [bitrouter](https://github.com/bitrouter/bitrouter) — Model router that continuously improves agentic workflows across harnesses.
- [bug-hunter](https://github.com/codexstar69/bug-hunter) — Adversarial multi-agent bug hunter with auto-fix, pi among supported agents.
- [claude_codex_bridge](https://github.com/SeemSeam/claude_codex_bridge) — Visible multi-agent CLI workspace mixing pi with Codex, Claude, Gemini, and more.
- [codemap](https://github.com/kcosr/codemap) — Compact, token-aware codebase maps for LLMs and coding agents.
- [gob](https://github.com/juanibiapina/gob) — Process manager for AI agents with background jobs and a TUI.
- [hcom](https://github.com/aannoo/hcom) — Let agents message, watch, and spawn each other across terminals.
- [magic-context](https://github.com/cortexkit/magic-context) — Self-managing memory; "the hippocampus for coding agents."
- [mco](https://github.com/mco-org/mco) — Run selected agents and models in parallel, compare raw answers.
- [memorix](https://github.com/AVIDS2/memorix) — Cross-agent memory layer via MCP.
- [opencode-power-pack](https://github.com/waybarrios/opencode-power-pack) — 45 rigorous skills for Codex, OpenCode, and pi.

## Lore

Every good project has history; pi's is better than most.

- pi was originally **the shitty coding agent** — [shittycodingagent.ai](https://shittycodingagent.ai) still redirects to pi.dev. [shitty-extensions](https://github.com/hjanuschka/shitty-extensions) keeps the flame alive.
- The code lived at `badlogic/pi-mono` before moving to [earendil-works/pi](https://github.com/earendil-works/pi); old links redirect, old habits die harder.
- [qualisero/awesome-pi-agent](https://github.com/qualisero/awesome-pi-agent) was the first awesome list for pi. It retired in mid-2026 with the words "time to retire!" — this list picks up the torch. Respect.
- [senpi](https://github.com/code-yeongyu/senpi)'s README apologizes to the author for forking. The author does not appear to mind.
- [dot314](https://github.com/w-winter/dot314) proves the naming space is not yet exhausted. 3.141592… neither is π.

## Contributing

Found something awesome? See [CONTRIBUTING.md](CONTRIBUTING.md).
The bar: alive, documented, actually about pi, one line, alphabetical.

## License

[CC0 1.0](LICENSE) — public domain. Like π itself.
