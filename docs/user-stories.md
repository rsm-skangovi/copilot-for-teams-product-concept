# Analytics & Metrics

This concept uses a small telemetry model to answer a few core questions:

- Who is using Copilot, and where?
- How often are AI suggestions accepted vs rejected?
- How does AI-touched code behave in tests and security scans?

## Example Metrics

- Active Copilot users (weekly, by team and repo)
- AI suggestion acceptance rate
- % of PRs with AI-generated changes
- Test coverage delta on AI-touched files (vs. baseline)
- Security / lint issues per 1k LOC on AI-touched code

## Sample Telemetry Schema

See [`data/sample-telemetry.csv`](../data/sample-telemetry.csv) for a tiny
mock dataset that could power a prototype dashboard.

Columns:

- `date`
- `team`
- `repo`
- `ai_suggestions`
- `ai_acceptances`
- `ai_loc_changed`
- `tests_passed`
- `tests_failed`
- `security_incidents`
