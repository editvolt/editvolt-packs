# GREEN — Pack license gate

Only list Packs that pass this checklist. Re-check when bumping a source `ref`/`sha`.

## Checklist (every Pack)

- [ ] SPDX identifier known (prefer **MIT** or **Apache-2.0**)
- [ ] Source is the vendor’s official GitHub org or a clearly maintained official package
- [ ] Catalog entry does **not** copy vendor skill trees into this repo
- [ ] Thin wrappers (pattern B) only ship EditVolt manifests + `.mcp.json` pointers
- [ ] No competitor product names in Pack `name` / `description` / keywords in this repo
- [ ] No vendor logos committed here

## Featured seed (v1)

| Pack id | Pattern | Upstream / package | SPDX (upstream) | Notes |
|---------|---------|--------------------|-----------------|-------|
| `adobe-app-builder` | A | `adobe/skills` → `plugins/app-builder` | Apache-2.0 | Skills Pack |
| `huggingface-skills` | A | `huggingface/skills` (repo root) | Apache-2.0 | Hub CLI bootstrap Pack |
| `superpowers` | A | `obra/superpowers` | MIT | Agent orchestration skills |
| `compound-engineering` | A | `EveryInc/compound-engineering-plugin` | MIT | Agent orchestration skills |
| `context7` | A | `upstash/context7` → `plugins/claude/context7` | MIT | Docs lookup MCP + skills |
| `github-mcp` | B | `ghcr.io/github/github-mcp-server` | MIT | Thin MCP wrapper |
| `notion-mcp` | B | `@notionhq/notion-mcp-server` | MIT | Thin MCP wrapper |
| `datadog-mcp` | B | Datadog remote MCP URL | Apache-2.0 (vendor product) | Thin URL MCP wrapper |
| `google-gcloud` | B | `@google-cloud/gcloud-mcp` | Apache-2.0 | Thin MCP wrapper |
| `cloudflare-mcp` | B | `@cloudflare/mcp-server-cloudflare` | Apache-2.0 | Thin MCP wrapper |

## Blocked (do not list)

- Host-proprietary or unclear-license bundles
- Unofficial scrapes of vendor skills
- Entries that require mirroring third-party source into this repository
