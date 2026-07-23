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
| `postgres-mcp` | B | `@modelcontextprotocol/server-postgres` | MIT | Data & Analytics |
| `google-gcloud` | B | `@google-cloud/gcloud-mcp` | Apache-2.0 | Thin MCP wrapper |
| `cloudflare-mcp` | B | `@cloudflare/mcp-server-cloudflare` | Apache-2.0 | Thin MCP wrapper |
| `playwright-mcp` | B | `@playwright/mcp` (`microsoft/playwright-mcp`) | Apache-2.0 | Browser automation MCP |
| `browserbase-mcp` | B | `@browserbasehq/mcp` | Apache-2.0 | Cloud browser MCP |
| `stripe-mcp` | B | `@stripe/mcp` | MIT | Payments |
| `shopify-dev-mcp` | B | `@shopify/dev-mcp` | ISC | Payments / commerce (permissive ISC) |
| `linear-mcp` | B | `https://mcp.linear.app/mcp` | MIT (remote product) | Productivity |
| `figma-mcp` | B | `https://mcp.figma.com/mcp` | Apache-2.0 (remote product) | Productivity |
| `atlassian-mcp` | B | `https://mcp.atlassian.com/v1/mcp` | Apache-2.0 | Productivity |
| `supabase-mcp` | B | `@supabase/mcp-server-supabase` | Apache-2.0 | Productivity |
| `neon-mcp` | B | `@neondatabase/mcp-server-neon` | MIT | Productivity |
| `firecrawl-mcp` | B | `firecrawl-mcp` | MIT | Productivity |
| `brave-search-mcp` | B | `@brave/brave-search-mcp-server` | MIT | Productivity |
| `hubspot-mcp` | B | `@hubspot/mcp-server` | MIT | Productivity |

Adobe Packs are **pattern A**: catalog entries only. Source trees stay in `adobe/skills` (repo license Apache-2.0).

Productivity / Payments v0.3 wrappers are **pattern B**: EditVolt-owned `.editvolt-pack` + `.mcp.json` only.

## Blocked (do not list)

- Host-proprietary or unclear-license bundles
- Unofficial scrapes of vendor skills
- Entries that require mirroring third-party source into this repository
