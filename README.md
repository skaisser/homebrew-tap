<div align="center">

# Homebrew Tap — Blueprint SDLC

**Install the [Blueprint](https://github.com/skaisser/blueprint) CLI via Homebrew.**

[![GitHub Release](https://img.shields.io/github/v/release/skaisser/blueprint?label=version)](https://github.com/skaisser/blueprint/releases)
[![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](LICENSE)
[![Homebrew](https://img.shields.io/badge/homebrew-tap-orange)](https://github.com/skaisser/homebrew-tap)

</div>

---

## Install

```bash
brew tap skaisser/tap
brew install blueprint
```

## Update

```bash
brew upgrade blueprint
```

## Verify

```bash
blueprint version
```

## What is Blueprint?

Blueprint turns [Claude Code](https://docs.anthropic.com/en/docs/claude-code) into a disciplined engineering team. One CLI, 27 slash commands, 15 audit rules — from idea to merged PR.

```
/backlog → /plan → /plan-review → /plan-approved → /plan-check → /pr → /review → /address-pr → /finish
```

### CLI Commands

| Command | What it does |
|---------|-------------|
| `blueprint audit` | 15-rule enforcement engine (runs on every tool call) |
| `blueprint status` | Show SDLC status — plan, branch, progress |
| `blueprint meta` | Plan metadata as JSON |
| `blueprint update` | Self-update from GitHub Releases |
| `blueprint sync` | Sync plan frontmatter with task counts |
| `blueprint commit` | Validated commit with emoji format |
| `blueprint backlog` | Manage backlog items |
| `blueprint context` | Git context for PR generation |

### Also Available As

- **Claude Code Plugin** (recommended): `/plugin marketplace add skaisser/blueprint-plugin`
- **Manual install**: `curl -fsSL https://raw.githubusercontent.com/skaisser/blueprint/main/install.sh | bash`

## Platforms

| OS | Architecture | Supported |
|----|-------------|-----------|
| macOS | Apple Silicon (arm64) | Yes |
| macOS | Intel (amd64) | Yes |
| Linux | x86_64 (amd64) | Yes |

## How This Tap Works

This tap is **auto-updated** by [GoReleaser](https://goreleaser.com/) whenever a new version of Blueprint is released. The formula in `Formula/blueprint.rb` is generated automatically — do not edit it manually.

## Links

- [Blueprint — Main Repo](https://github.com/skaisser/blueprint) — source code, development, contributing
- [Blueprint — Claude Code Plugin](https://github.com/skaisser/blueprint-plugin) — install via Claude Code plugin system
- [Releases](https://github.com/skaisser/blueprint/releases) — all versions and changelogs

## License

Apache 2.0 — see [LICENSE](LICENSE)
