# CS Organization Plugin

Shared customer success skills for Claude Code and Codex.

**Skills:** setup and connection checks, account briefs, success plans, handoffs, recovery plans, adoption impact, renewal reviews, and customer retrospectives.

**Claude Code:** `/plugin marketplace add seeq12/cs-agent-plugin`, then `/plugin install cs-org@cs-organization`.

**Codex:** add `seeq12/cs-agent-plugin` in Plugins → Add plugin marketplace, then install **cs-org**. CLI: `codex plugin marketplace add seeq12/cs-agent-plugin`.

Ask: “Use account-brief for this customer.” Claude also supports `/cs-org:account-brief`.

Connect your approved Glean, Slack, CRM, and analytics tools separately. Installation grants no data access. See [connections and evidence](plugins/cs-org/references/evidence-and-connections.md) and [packaging](docs/packaging.md).

## Contribute

Propose a small change with an example request and expected output. Use synthetic fixtures to check citations, freshness, calculations, and missing-access behavior. Open draft PRs and keep them draft until the repository owner explicitly approves readiness for review. Never merge automatically.

This is the canonical repository for the CS Organization plugin. The original setup scaffold's history and connection guidance have been consolidated here. Shared methods and synthetic examples belong in this public package; customer data, credentials, internal transcripts, and private templates stay in authorized private systems.
