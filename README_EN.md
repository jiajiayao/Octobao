# 🐙 Octobao

<div align="center">
  <p><a href="./README.md">简体中文</a> · <strong>English</strong></p>

  <img src="./assets/octobao.png" alt="Octobao AI desktop pet" width="320">

  <p><strong>See what your AI is doing at a glance.</strong></p>
  <p>A transparent desktop octopus that turns AI coding-agent activity into visible status.</p>

  <p>
    <a href="https://github.com/jiajiayao/Octobao/releases/tag/v0.1.0-early-preview.1"><strong>Download the Windows preview</strong></a>
    ·
    <a href="https://github.com/jiajiayao/Octobao/releases">All releases</a>
    ·
    <a href="https://github.com/jiajiayao/Octobao/issues">Report an issue</a>
  </p>
</div>

> [!IMPORTANT]
> **Early Preview · Windows x64 · Unsigned · Closed Source**<br>
> The current preview is not code-signed, so Windows may show an “Unknown publisher” warning. Download it only from this repository's Releases and read the release notes before installing.

## What does Octobao do?

Octobao is not a chat window and it does not operate an agent for you. It turns background work into desktop status you can understand at a glance:

- **Is it still working?** A sleeping Octobao means there is no active task; an awake Octobao means an agent is doing something.
- **What is it doing?** Thinking, searching, reading, editing, running commands, and browsing all have distinct expressions and animations.
- **Does it need me?** `your turn` asks for your input, choice, or approval; `review` means a response is ready.
- **Are several tasks active?** Multiple agents or sessions appear as separate task badges, so you do not have to check every window.

Start working in an agent you already use and Octobao wakes automatically. It does not take over another chat window, and it does not require a liquid-cooling display or any other hardware.

## Status guide

The status text at the bottom, Octobao's expression, and the symbol near its upper-right side change together:

| Status text | What you will see | What it means |
|---|---|---|
| `idle` | Closed eyes and slowly drifting sleep bubbles | The agent is online but has no active task |
| `offline` | A grey sleeping state | No usable agent status is currently available |
| `thinking` / `reasoning` | Dots light up inside a thought bubble | Planning, reasoning, or understanding context |
| `processing` | Several dots converge toward the centre | Organising tool results before the next step |
| `searching` | A magnifier sweeps back and forth | Searching code, files, or local resources |
| `reading` | Pages move inside an open book | Reading files or reference material |
| `editing` | A pencil writes while tentacles type | Modifying code, documents, or other files |
| `running` | A small terminal and rotating progress arc | Running commands, tests, builds, or tools |
| `browsing` | A globe with an orbiting light | Using the web, a browser, or computer-use tools |
| `delegating` | Task nodes orbit a central coordinator | Assigning subtasks or coordinating agents |
| `responding` | Two flowing rings rotate independently | Generating and displaying a response |
| `compacting` | Curved brackets squeeze inward | Organising a long context window |
| `your turn` | A question mark and an alert expression | Waiting for your input, choice, confirmation, or approval |
| `review` | A smile and a check mark | The agent has replied and the result is ready to review |
| `error` | A warning symbol and error expression | A tool, request, or task has failed |

While work is active, the bottom row may also show:

- `TOK`: the current task's token count; a leading `~` means it is an estimate.
- `RUN`: how long the current task has been running.

Different agents expose different information, so some numbers may be absent. The status animations still work without them.

## What happens with multiple tasks?

When several agents, sessions, or subtasks are active, Octobao enters multi-task command mode:

- The main Octobao stays visually stable instead of changing expression for every small task transition.
- Each badge above it represents one task and can independently show thinking, reading, editing, running, or waiting.
- When there are more tasks than visible badge slots, `+N` shows how many remain.
- By default, Octobao puts on sunglasses at 4 busy tasks and enters the fire-eye state at 8.

> `Boost` is a playful visualization of parallel task load. It does not make a model or agent run faster.

<div align="center">
  <img src="./assets/octobao-boost-lite.gif" alt="Octobao moving from one task into multi-task Boost mode" width="360">
</div>

## Everyday controls

- **Move:** hold and drag Octobao anywhere on the desktop.
- **Resize:** hover over Octobao, then drag the resize area that appears near the upper-right corner.
- **Automatic memory:** position and size are restored the next time Octobao starts.
- **Right-click menu:** reset size and position, open the log folder, or exit the desktop pet.
- **Start at sign-in:** the installer starts Octobao when the current Windows user signs in.
- **Transparent and always on top:** Octobao floats above other windows without a separate console or settings window.

## Supported agents

| Agent | Current preview status |
|---|---|
| Claude Code | Supported |
| Codex | Supported |
| Qoder Quest | Early support; setup experience is still being improved |
| WorkBuddy | Early support; first-time setup may require Hook confirmation |

You do not need every agent. Octobao shows only agents and sessions that actually exist on this computer; an agent that is not installed does not create fake tasks.

## Platforms and downloads

| Platform | Current status |
|---|---|
| Windows x64 | Early Preview available |
| macOS Apple Silicon | Planned; no public installer yet |
| macOS Intel / Universal | No release planned at this time |

Download Octobao only from [GitHub Releases](https://github.com/jiajiayao/Octobao/releases):

1. Most users should choose `Octobao-Windows-x64-Setup-unsigned.exe`.
2. The portable ZIP is intended for manual testing and does not provide installation, sign-in startup, or a Start menu entry.
3. The current build is unsigned, so Windows may display a security warning during installation.
4. To verify the files, use `SHA256SUMS-unsigned.txt` from the Release Assets.

> [!WARNING]
> GitHub's automatically generated `Source code (zip)` and `Source code (tar.gz)` files are not Octobao installers. Do not download Octobao from third-party file-sharing sites, reposted pages, or unknown mirrors.

## Privacy and local processing

Octobao is **local-first**: status is read, interpreted, and displayed on your computer.

- It does not automatically upload prompts, responses, conversation content, tool arguments, or tool results.
- It does not automatically upload credentials, screenshots, logs, or diagnostic files.
- It does not approve permissions, answer questions, or send commands to an agent for you.
- Local diagnostic logs are for troubleshooting only. When reporting an issue, attach only the minimum necessary, redacted excerpt.

## FAQ

### Does Octobao require a liquid-cooling display or other hardware?

No. This is a standalone Windows desktop pet. It does not include LCD, USB, RGB, sensor, or hardware-monitoring features.

### Must I install all four agents?

No. You can use only one. Agents that are not installed remain dormant.

### Does Octobao control my agents?

No. Octobao currently observes and displays status only. All input, permissions, and decisions remain with you.

### Is Octobao open source?

Not currently. This repository is for product information, official binary distribution, and issue tracking; it does not contain the product source code.

## Report an issue

Bug reports and suggestions are welcome through [GitHub Issues](https://github.com/jiajiayao/Octobao/issues). When possible, include your Octobao version, Windows version, agent, reproduction steps, and a screenshot without private information or a redacted log excerpt.

Do not publicly upload complete conversations, raw log directories, credentials, or screenshots containing real project paths.

## Copyright notice

Octobao is currently not open-source software. Without written permission, do not repackage or mirror the product, impersonate an official release, or copy the program, character design, animations, graphics, or brand assets into another commercial product. Third-party components included in a release remain subject to their respective licenses.

Claude Code, Codex, Qoder Quest, and WorkBuddy are products or trademarks of their respective owners. Octobao is an independent project and is not officially affiliated with, sponsored by, or endorsed by those products.

---

<div align="center">
  Made with 🐙 for people working with too many agents.
</div>
