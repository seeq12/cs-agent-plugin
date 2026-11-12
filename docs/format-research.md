# Plugin format research

Reviewed November 12, 2026.

There are host-specific manifests, not one identical Claude/Codex installation format. The reusable unit is a root `skills/<name>/SKILL.md` directory with YAML name/description and workflow instructions.

- [OpenAI packaging](https://developers.openai.com/plugins/build/plugins): root `plugin.json` for portable Agent Plugins, root `skills/`, optional `mcp.json`, and a supported `.codex-plugin/plugin.json` compatibility overlay. This scaffold uses portable identity plus the compatibility overlay; it omits inline `extensions.com.openai` so the overlay can supply skill discovery.
- [Claude manifest reference](https://code.claude.com/docs/en/plugins-reference): `.claude-plugin/plugin.json` holds metadata; skills and other components live outside that directory, at the plugin root.
- [Claude marketplaces](https://code.claude.com/docs/en/plugin-marketplaces): a repository can expose `.claude-plugin/marketplace.json`; each entry identifies a plugin source. This repo catalogs its root plugin.

Keep the three manifests' name, description, and version aligned. MCP endpoints, hooks, and executable helpers are optional; omit them until there is a concrete tested integration. Host support and authentication must be tested separately from manifest syntax.
