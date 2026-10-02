# Ballet Ops Playbooks

Signed webhooks, scheduled digests and issue triage with retries and observability. One click into Ballet.

Built for platform, DevOps and internal-tools engineers. Every template here imports into [Ballet](https://ballet.dev), the agent operations platform for building, running and observing deterministic workflows, with one click.

[![Validate](https://github.com/brainfish-ai/ballet-ops-playbooks/actions/workflows/validate.yml/badge.svg)](https://github.com/brainfish-ai/ballet-ops-playbooks/actions/workflows/validate.yml)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

## Templates

<!-- templates:start -->

### Ops

| Template | What it does | Trigger | Import |
|---|---|---|---|
| [Daily API Digest to Slack](templates/daily-api-digest-slack) | Pull records from any JSON API, summarise them, and post a digest to Slack on a schedule. | Manual run, or attach a daily schedule in Studio | [Import](https://app.ballet.dev/import?repo=brainfish-ai/ballet-ops-playbooks&path=templates/daily-api-digest-slack&ref=main) |
| [Generic Webhook Relay](templates/generic-webhook-relay) | Verify any signed incoming webhook, reshape it, and forward it to a downstream service with retries. | Generic HMAC webhook | [Import](https://app.ballet.dev/import?repo=brainfish-ai/ballet-ops-playbooks&path=templates/generic-webhook-relay&ref=main) |
| [GitHub Issue Triage](templates/github-issue-triage) | Label every newly opened GitHub issue with an LLM through a signed webhook. | GitHub webhook (issues) | [Import](https://app.ballet.dev/import?repo=brainfish-ai/ballet-ops-playbooks&path=templates/github-issue-triage&ref=main) |

<!-- templates:end -->

## How import works

1. Click **Import** next to a template.
2. Sign in or create a Ballet workspace. Ballet fetches the template from this repository, pinned to an exact commit.
3. Review the steps and code on the preview screen, then confirm.
4. Add the listed secrets and publish.

Imported playbooks always start unpublished with triggers off, and secrets are never part of a template.

## More templates

This repository is one focused slice of [brainfish-ai/ballet-templates](https://github.com/brainfish-ai/ballet-templates), which holds every Ballet template. Other collections:

- [ballet-support-playbooks](https://github.com/brainfish-ai/ballet-support-playbooks): Support triage, summaries and reply drafting for Zendesk, Freshdesk and more. One click into Ballet.
- [ballet-sales-playbooks](https://github.com/brainfish-ai/ballet-sales-playbooks): Lead enrichment, scoring and Slack alerts for Salesforce and web forms. One click into Ballet.
- [ballet-mcp-playbooks](https://github.com/brainfish-ai/ballet-mcp-playbooks): Agent workflows that call MCP servers such as Linear and Slack. One click into Ballet.

## Contributing

This repository is generated from [brainfish-ai/ballet-templates](https://github.com/brainfish-ai/ballet-templates). Please open template pull requests there so every collection stays in sync. Issues are welcome here.

## License

[MIT](LICENSE)
