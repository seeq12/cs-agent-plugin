# Packaging

One marketplace distributes one plugin. Both clients share `plugins/cs-org/skills/<name>/SKILL.md`.

- `.agents/plugins/marketplace.json`: Codex catalog.
- `.claude-plugin/marketplace.json`: Claude Code catalog.
- `plugins/cs-org/plugin.json`: portable plugin manifest.
- `plugins/cs-org/.claude-plugin/plugin.json`: Claude compatibility metadata; keep identity and version aligned.
- `plugins/cs-org/references/`: shared evidence contract and connection checks used by `cs-setup`.

This is a skills-only plugin. MCP servers supply live tools; hooks run lifecycle actions; neither is needed to distribute these workflows. Existing authenticated connections are used at runtime. Organization-specific connection URLs and credentials stay outside this public repository.

Validate with `claude plugin validate . --strict` and `claude plugin validate ./plugins/cs-org --strict`. Each skill uses YAML `name` and `description` frontmatter followed by workflow instructions. Releases must keep both manifests aligned.

Official references, checked November 12, 2026: [OpenAI packaging](https://developers.openai.com/plugins/build/plugins), [Claude plugin reference](https://code.claude.com/docs/en/plugins-reference), [Claude marketplaces](https://code.claude.com/docs/en/plugin-marketplaces), [Claude MCP](https://code.claude.com/docs/en/mcp).

Manifest and link checks validate packaging only; installation and authentication must also be checked separately in each host.
