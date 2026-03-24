# agent-dashboard

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
