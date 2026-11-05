# Changelog

## 1.0.0 — 2026-11-05

First release as its own repository. This code started as a rewrite of [feedback-agent](https://github.com/ericzakariasson/feedback-agent), which stays the in-app feedback widget.

### Added

- Slack bot (`bot/`) on `@grok/agent-sdk@0.6.0`: native Slack channel, `slack-communication` tools and the `cursor-cloud-agents` extension
- `launch_fix_agent`: one cloud agent per Slack thread that reproduces the bug, fixes it, opens a PR and records a demo video
- `fetch_demo_video`: downloads the agent's demo video from the Cursor artifacts API so the bot posts it in the thread
- Triage evals under `evals/`
- `demo-app/`, an invoicing app with a seeded invoice-rename bug, as the default target, with `AGENTS.md` for cloud agents
- Untrusted-input hard rules, redaction of emails and credentials, one run per report, feedback id in the PR
