# BD: Business Development Suite

AI-powered Business Development toolkit for winning freelance work

Proposal writing, portfolio creation, and past project management for Upwork

---

## Overview

The BD module is a lean, sharp Business Development toolkit for freelancers bidding on Upwork. It packages everything needed to win work — starting with proposal writing and portfolio creation, built to expand into a full BD suite over time.

BDO, your in-house Business Development Officer, knows your entire work history, applies a proven 3-line formula (What I Saw → How I'll Help → Next Step), and produces proposals under 120 words that sound like you wrote them — every time.

**The "aha!" moment:** Applying to 5 jobs, each proposal referencing the right past project, each one sounding different — in the time it used to take to write one.

---

## Installation

```bash
bmad install bd
```

---

## Quick Start

1. Install the module and configure your BD artifacts folder
2. Add your past projects: activate BDO → `[PP]` Past Projects → Add entries
3. Spot a good Upwork job → activate BDO → `[WP]` Write Proposal → paste the job description
4. Receive a tailored, ready-to-send proposal in seconds

**For detailed documentation, see [docs/](docs/).**

---

## Components

### Agents

| Agent | Name | Role |
|-------|------|------|
| 💼 BDO | BDO | Business Development Officer — proposals, portfolios, past project management |

### Workflows

| Workflow | Type | Description |
|----------|------|-------------|
| `write-proposal` | Core | Write a tailored Upwork proposal from a job posting |
| `manage-past-projects` | Core | Add, view, or update past project references |
| `write-portfolio` | Feature | Write a polished portfolio case study + image suggestions |

---

## Configuration

The module supports these configuration options (set during installation):

| Variable | Description | Default |
|----------|-------------|---------|
| `bd_artifacts` | Where proposals and portfolio pieces are stored | `{output_folder}/bd-artifacts` |

Core config variables (`user_name`, `communication_language`, `output_folder`) are available automatically.

---

## Module Structure

```
bd/
├── module.yaml
├── README.md
├── TODO.md
├── docs/
│   ├── getting-started.md
│   ├── agents.md
│   ├── workflows.md
│   └── examples.md
├── agents/
│   └── bdo.agent.yaml
└── workflows/
    ├── write-proposal/
    ├── manage-past-projects/
    └── write-portfolio/
```

---

## Documentation

For detailed user guides and documentation, see the **[docs/](docs/)** folder:
- [Getting Started](docs/getting-started.md)
- [Agents Reference](docs/agents.md)
- [Workflows Reference](docs/workflows.md)
- [Examples](docs/examples.md)

---

## Development Status

This module is currently in development. The following components are planned:

- [ ] Agents: 1 agent (BDO)
- [ ] Workflows: 3 workflows

See TODO.md for detailed status.

---

## Author

Created by Riz via BMAD Module workflow — 2026-03-01

---

## License

Part of the BMAD framework.
