# Examples of Common Toil

Not sure what counts as toil? Here are real-world examples to inspire your team.

## Development & CI/CD

| Toil | Automation Idea |
|------|-----------------|
| Manually running tests before merging | GitHub Actions CI pipeline |
| Copy-pasting release notes from PRs | Auto-generate release notes from PR titles/labels |
| Updating version numbers across files | Version bump script or semantic-release |
| Manually creating release branches | GitHub Action triggered on tag push |
| Checking if dependencies are up to date | Dependabot or Renovate |

## Operations & Infrastructure

| Toil | Automation Idea |
|------|-----------------|
| Rotating on-call schedules manually | PagerDuty/OpsGenie integration or script |
| Restarting services after known failures | Auto-restart with health checks |
| Manually scaling resources | Auto-scaling policies |
| Copying logs to a shared location | Centralized logging pipeline |

## Communication & Reporting

| Toil | Automation Idea |
|------|-----------------|
| Writing weekly status updates | Agent that summarizes merged PRs and closed issues |
| Notifying stakeholders of deployments | Slack bot triggered by deploy events |
| Updating project trackers after standups | GitHub Project automation rules |
| Sending reminders for recurring meetings | Slack scheduled messages or workflows |

## Code Review & Quality

| Toil | Automation Idea |
|------|-----------------|
| Checking for common code patterns | Custom linter rules |
| Verifying PR descriptions are complete | GitHub Action that checks PR template fields |
| Assigning reviewers manually | CODEOWNERS file + auto-assign action |
| Checking for secrets in code | Secret scanning / pre-commit hooks |

## Onboarding & Documentation

| Toil | Automation Idea |
|------|-----------------|
| Setting up dev environments for new hires | Dev container or setup script |
| Keeping API docs in sync with code | Auto-generate docs from OpenAPI spec |
| Answering the same onboarding questions | FAQ bot or knowledge base |
| Granting access to repos/tools one by one | Onboarding automation script |

---

💡 **Tip:** If you find yourself saying _"I do this every week"_ or _"I wish this just happened automatically"_ — that's toil. File it!
