# claude-plugins

WayLit's Claude Code plugin marketplace.

## Install

From inside Claude Code:

```
/plugin marketplace add satya-waylit/claude-plugins
```

Then install any listed plugin, for example:

```
/plugin install impasse
```

## Plugins

- **[impasse](https://github.com/satya-waylit/impasse)** — an independent second opinion on any
  high-stakes artifact (a decision, an essay, a research claim, a dataset, or code) from a
  cross-provider AI reviewer, verified and reconciled before anything reaches you.

## Maintaining

Each entry in [`.claude-plugin/marketplace.json`](.claude-plugin/marketplace.json) pins its
plugin repo by commit `sha`. There is no auto-tracking — after a release in a plugin's own repo,
update its `sha` here (and `version`, if the plugin bumped one) so `/plugin install` and
`/plugin update` pick up the change.
