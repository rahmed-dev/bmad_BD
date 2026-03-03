# bdo-sidecar

This folder stores persistent memory for the **BDO** (Business Development Officer) agent.

## Purpose

BDO's sidecar is his knowledge base — everything he knows about your past projects
lives here. The richer this data, the more personalised and effective every proposal becomes.

## Files

| File | Purpose |
|------|---------|
| `memories.md` | Past project entries — the knowledge base BDO draws on for every proposal |
| `instructions.md` | BDO's operating protocols, quality standards, and confidence signal rules |

## Runtime Access

After BMAD installation, this folder is accessible at:
`{project-root}/_bmad/_memory/bdo-sidecar/`

BDO loads `memories.md` and `instructions.md` on every activation via `critical_actions`.

## Growing the Knowledge Base

Add projects via **[PP] Past Projects → Add** from BDO's menu.
The more specific and quantified the entries, the stronger BDO's proposals become.
