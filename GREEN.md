# GREEN — Pack license gate

Only list Packs that pass this checklist. Re-check when bumping a source `ref`/`sha`.

## Checklist (every Pack)

- [ ] SPDX identifier known (prefer **MIT** or **Apache-2.0**)
- [ ] Source is the vendor’s official GitHub org or a clearly maintained official package
- [ ] Catalog entry does **not** copy vendor skill trees into this repo
- [ ] Thin wrappers (pattern B) only ship EditVolt manifests + `.mcp.json` pointers
- [ ] No competitor product names in Pack `name` / `description` / keywords in this repo
- [ ] No vendor logos committed here

## Featured + Adobe seed

| Pack id | Pattern | Upstream / package | SPDX (upstream) | Notes |
|---------|---------|--------------------|-----------------|-------|
| `adobe-app-builder` | A | `adobe/skills` → `plugins/app-builder` | Apache-2.0 | Skills Pack |
| `adobe-stardust` | A | `adobe/skills` → `plugins/stardust` | Apache-2.0 | Design redesign flow |
| `adobe-web` | A | `adobe/skills` → `plugins/web` | Apache-2.0 | Browser / web analysis |
| `adobe-aem-eds` | A | `adobe/skills` → `plugins/aem/edge-delivery-services` | Apache-2.0 | AEM EDS |
| `adobe-aem-cloud-service` | A | `adobe/skills` → `plugins/aem/cloud-service` | Apache-2.0 | AEMaaCS |
| `adobe-aem-6-5-lts` | A | `adobe/skills` → `plugins/aem/6.5-lts` | Apache-2.0 | AEM 6.5 LTS |
| `adobe-aem-project-management` | A | `adobe/skills` → `plugins/aem/project-management` | Apache-2.0 | EDS PM |
| `adobe-aem-eds-content-ops` | A | `adobe/skills` → `plugins/aem/edge-delivery-services-content-ops` | Apache-2.0 | Content ops |
| `adobe-analytics` | A | `adobe/skills` → `plugins/adobe-analytics` | Apache-2.0 | Analytics + MCP auth |
| `adobe-cja` | A | `adobe/skills` → `plugins/adobe-cja` | Apache-2.0 | CJA + MCP auth |
| `adobe-commerce-app-management` | A | `adobe/skills` → `plugins/commerce/app-management` | Apache-2.0 | Commerce |
| `adobe-commerce-app-migration` | A | `adobe/skills` → `plugins/commerce/app-migration` | Apache-2.0 | Commerce migrate |
| `adobe-for-creativity` | A | `adobe/skills` → `plugins/creative-cloud/adobe-for-creativity` | Apache-2.0 | Creative Cloud |
| `huggingface-skills` | A | `huggingface/skills` (repo root) | Apache-2.0 | Hub CLI bootstrap Pack |
| `superpowers` | A | `obra/superpowers` | MIT | Agent orchestration skills |
| `compound-engineering` | A | `EveryInc/compound-engineering-plugin` | MIT | Agent orchestration skills |
| `context7` | A | `upstash/context7` → `plugins/claude/context7` | MIT | Docs lookup MCP + skills |
| `github-mcp` | B | `ghcr.io/github/github-mcp-server` | MIT | Thin MCP wrapper |
| `notion-mcp` | B | `@notionhq/notion-mcp-server` | MIT | Thin MCP wrapper |
| `datadog-mcp` | B | Datadog remote MCP URL | Apache-2.0 (vendor product) | Thin URL MCP wrapper |
| `google-gcloud` | B | `@google-cloud/gcloud-mcp` | Apache-2.0 | Thin MCP wrapper |
| `cloudflare-mcp` | B | `@cloudflare/mcp-server-cloudflare` | Apache-2.0 | Thin MCP wrapper |

Adobe Packs are **pattern A**: catalog entries only. Source trees stay in `adobe/skills` (repo license Apache-2.0).

## Blocked (do not list)

- Host-proprietary or unclear-license bundles
- Unofficial scrapes of vendor skills
- Entries that require mirroring third-party source into this repository
