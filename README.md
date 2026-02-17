# 🤖 AI First - Toil Tracker

A lightweight system to surface and track repetitive work that could be automated with agents.

## Where Everything Lives

All toil ideas and automation proposals are tracked as **GitHub Issues** in this repo. Bookmark these views:

| View | Link |
|------|------|
| 📋 **All toil ideas** | [View](../../issues?q=is%3Aissue+label%3Atoil) |
| 🏷️ **Needs triage** | [View](../../issues?q=is%3Aissue+label%3Atriage+is%3Aopen) |
| 🔨 **In progress** | [View](../../issues?q=is%3Aissue+label%3Ain-progress+is%3Aopen) |
| ✅ **Automated (done)** | [View](../../issues?q=is%3Aissue+label%3Aautomated) |

## How It Works

1. **Weekly Slack ping** — Every Friday at 10:00 AM PST, the team is asked: _"What toil could be automated?"_
2. **File an issue** — Use the [Toil Automation Idea](../../issues/new?template=toil-idea.md) template to log ideas
3. **Score & prioritize** — Rate ideas using the [scoring guide](docs/scoring-guide.md) and triage as a team
4. **Propose a solution** — Use the [Automation Proposal](../../issues/new?template=automation-proposal.md) template
5. **Build & ship** — Automate the toil and eliminate it for good 🎉

## Quick Links

- [📝 Submit a toil idea](../../issues/new?template=toil-idea.md)
- [🔧 Propose an automation](../../issues/new?template=automation-proposal.md)
- [📋 View all toil ideas](../../issues?q=is%3Aissue+label%3Atoil)
- [🏷️ Triage queue](../../issues?q=is%3Aissue+label%3Atriage+is%3Aopen)
- [✅ Automated (completed)](../../issues?q=is%3Aissue+label%3Aautomated)

## Documentation

| Doc | Description |
|-----|-------------|
| [Scoring Guide](docs/scoring-guide.md) | How to prioritize toil by impact |
| [Triage Workflow](docs/triage-workflow.md) | Step-by-step process for reviewing ideas |
| [Examples](docs/examples.md) | Common toil patterns to inspire your team |
| [Contributing](CONTRIBUTING.md) | How to submit ideas and build automations |
| [Security](SECURITY.md) | Security policy for automations |

## Slack Setup

Set up a weekly reminder in your team channel using Slack Workflow Builder:

1. Open Slack → **Tools** → **Workflow Builder** → **Create Workflow**
2. Trigger: **On a schedule** → Every Friday at 10:00 AM PST
3. Add step: **Send a message to a channel** (e.g. `#team-toil`)
4. Paste this message:

> 🤖 **Weekly Toil Check-in**
>
> What repetitive work are you doing that could be automated with an agent?
>
> 👉 [File it here](https://github.com/DUBSOpenHub/toil-tracker/issues/new?template=toil-idea.md) — takes 2 minutes.
>
> Not sure what counts? Check out the [examples](https://github.com/DUBSOpenHub/toil-tracker/blob/main/docs/examples.md).

## Labels

| Label | Purpose |
|-------|---------|
| `toil` | All toil ideas |
| `triage` | Needs review and prioritization |
| `high-impact` | Saves significant time or affects many people |
| `quick-win` | Could be automated quickly |
| `in-progress` | Automation is being built |
| `automated` | Toil has been eliminated 🎉 |

## Automations

This repo includes a **stale issue workflow** that:
- Nudges toil ideas with no activity after 30 days
- Auto-closes after 60 days of inactivity
- Exempts issues labeled `in-progress`, `automated`, or `high-impact`

## License

[MIT](LICENSE)
