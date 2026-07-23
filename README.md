# EditVolt Packs

Curated **Pack** catalog for [EditVolt](https://github.com/editvolt). A Pack can include skills, rules, subagents, hooks, and MCP server definitions that install into EditVolt.

## How installs work

- EditVolt reads [`.editvolt-pack/marketplace.json`](.editvolt-pack/marketplace.json).
- **Get** clones the Pack’s declared Git source (upstream repo or a thin wrapper in this catalog).
- This repo does **not** mirror vendor skill or MCP source trees. Upstream Packs keep their own licenses (see [GREEN.md](GREEN.md)).
- The MIT [LICENSE](LICENSE) here covers EditVolt-authored files only (manifests, thin wrappers, docs).

## Catalog entry patterns

| Pattern | What we ship | Example |
|---------|----------------|---------|
| **A — Upstream Pack** | Catalog entry points at a GitHub repo/path that already has a Pack/plugin manifest | Adobe App Builder via `adobe/skills` |
| **B — Thin wrapper** | Folder under `packs/<id>/` with `.editvolt-pack/pack.json` + `.mcp.json` only | GitHub MCP, Notion MCP |

## Layout

```text
.editvolt-pack/marketplace.json   # Pack index
GREEN.md                          # SPDX / license gate for listed Packs
packs/<id>/                       # EditVolt-owned thin wrappers (MIT)
  .editvolt-pack/pack.json
  .mcp.json
```

## Adding a Pack

1. Confirm SPDX license is acceptable (prefer MIT or Apache-2.0). Document in `GREEN.md`.
2. Prefer pattern A when the upstream already publishes a discoverable manifest.
3. Otherwise add a pattern B wrapper — **no copied vendor skills**.
4. Add a `plugins[]` entry with `name`, `description`, `category`, `keywords`, and `source`.

## Categories

Featured · Infrastructure · Data & Analytics · Productivity · Payments · Agent Orchestration

Cards are text-only (no vendor logos).
