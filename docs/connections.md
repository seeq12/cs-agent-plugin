# Connection plan

These are proposed integration categories, not bundled servers or verified access. Users authenticate through their agent host with their own approved accounts.

| Source | Intended use | First access check |
| --- | --- | --- |
| Enterprise knowledge search, such as Glean | Find current playbooks, enablement assets, and account evidence | Read one known authorized document and return its source link |
| Slack | Read relevant account discussions and locate shared plans | Read a user-specified thread; verify its audience before sharing derived content |
| CRM, such as Salesforce | Resolve account identity, ownership, and opportunities | Resolve a known account without changing records |
| Product analytics and approved warehouse access | Usage trends and consistent business definitions | Inspect the approved metric definition and run a bounded read-only aggregate |
| Jira and GitHub | Track proposed work and review plugin changes | Read a known issue or repository |

Add a root MCP configuration only after endpoint, transport, authentication, and host support are verified. Portable Agent Plugins use `mcp.json`; Claude and Codex compatibility packages use `.mcp.json`. Their schemas differ, so create and validate each deliberately rather than renaming a file.

Record source, access scope, data freshness, and calculation limits in outputs. Request authorization appropriate to the task before external writes or scheduling. A personal plugin does not inherit a deployed bot's service-account permissions or delivery authority.
