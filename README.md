# AI Web Dashboard
---------------------
A production-grade web application for monitoring AI systems, agents, and workflows in real time. Built as a fully self-contained single-file application — no backend or installation required.

---

## Live Demo

> After enabling GitHub Pages:
> `https://Roshini-12805.github.io/AI-web-Dashboard/ai_dashboard.html`

---

## Problem Statement

**Problem Statement 11 — AI Web Dashboard**
> Design a web application for monitoring AI systems and workflows, with real-time updates, a control panel, and documentation deliverables.

---

## Features

### Dashboard UI
- 4 live metric cards — Active Agents, Tasks Completed, Avg Latency, Error Rate
- Real-time throughput / latency / error rate line chart with tab switching
- Task distribution donut chart by agent type
- Active alerts panel with dismiss controls
- Top agents leaderboard with progress bars
- Live log feed with auto-scroll

### Real-Time Updates
- Log stream updates every 1.2 seconds
- System resource bars (CPU / Memory / GPU) update every 2.5 seconds
- Task counter increments live
- Latency simulation with realistic jitter

### AI Agent Management
- Full agent registry table (12 agents)
- Filter by status: Running / Idle / Error / Queued
- Per-agent actions: Start / Stop
- Progress bars and latency per agent

### Pipeline Monitoring
- Step-by-step workflow execution view
- Live status indicators (Done / Active / Pending)
- Execution stats panel
- Weekly pipeline run history chart
- Export pipeline as JSON

### Control Panel
- Toggle switches: Auto-scaling, Log Streaming, Anomaly Detection, Rate Limiting
- Range sliders: Max Concurrent Agents, Request Timeout, Retry Attempts
- Model selector: claude-sonnet-4-6, claude-opus-4-6, claude-haiku-4-5
- Quick action buttons: Deploy, Flush Cache, Export Logs, Health Check, Restart Workers, Emergency Stop

### API Explorer (Mock)
- 8 documented REST endpoints (GET / POST / PUT / DELETE)
- Sample JSON responses for each endpoint
- "Try it" button with simulated response + log entry

### System Architecture
- 4-layer architecture diagram: Client → API Gateway → Core Services → Data/AI
- Full technology stack breakdown
- Data flow walkthrough
- Integration status (CRM, Email, SMS, Slack, PagerDuty)

### UI Wireframes
- Annotated wireframe mockups for all 4 major screens
- Dashboard Layout (UI-01)
- Agent Management (UI-02)
- Log Stream View (UI-03)
- Control Panel (UI-04)

---

## Tech Stack

| Layer | Technology |
|---|---|
| Frontend | HTML5, CSS3, Vanilla JavaScript |
| Charts | Chart.js 4.4.1 |
| Fonts | JetBrains Mono, Syne (Google Fonts) |
| Backend | Mock API (simulated in-browser) |
| Hosting | GitHub Pages |

---

## Project Structure

```
AI-web-Dashboard/
├── ai_dashboard.html     # Complete application (single file)
└── README.md             # Project documentation
```

---

## How to Run

### Option 1 — Open directly in browser
1. Download `ai_dashboard.html`
2. Double-click the file to open it in any browser
3. No server or installation needed

### Option 2 — GitHub Pages (live URL)
1. Go to repository **Settings → Pages**
2. Set source to **main** branch, **/ (root)**
3. Click **Save**
4. Access at: `https://Roshini-12805.github.io/AI-web-Dashboard/ai_dashboard.html`

---

## Mock API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/v1/agents` | List all agents |
| POST | `/v1/agents/{id}/run` | Trigger agent task |
| GET | `/v1/metrics` | System metrics snapshot |
| GET | `/v1/logs` | Fetch recent logs |
| PUT | `/v1/config` | Update system config |
| DELETE | `/v1/agents/{id}` | Deregister an agent |
| GET | `/v1/pipelines` | List workflow pipelines |
| POST | `/v1/alerts/acknowledge` | Dismiss an alert |

---

## Deliverables Checklist

| Deliverable | Status |
|---|---|
| Dashboard UI | Done |
| Real-time updates | Done |
| Control panel | Done |
| UI Wireframes | Done (UI-01 to UI-04) |
| System Architecture diagram | Done |
| API Structure documentation | Done |

---

## Author

**Roshini-12805**
GitHub: [github.com/Roshini-12805](https://github.com/Roshini-12805)

---

## License

This project is submitted as part of a company evaluation assignment.
