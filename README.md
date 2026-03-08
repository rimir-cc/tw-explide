# explide

Interactive testcase composition IDE for TiddlyWiki. Create config tiddlers that assemble plugins, shadow tiddlers, and ad-hoc content into isolated `$testcase` sandboxes — all from within the wiki.

## Key features

- **Config-driven** — each config tiddler (`rri.type: explide/config`) defines a complete testcase sandbox
- **Plugin import** — import entire plugins or individual shadow tiddlers, with bulk import from filter
- **Explide data** — override imported shadow tiddlers with editable copies using `$rri$:` field remapping
- **Field editor** — add, edit, and delete `$rri$:` remapped fields via the FIELDS tab
- **Ad-hoc tiddlers** — create text-only tiddlers inline without separate files
- **Snapshot & diff** — take snapshots of explide data, compare changes, and restore previous states
- **Diagnostics** — detect missing plugins, unused imports, and stale snapshots
- **Layout toggle** — switch between stacked and side-by-side view
- **Output tiddler** — configurable which tiddler the testcase Output tab displays (defaults to `Output`)
- **ViewTemplate integration** — config tiddlers automatically render the IDE when viewed

## Prerequisites

- `$:/plugins/rimir/theme` — CSS utility classes
- `$:/plugins/rimir/components` — tabs and UI components
- `$:/plugins/kookma/shiraz` — slider macro and UI utilities

## Quick start

1. Create a new tiddler
2. Set the field `rri.type` to `explide/config`
3. Save — the IDE appears automatically in the tiddler view
4. Use the CONFIG tab to import plugins and select shadow tiddlers
5. Create an ad-hoc tiddler named `Output` in the ADHOC tab — this is what the testcase renders
6. Click on explide data tabs to edit overridden tiddlers in EDITOR, manage fields in FIELDS, or compare in DIFF

## Bundled examples

- `$:/plugins/rimir/explide/examples/callout-sandbox` — theme callout types
- `$:/plugins/rimir/explide/examples/mini-app` — counter app with state management
- `$:/plugins/rimir/explide/examples/component-lab` — pills facade components

## License

MIT
