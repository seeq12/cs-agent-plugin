# CS Organization Plugin

Shared customer success skills for Claude Code and Codex.

**Skills:** account briefs, success plans, handoffs, recovery plans, adoption impact, renewal reviews, and customer retrospectives.

**Claude Code:** `/plugin marketplace add seeq12/cs-agent-plugin`, then `/plugin install cs-org@cs-organization`.

**Codex:** add `seeq12/cs-agent-plugin` in Plugins → Add plugin marketplace, then install **cs-org**. CLI: `codex plugin marketplace add seeq12/cs-agent-plugin`.

Ask: “Use account-brief for this customer.” Claude also supports `/cs-org:account-brief`.

Connect your approved Glean, Slack, CRM, and analytics tools separately. Installation grants no data access. See [connections and evidence](plugins/cs-org/references/evidence-and-connections.md) and [packaging](docs/packaging.md).
