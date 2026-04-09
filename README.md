# kuicao-plugins

A Claude Code plugin marketplace by [kuicao55](https://github.com/kuicao55).

## Available Plugins

| Plugin name | Marketplace | Description |
| ----------- | ----------- | ----------- |
| `super-harness` | `kuicao-plugins` | Structured development workflow with pre-flight checks, Orchestrator/Executor/Reviewer architecture, cross-session milestone tracking, activity logging, TDD process enforcement, and dual-engine Codex integration (v3.2.3) — [repo](https://github.com/kuicao55/super-harness) |

## How to Install

**Step 1 — Add this marketplace** (one-time, inside a Claude Code session):

```
/plugin marketplace add kuicao55/claude-plugins
```

**Step 2 — Browse plugins** (optional, opens the UI):

```
/plugin
```

Go to the **Discover** tab to browse all available plugins.

**Step 3 — Install a plugin:**

```
/plugin install super-harness@kuicao-plugins
```

> Format: `/plugin install <plugin name>@<marketplace name>`

**Step 4 — Reload:**

```
/reload-plugins
```

## Adding More Plugins

To add a new plugin to this marketplace, add an entry to `.claude-plugin/marketplace.json`:

```json
{
  "name": "your-plugin-name",
  "source": {
    "source": "github",
    "repo": "kuicao55/your-plugin-repo"
  },
  "description": "...",
  "version": "1.0.0",
  "author": { "name": "kuicao55" },
  "homepage": "https://github.com/kuicao55/your-plugin-repo",
  "repository": "https://github.com/kuicao55/your-plugin-repo",
  "license": "MIT"
}
```
