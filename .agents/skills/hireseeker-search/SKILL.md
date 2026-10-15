---
name: hireseeker-search
description: >
  Find and read public HireSeeker job listings through existing web-search and
  page-fetch tools. Use when the user selects HireSeeker. Loads the canonical
  instructions without configuring services or installing packages.
enabled: false
---

# HireSeeker Portable Entry Point

Read and follow [the canonical HireSeeker skill](../../../.claude/skills/hireseeker/SKILL.md)
before searching. From the repository root, that file is
`.claude/skills/hireseeker/SKILL.md`. It defines public-page discovery, candidate
preferences, verification, source policies, and handoff to `/apply`.

This pointer makes the same instructions discoverable in Codex and Antigravity.
Claude Code uses the canonical `/hireseeker` skill directly.

`enabled: false` excludes this standalone web-search skill from the repository's
`/scrape` CLI loop. Direct HireSeeker searches remain available. No Bun portal
CLI or portal health probe is provided.
