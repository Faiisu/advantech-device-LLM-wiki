# LLM-Wiki — Advantech ARK Series Knowledge Base

A persistent, LLM-maintained knowledge base for Advantech ARK industrial and edge PCs. Built on the LLM Wiki pattern: raw sources go in, structured wiki pages come out.

## What's in here

**21 ARK models documented** across 6 product lines:

| Series | Models | Type |
|---|---|---|
| ARK-6000 | ARK-6322 | Fanless box PC |
| ARK-1000/1100 | ARK-10, ARK-11, ARK-1123x, ARK-1124x, ARK-1125x | Compact & DIN-rail box PCs |
| ARK-1200 | ARK-1220F, ARK-1220L, ARK-1221L, ARK-1250L | Wide DIN-rail PCs |
| ARK-1500 | ARK-1551 | Slim wall-mount PC |
| ARK-3000 | ARK-3520L, ARK-3532x, ARK-3534x | Expansion box PCs (fanless) |
| ARK-7000 | ARK-7060 | Extreme performance box PC (fan-cooled) |

Each model has a structured source page covering CPU, memory, storage, I/O, operating temperature, certifications, and connections to related models.

## Structure

```
LLM-wiki/
├── CLAUDE.md        — wiki-agent operating manual (schema, workflows, rules)
├── hotcache.md      — rolling session summary (~500 words); read first
├── index.md         — flat catalog of all 52 wiki pages
├── log.md           — append-only history of all wiki activity
├── raw/             — original source documents (read-only)
└── wiki/
    ├── sources/     — one page per ingested source (21 ARK models)
    ├── entities/    — processors, organisations (14 pages)
    ├── concepts/    — standards, form factors, interfaces (11 pages)
    └── synthesis/   — comparison tables, sub-series hubs (6 pages)
```

## How to use

This wiki is operated by Claude (via `CLAUDE.md` instructions). Typical operations:

- **Ingest** — drop a spec sheet into `raw/` and say "ingest"
- **Query** — ask any question about the ARK series; the agent reads the wiki and answers
- **Lint** — say "lint the wiki" for a health check (orphan pages, broken links, stale data)

## Key synthesis pages

- [Advantech ARK Series Comparison](wiki/synthesis/advantech-ark-series-comparison.md) — master table of all 21 models with CPU, COM, CAN, temp, RAM, form factor
- [ARK-1123x hub](wiki/synthesis/ARK-1123x.md), [ARK-1124x](wiki/synthesis/ARK-1124x.md), [ARK-1125x](wiki/synthesis/ARK-1125x.md) — sub-series comparison guides
- [ARK-3532x hub](wiki/synthesis/ARK-3532x.md), [ARK-3534x](wiki/synthesis/ARK-3534x.md) — ARK-3000 sub-series guides
