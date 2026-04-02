# kuicao-plugins

A Claude Code plugin marketplace by [kuicao55](https://github.com/kuicao55).

## Available Plugins

| Plugin | Description |
| ------ | ----------- |
| [claude-codex-harness](https://github.com/kuicao55/claude-codex-harness) | Structured development workflow with cross-session progress tracking, activity logging, and Generator vs. Evaluator (GvE) architecture |

## How to Use

Inside a Claude Code session:

```
/plugin marketplace add kuicao55/claude-plugins
```

Then install individual plugins:

```
/plugin install claude-codex-harness@kuicao-plugins
```

Then reload:

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
