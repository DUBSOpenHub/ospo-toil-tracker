# 🤖 Toil Tracker

A lightweight system to surface and track repetitive work that could be automated with agents.

## How It Works

1. **Weekly Slack ping** — Every Friday, the team is asked: _"What toil could be automated?"_
2. **File an issue** — Use the [Toil Automation Idea](../../issues/new?template=toil-idea.md) template to log ideas
3. **Prioritize** — The team reviews and prioritizes ideas by impact and frequency
4. **Automate** — Build agents to eliminate the highest-impact toil

## Quick Links

- [📝 Submit a toil idea](../../issues/new?template=toil-idea.md)
- [📋 View all toil ideas](../../issues?q=is%3Aissue+label%3Atoil)
- [🏷️ Triage queue](../../issues?q=is%3Aissue+label%3Atriage+is%3Aopen)

## Slack Setup

Set up a weekly reminder in your team channel using Slack Workflow Builder:

1. Open Slack → **Tools** → **Workflow Builder** → **Create Workflow**
2. Trigger: **On a schedule** → Every Friday at 9:00 AM
3. Add step: **Send a message to a channel** (e.g. `#team-toil`)
4. Paste this message:

> 🤖 **Weekly Toil Check-in**
>
> What repetitive work are you doing that could be automated with an agent?
>
> Reply in-thread with what the toil is, how often it happens, and how long it takes.
> Then file it 👉 [Submit a toil idea](https://github.com/DUBSOpenHub/toil-tracker/issues/new?template=toil-idea.md)

## Labels

| Label | Purpose |
|-------|---------|
| `toil` | All toil ideas |
| `triage` | Needs review and prioritization |
| `high-impact` | Saves significant time or affects many people |
| `quick-win` | Could be automated quickly |
| `in-progress` | Automation is being built |
| `automated` | Toil has been eliminated 🎉 |
