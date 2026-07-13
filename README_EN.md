# 🐙 Octobao

<div align="center">
  <p><a href="./README.md">简体中文</a> · <strong>English</strong></p>

  <img src="./assets/octobao.png" alt="Octobao AI desktop pet" width="320">

  <p><strong>See what your AI is doing at a glance.</strong></p>
  <p>A local desktop octopus for AI coding agents.</p>

  <p>
    <a href="./releases/latest"><strong>Download the latest release</strong></a>
    ·
    <a href="./releases">All releases</a>
    ·
    <a href="./issues">Report an issue</a>
  </p>
</div>

> [!IMPORTANT]
> **Current status: Early Preview · Closed Source**  
> This repository is for product information, official binary distribution, and issue tracking only. It does not contain the product source code. Available platforms and implemented features are defined by each Release. If no installer is attached to a Release, only the product introduction is currently available.

## What is Octobao?

Octobao is not another chat window, and it does not replace the agents you already use.

It is a persistent visual layer for AI work. When an agent is thinking, reading files, editing code, running commands, browsing, or waiting for your input, Octobao shows the activity through expressions, motion, and task badges.

Instead of repeatedly switching windows, glance at Octobao to see whether your AI is working or waiting for you.

## Understand the status at a glance

| What Octobao shows | What the agent is doing |
|---|---|
| Thinking or reasoning | Planning or processing context |
| Searching, reading, or browsing | Finding or retrieving information |
| Editing or running | Modifying files or using tools |
| Delegating | Coordinating sub-agents or workflows |
| `your turn` | Waiting for your input, decision, or approval |
| `review` | A response is ready for you to review |
| Task badges | Multiple agents or sessions are working in parallel |

## Single-task and multi-task modes

- **Single task:** one large expression communicates the current activity directly.
- **Multiple tasks:** Octobao enters command mode, with a separate status badge for each session.
- **Busy upgrades:** as concurrent tasks increase, Octobao puts on sunglasses and eventually enters the fire-eye state.
- **High-priority signals:** waiting for you, completed replies, and errors use stronger visual cues.

> `Boost` is only a visual representation of multi-task load. It does not change model speed or agent performance.

<div align="center">
  <img src="./assets/octobao-boost-lite.gif" alt="Octobao transitioning from one task into Boost multi-agent mode" width="360">
</div>

## Agent integration status

| Agent | Current progress | Local status source |
|---|---|---|
| Claude Code | Adapter connected | CLI Hooks; local transcripts may be used as a supplementary source |
| Codex | Adapter connected | Local session / rollout data and Hook events |
| Qoder Quest | Adapter connected; installation integration in progress | Local Quest logs |
| WorkBuddy | Hook ingress connected; installation integration in progress | WorkBuddy Hooks; may require one-time user approval |

You do not need to install every agent. Octobao only uses status sources that already exist on the local machine and are disclosed for that release. Agents that are not installed remain dormant and do not create fake tasks.

## Platform and release status

| Platform | Architecture | Status |
|---|---|---|
| Windows | x64 | Transparent desktop-pet prototype implemented; public preview packages are listed in Releases |
| macOS | Apple Silicon arm64 | Planned; no public download yet |
| macOS | Intel / Universal | No release planned at this time |

The Windows prototype currently supports a transparent always-on-top window, dragging, smooth hover scaling, and persistent position and size. Standalone desktop-pet packaging, clean-machine verification, unified logging boundaries, and macOS support are still in progress.

## Download

Download Octobao only from this repository's [GitHub Releases](./releases).

1. Open Releases and select a version for your operating system and architecture.
2. Read the feature list, known issues, and data-access notes for that version.
3. Download the official installer from Release Assets and verify its published SHA-256 checksum.

> [!WARNING]
> GitHub's automatically generated `Source code (zip)` and `Source code (tar.gz)` files are not Octobao installers. If a Release has no other executable assets, no binary download is available for that version.

Do not download Octobao from third-party file-sharing services, reposted pages, or unknown mirrors. Do not use builds produced from unidentified legacy projects.

## Privacy and local processing

Octobao follows a **local-first** design. Status is extracted locally from the relevant agent's Hooks, transcript / rollout data, or logs, then aggregated and rendered on the same machine.

The public distribution follows these boundaries:

- It does not automatically upload prompt, response, or transcript content.
- It does not store prompt, response, or tool content in Octobao's status database or diagnostic logs.
- It does not automatically upload tool arguments, tool results, credentials, screenshots, or diagnostic files.
- Every Release should disclose the local data sources it uses and any known limitations.

Unified log redaction, storage rotation, and diagnostic export are still being improved for the early preview. Do not upload an entire log directory or raw session data to a public Issue. Review everything manually and attach only the minimum necessary, redacted excerpt.

## Product boundaries

The desktop-pet edition of Octobao focuses on observing and displaying agent status:

- It does not approve permissions, answer questions, or send commands to an agent for you.
- It does not bundle LCD, USB, case-display, RGB, or hardware-sensor functionality.
- It does not treat CPU, RAM, temperature, power, GPU, or fan telemetry as desktop-pet features.
- It does not represent an uninstalled agent as an active session.

## FAQ

### Is Octobao open source?

Not currently. This repository contains no product source code and is used only for product information, official binary distribution, and issue tracking.

### Must I install all four agents?

No. Each agent can be integrated independently. If its local data source is absent, that integration remains dormant.

### Does Octobao control my agents?

No. The desktop pet currently observes and displays status only. It does not take actions on behalf of the user.

### Does Octobao upload my conversations?

Not automatically. Some adapters locally parse Hooks, transcript / rollout data, or logs to determine status, but prompt, response, and tool content should not be written into Octobao's status database or diagnostic logs.

### Does Octobao require a liquid-cooling display or other hardware?

No. Only builds that remove hardware dependencies and pass standalone desktop-pet release validation will be distributed as official desktop-pet packages.

### Why is my operating system missing from Releases?

That platform has not yet passed public distribution validation. Do not download placeholder packages or unverified builds from other sources.

## Report an issue

Bug reports and feature requests are welcome through [GitHub Issues](./issues). Please include, when possible:

- Octobao version;
- operating system and architecture;
- agent being used;
- reproducible steps;
- screenshots without private information, or redacted log excerpts.

Do not publicly upload complete transcripts, session databases, raw log directories, credentials, or screenshots containing real project paths.

## Closed-source and copyright notice

Octobao is currently not open-source software.

The absence of an open-source license does not grant permission to copy, modify, or redistribute the product program, character design, animation, graphics, brand name, or official assets. You are welcome to share the official repository link. Without written permission, do not repackage or mirror the product, impersonate an official release, or use official assets in another commercial product.

If a release package includes separate license terms, those terms apply to that version. Third-party components included in a package remain subject to their respective licenses.

Claude Code, Codex, Qoder Quest, and WorkBuddy are products or trademarks of their respective owners. Octobao is an independent project and is not officially affiliated with, sponsored by, or endorsed by those products.

---

<div align="center">
  Made with 🐙 for people working with too many agents.
</div>
