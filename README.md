<!-- BlackRoad SEO Enhanced -->

# agent dashuoard

> Part of **[BlackRoad OS](https://blackroad.io)** — Sovereign Computing for Everyone

[![BlackRoad OS](https://img.shields.io/badge/BlackRoad-OS-ff1d6c?style=for-the-badge)](https://blackroad.io)
[![BlackRoad Agents](https://img.shields.io/badge/Org-BlackRoad-Agents-2979ff?style=for-the-badge)](https://github.com/BlackRoad-Agents)
[![License](https://img.shields.io/badge/License-Proprietary-f5a623?style=for-the-badge)](LICENSE)

**agent dashuoard** is part of the **BlackRoad OS** ecosystem — a sovereign, distributed operating system built on edge computing, local AI, and mesh networking by **BlackRoad OS, Inc.**

## About BlackRoad OS

BlackRoad OS is a sovereign computing platform that runs AI locally on your own hardware. No cloud dependencies. No API keys. No surveillance. Built by [BlackRoad OS, Inc.](https://github.com/BlackRoad-OS-Inc), a Delaware C-Corp founded in 2025.

### Key Features
- **Local AI** — Run LLMs on Raspberry Pi, Hailo-8, and commodity hardware
- **Mesh Networking** — WireGuard VPN, NATS pub/sub, peer-to-peer communication
- **Edge Computing** — 52 TOPS of AI acceleration across a Pi fleet
- **Self-Hosted Everything** — Git, DNS, storage, CI/CD, chat — all sovereign
- **Zero Cloud Dependencies** — Your data stays on your hardware

### The BlackRoad Ecosystem
| Organization | Focus |
|---|---|
| [BlackRoad OS](https://github.com/BlackRoad-OS) | Core platform and applications |
| [BlackRoad OS, Inc.](https://github.com/BlackRoad-OS-Inc) | Corporate and enterprise |
| [BlackRoad AI](https://github.com/BlackRoad-AI) | Artificial intelligence and ML |
| [BlackRoad Hardware](https://github.com/BlackRoad-Hardware) | Edge hardware and IoT |
| [BlackRoad Security](https://github.com/BlackRoad-Security) | Cybersecurity and auditing |
| [BlackRoad Quantum](https://github.com/BlackRoad-Quantum) | Quantum computing research |
| [BlackRoad Agents](https://github.com/BlackRoad-Agents) | Autonomous AI agents |
| [BlackRoad Network](https://github.com/BlackRoad-Network) | Mesh and distributed networking |
| [BlackRoad Education](https://github.com/BlackRoad-Education) | Learning and tutoring platforms |
| [BlackRoad Labs](https://github.com/BlackRoad-Labs) | Research and experiments |
| [BlackRoad Cloud](https://github.com/BlackRoad-Cloud) | Self-hosted cloud infrastructure |
| [BlackRoad Forge](https://github.com/BlackRoad-Forge) | Developer tools and utilities |

### Links
- **Website**: [blackroad.io](https://blackroad.io)
- **Documentation**: [docs.blackroad.io](https://docs.blackroad.io)
- **Chat**: [chat.blackroad.io](https://chat.blackroad.io)
- **Search**: [search.blackroad.io](https://search.blackroad.io)

---


Real-time agent monitoring dashboard for BlackRoad OS.

## What This Is

A single-file HTML dashboard that displays the status of all 12 BlackRoad agents in a dark-themed grid. Fetches live data from the stats worker endpoint. Shows agent name, status, message count, last active time, and group membership. Auto-refreshes every 30 seconds. Falls back to cached state if the endpoint is unreachable.

## Usage

Open `index.html` in any browser. No build step, no dependencies, no server required.

```bash
# Local
open index.html

# Or serve it
python3 -m http.server 8080
# Then visit http://localhost:8080
```

## Data Source

Fetches from `https://stats-blackroad.blackroad.workers.dev/live` for real-time agent data. If the endpoint is down, the dashboard shows all 12 agents in standby mode with a warning banner.

## Features

- Dark theme (#0a0a0a background, white/gray text only)
- Brand colors used only for decorative dots and group tags (shapes, not text)
- Responsive grid layout (adapts to any screen size)
- Summary bar showing online count, total messages, group count
- Per-agent cards with status indicator, message count, last active
- Group labels: core (blue), fleet (pink), specialist (violet)
- Live pulse animation on the connection indicator
- 30-second auto-refresh with timestamp display

## Agents Shown

12 agents across 3 groups: core (road, coder, scholar), fleet (alice, cecilia, octavia, lucidia, aria), specialist (pascal, writer, tutor, cipher).

Part of BlackRoad-Agents. Remember the Road. Pave Tomorrow. Incorporated 2025.
