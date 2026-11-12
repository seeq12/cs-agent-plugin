# CS Customer Success Plugin

A common foundation for people using their own Claude or Codex agents: shared skills, connection guidance, installation, and working principles reviewed in GitHub.

**Initial scaffold:** one setup skill is included. Account research, metrics, plans, and presentations below are proposed work, not implemented capabilities. No live connections or automatic jobs are bundled.

## Structure

```text
plugin.json                         Portable Agent Plugins identity
.claude-plugin/plugin.json          Claude Code manifest
.claude-plugin/marketplace.json     Claude Code installation catalog
.codex-plugin/plugin.json           Codex compatibility manifest
skills/cs-setup/SKILL.md             Shared setup skill
docs/connections.md                 Connection plan and access checks
docs/proposed-contents.md           Suggested first workflows
docs/format-research.md             Format decisions and official sources
```

Keep skills at the plugin root so both hosts can reuse them. Add MCP configuration, scripts, hooks, or assets only when a workflow needs them.

## Try it

Claude Code:

```sh
claude plugin marketplace add seeq12/cs-customer-success-plugin
claude plugin install cs-customer-success@cs-customer-success-marketplace
```

Then ask Claude to use `cs-setup`. For a local development preview, clone this repo and run `claude --plugin-dir /absolute/path/to/cs-customer-success-plugin`.

Codex: this repo includes the documented compatibility manifest and shared skills. Follow the [official local plugin packaging workflow](https://developers.openai.com/plugins/build/plugins) for the installed Codex surface. Marketplace registration and authentication vary by host; end-to-end Codex installation has not yet been tested. This GitHub publication is not a listing in either vendor's public plugin directory.

## Contribute

Propose a small change with an example request and expected output. Use synthetic fixtures to test citations, freshness, calculations, and handling of missing access. Open draft PRs; keep them draft until the repository owner explicitly approves readiness for review. Never merge automatically. Review and version shared principles alongside skills.

Keep this public repository limited to generic instructions and synthetic examples. Retrieve account information through each user's authorized connections at runtime. Credentials, customer records, internal transcripts, and private templates belong outside the package.
