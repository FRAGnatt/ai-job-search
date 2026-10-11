---
name: hireseeker
description: >
  Search IT and digital vacancies on HireSeeker via public MCP or the official
  CLI, especially for Russian-speaking candidates targeting Russia, the CIS,
  or international employers. Use for requests such as "find jobs on HireSeeker"
  or "show remote Python vacancies". Loads the canonical search instructions.
enabled: false
---

# HireSeeker Portable Entry Point

Read and follow [the canonical HireSeeker skill](../../../.claude/skills/hireseeker/SKILL.md)
before searching. From the repository root, that file is
`.claude/skills/hireseeker/SKILL.md`. It defines MCP access, official CLI commands,
live catalog selection, supported filters, result handling, and recommendations
for Russian-speaking candidates.

This entry point makes the same instructions discoverable in Codex and
Antigravity without maintaining a second workflow. Claude Code uses the canonical
`/hireseeker` skill directly.

`enabled: false` controls inclusion in this repository's `/scrape` portal loop;
it does not prevent directly requested HireSeeker searches. This integration has
no Bun portal CLI and is excluded from `/scrape` and its portal health probes.
