# mjb-plugins

A Claude Code plugin marketplace maintained by Matthew Bellantoni.

## Add this marketplace

```
/plugin marketplace add mjbellantoni/cc-marketplace
```

## Install a plugin

```
/plugin install brivlo-claude@mjb-plugins
```

## Available plugins

| Plugin | Description |
|--------|-------------|
| [`brivlo-claude`](https://github.com/mjbellantoni/brivlo-claude) | [Brivlo](https://github.com/mjbellantoni/brivlo) plugin for Claude Code |

## Adding a new plugin

Add an entry to the `plugins` array in `.claude-plugin/marketplace.json`:

```json
{
  "name": "your-plugin-name",
  "source": {
    "source": "github",
    "repo": "mjbellantoni/your-plugin-repo"
  },
  "description": "Short description of the plugin"
}
```

The `name` field here must match the `name` in the plugin repo's `.claude-plugin/plugin.json`.
