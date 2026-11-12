---
name: cs-setup
description: Check Customer Success plugin readiness, verify approved connections, and identify missing access before using account workflows.
---

Inspect the tools available in the current agent session. Read [connection guidance](../../references/connections.md) for the proposed sources and access checks, and [the evidence contract](../../references/evidence-and-connections.md) before retrieving customer information.

Report available connections, verified access, and gaps separately. When requested, use one bounded read-only lookup to verify a relevant connection. An installed connector alone is not proof of access to an account or permission to share its data.

Match the user's task to an installed workflow: account-brief, success-plan, account-handoff, account-recovery, adoption-impact, renewal-review, or customer-retrospective. Verify the required source access before describing a workflow as ready to run.

Keep credentials in the host's authentication flow. Installation does not authorize customer-data publication, messages, record changes, or recurring jobs. Finish with the smallest next setup step needed for the user's intended workflow.
