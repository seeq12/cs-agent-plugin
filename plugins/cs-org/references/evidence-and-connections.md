# Evidence and connections

## Connect once per user

Use the client's existing approved connectors or MCP servers. Discover their available operations before assuming a tool name or capability. Configure and authenticate connections through the client or organization administrator; this plugin ships no servers or credentials.

| Need | Typical source | Check |
|---|---|---|
| Account identity, ownership, contract, renewal | Salesforce or approved CRM | Match account ID and parent/site scope; verify dates and record freshness. |
| Account discussions and action tracking | Slack or meeting notes | Read linked threads; distinguish suggestions from accepted commitments. |
| Templates, playbooks, account history | Glean or document search | Read underlying documents; verify generated summaries against their sources. |
| Usage, adoption, health | Power BI, approved read-only warehouse, Mixpanel | Inspect metric definitions, filters, coverage, and refresh time. |
| Customer issues | Jira or support system | Confirm account association, status, severity, and customer impact. |

When a connection is missing, use supplied exports or documents and name the coverage gap. Ask for the smallest missing input that changes the answer. Never invent endpoints, metric formulas, access, or a successful query. Follow the organization's approved data-access method; use read-only operations for research.

## Evidence contract

- Resolve ambiguous customer names, subsidiaries, sites, time zones, and analysis periods before combining data.
- Attach source links and an as-of date to material claims. For queries, include metric definition, period, filters, source refresh date, and enough query detail to reproduce a disputed number without exposing credentials or raw personal data.
- Label observed facts, reported statements, hypotheses, and recommendations. Preserve source conflicts and explain scope or definition differences instead of silently choosing a convenient number.
- Treat missing data as unknown. Zero requires evidence of a complete, empty measurement. Distinguish users, active users, paid users, and licensed users; inspect the actual business definitions.
- Separate measured business outcomes from activity and estimated benefits. Avoid causal claims from a before/after comparison alone.
- Return only information appropriate for the audience. Keep internal risk notes and personal details out of customer-facing material unless sharing is authorized.
- Draft proposed actions with owners and dates marked proposed when unconfirmed. Send messages, create tasks, or update shared artifacts only within the user's explicit request and existing permissions. Account-specific requests do not authorize portfolio-wide changes or scheduled monitoring.
- When updating an existing plan or handoff, preserve its stable link and human edits. If a write fails, return the draft and report the actual outcome.

Public contributions contain reusable methods and synthetic examples only. Keep customer records, private links, internal schemas, exports, and secrets in authorized private systems.
