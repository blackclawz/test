# blackclawz/test

Test repository for verifying GitHub App integration with OpenClaw agents.

## Purpose

This repo validates that the following agents can authenticate and perform Git operations via their GitHub App identities:

| Agent | App | Role |
|-------|-----|------|
| Oscar (Dev Agent) | `oscar-dev-agent` | Code, PRs, commits, issues |
| Melanie (PM Agent) | `melanie-pm-agent` | Issues, projects, releases |

## Setup

GitHub Apps are installed on the `blackclawz` org with installation IDs:
- Oscar-Dev-Agent: `133710238`
- Melanie-PM-Agent: `133710317`

Authentication uses RSA private keys to generate short-lived JWTs, exchanged for installation access tokens via the GitHub API.

## Status

- [x] Apps created and installed on org
- [x] Private keys configured
- [x] `gh` CLI authenticated as `oscar-dev-agent[bot]`
- [x] Test repo created
- [ ] Melanie token rotation configured
- [ ] OpenClaw skill env wired up

## Workflow Test

This commit was made on a feature branch to test the PR-required workflow.
