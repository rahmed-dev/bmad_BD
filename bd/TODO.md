# TODO: BD: Business Development Suite

Development roadmap for the `bd` module.

---

## Agents to Build

- [ ] BDO (Business Development Officer)
  - Use: `bmad:bmb:agents:agent-builder`
  - Spec: `agents/bdo.spec.md`
  - Note: hasSidecar = true — sidecar stores past project references

---

## Workflows to Build

- [ ] write-proposal
  - Use: `bmad:bmb:workflows:workflow` or `/workflow`
  - Spec: `workflows/write-proposal/write-proposal.spec.md`
  - Note: 6 steps — gather → parse → select → write → quality check → deliver

- [ ] manage-past-projects
  - Use: `bmad:bmb:workflows:workflow` or `/workflow`
  - Spec: `workflows/manage-past-projects/manage-past-projects.spec.md`
  - Note: Tri-modal (add/edit/view) — drives the sidecar knowledge base

- [ ] write-portfolio
  - Use: `bmad:bmb:workflows:workflow` or `/workflow`
  - Spec: `workflows/write-portfolio/write-portfolio.spec.md`
  - Note: 6 steps — platform-aware output with specific image suggestions

---

## Installation Testing

- [ ] Test installation with `bmad install bd`
- [ ] Verify module.yaml prompts work correctly (`bd_artifacts` path)
- [ ] Verify BDO agent is discoverable and activates correctly
- [ ] Verify all 3 workflows are reachable from BDO's menu
- [ ] Test sidecar persistence across sessions

---

## Documentation

- [ ] Complete README.md with real usage examples once agents/workflows are built
- [ ] Enhance docs/ with troubleshooting section
- [ ] Add example proposals and portfolio pieces to docs/examples.md

---

## Future Workflows (v2+)

- [ ] `analyse-job` — Score/evaluate a job posting before committing to write a proposal
- [ ] `followup-message` — Write a follow-up message for a pending proposal
- [ ] `outreach-message` — Write cold outreach to potential clients

---

## Next Steps

1. Build BDO agent using create-agent workflow
2. Build `write-proposal` workflow (highest value — build this first)
3. Build `manage-past-projects` workflow (powers personalisation)
4. Build `write-portfolio` workflow
5. Test installation and end-to-end functionality
6. Iterate based on real use

---

_Last updated: 2026-03-01_
