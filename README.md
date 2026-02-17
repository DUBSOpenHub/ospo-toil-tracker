# 🤖 AI First - Toil Tracker

**Stop doing repetitive work. Start automating it.**

Every team has toil - the manual, repetitive tasks that eat up time and could be handled by an agent or script. This repo gives your team a simple, ready-to-use system to surface that toil, track it, and eliminate it.

> 💡 **This is for any team.** Fork it, set up a weekly Slack reminder, and start collecting ideas in under 10 minutes. No code required.

---

## 🍴 Get Started (Any Team)

1. **[Fork this repo](../../fork)** - you get everything: issue templates, labels, workflows, scoring guides, and docs
2. **Enable GitHub Actions** - go to the **Actions** tab in your fork and click **"I understand my workflows, go ahead and enable them"**
3. **Update two URLs** - in the [Slack Setup](#slack-setup) section, replace `<YOUR_ORG>/<YOUR_REPO>` with your fork's path. Also update the Slack channel link in `.github/ISSUE_TEMPLATE/config.yml`
4. **Create a Slack reminder** - follow the [3-step Slack setup](#slack-setup) to ping your team every Friday
5. **Start collecting ideas** - your team clicks the link, fills out a 2-minute form, done

That's it. Your team now has a living backlog of automation opportunities.

---

## Where Everything Lives

All toil ideas and automation proposals are tracked as **GitHub Issues** in this repo. Bookmark these views:

| View | Link |
|------|------|
| 📋 **All toil ideas** | [View](../../issues?q=is%3Aissue+label%3Atoil+sort%3Acreated-desc) |
| 🏷️ **Needs triage** | [View](../../issues?q=is%3Aissue+label%3Atriage+is%3Aopen+sort%3Acreated-desc) |
| 🔨 **In progress** | [View](../../issues?q=is%3Aissue+label%3Ain-progress+is%3Aopen+sort%3Acreated-desc) |
| ✅ **Automated (done)** | [View](../../issues?q=is%3Aissue+label%3Aautomated+sort%3Acreated-desc) |
| 🎉 **Wins & time saved** | [View](../../issues?q=is%3Aissue+%22%5BWIN%5D%22+label%3Aautomated+sort%3Acreated-desc) |

> **Tip:** Each issue shows the submitter's name, frequency (🔴🟠🟡🔵⚪), time cost, and who's affected - all visible in the issue body. Sort by newest, most commented, or filter by label to find what matters most.

## How It Works

1. **Weekly Slack ping** - Every Friday at 10:00 AM PST, the team is asked: _"What toil could be automated?"_
2. **File an issue** - Use the [Toil Automation Idea](../../issues/new?template=toil-idea.yml) template to log ideas
3. **Score & prioritize** - Rate ideas using the [scoring guide](docs/scoring-guide.md) and triage as a team
4. **Propose a solution** - Use the [Automation Proposal](../../issues/new?template=automation-proposal.md) template
5. **Build & ship** - Automate the toil and eliminate it for good
6. **Log the win** - Use the [Log Completed Automation](../../issues/new?template=log-win.yml) template to record time saved 🎉

## Quick Links

- [📝 Submit a toil idea](../../issues/new?template=toil-idea.yml)
- [🔧 Propose an automation](../../issues/new?template=automation-proposal.md)
- [📋 View all toil ideas](../../issues?q=is%3Aissue+label%3Atoil)
- [🏷️ Triage queue](../../issues?q=is%3Aissue+label%3Atriage+is%3Aopen)
- [✅ Automated (completed)](../../issues?q=is%3Aissue+label%3Aautomated)
- [🎉 Log a win](../../issues/new?template=log-win.yml)

## Documentation

| Doc | Description |
|-----|-------------|
| [Scoring Guide](docs/scoring-guide.md) | How to prioritize toil by impact |
| [Triage Workflow](docs/triage-workflow.md) | Step-by-step process for reviewing ideas |
| [ROI Tracking](docs/roi-tracking.md) | Measure and share time saved |
| [Examples](docs/examples.md) | Common toil patterns to inspire your team |
| [Contributing](CONTRIBUTING.md) | How to submit ideas and build automations |
| [Code of Conduct](CODE_OF_CONDUCT.md) | Community standards |
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
> 👉 File it here: `https://github.com/<YOUR_ORG>/<YOUR_REPO>/issues/new?template=toil-idea.yml` - takes 2 minutes.
>
> Not sure what counts? Check out the examples in the repo's `docs/examples.md`.

> ⚠️ **Replace** `<YOUR_ORG>/<YOUR_REPO>` with your actual repo path (e.g. `DUBSOpenHub/ai-first-toil-tracker`).

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

---

## 🐙 Built with Love

Made with 💜 by DUBSOpenHub to help more people discover the joy of GitHub Copilot CLI.

Happy learning! 🚀✨
