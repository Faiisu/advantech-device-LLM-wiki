# Wiki Log

> Append-only chronological record of all wiki activity. Never modify past entries.
> Parse tip: `grep "^## \[" log.md | tail -10` returns the last 10 entries.

---

## [2026-04-16] schema-update | Initial Setup

- Action: Initialized wiki vault with full schema
- Folder structure created: `raw/`, `raw/assets/`, `wiki/sources/`, `wiki/entities/`, `wiki/concepts/`, `wiki/synthesis/`
- Files created: `CLAUDE.md` (v1.0), `index.md`, `log.md`
- Pages created: none (wiki is empty)
- Pages updated: none
- Notes: First session. Wiki-agent is operational. Awaiting first source ingest.

---

## [2026-04-16] ingest | Attention Is All You Need

- Action: Ingested `raw/attention-is-all-you-need.md` (Vaswani et al., 2017)
- Pages created: `wiki/sources/attention-is-all-you-need.md`, `wiki/concepts/Transformer Architecture.md`, `wiki/concepts/Self-Attention.md`, `wiki/concepts/Multi-Head Attention.md`, `wiki/concepts/Positional Encoding.md`, `wiki/entities/Ashish Vaswani.md`, `wiki/entities/Google Brain.md`
- Pages updated: `index.md` (7 entries added)
- Contradictions found: none (first source)
- Open questions flagged: quadratic attention scaling, sparse/linear attention variants, BERT/GPT divergence from original encoder-decoder design

---

## [2026-04-16] schema-update | Hotcache system added (v1.1)

- Action: Created `hotcache.md` and updated `CLAUDE.md` to v1.1
- Files created: `hotcache.md` (current session summary, ~500 words)
- Files updated: `CLAUDE.md` — added Hotcache section with read-first rule and update protocol; folder structure diagram updated
- Rationale: Hotcache allows the agent to answer questions from recent context without reading index.md or multiple wiki files, reducing overhead on repeated queries within a session

---

## [2026-04-16] ingest | ARK-6322

- Action: Ingested `raw/ARK-6322.md` (Advantech product spec sheet)
- Pages created: `wiki/sources/ARK-6322.md`, `wiki/entities/Advantech.md`, `wiki/entities/Intel Celeron J1900.md`, `wiki/concepts/Fanless Embedded PC.md`, `wiki/concepts/Industrial I⁄O.md`, `wiki/concepts/iDoor.md`, `wiki/concepts/Mini PCIe.md`
- Pages updated: `index.md` (7 new entries added, total 14 pages)
- Contradictions found: none
- Open questions flagged: intended deployment use case unknown; OS choice (Windows vs Linux) unknown; significance of 6x COM ports unclear; RED certification relevance unknown; mSATA/WWAN mutual exclusivity on Mini PCIe slot 1 may be a constraint depending on project

---

## [2026-04-16] ingest | ARK-1000/1200/1500 Series (14 files)

- Action: Batch-ingested 14 Advantech ARK spec sheets from `raw/`
- Source files: ARK-10, ARK-11, ARK-1123C, ARK-1123H, ARK-1123L, ARK-1124C, ARK-1124H, ARK-1125C, ARK-1125H, ARK-1220F, ARK-1220L, ARK-1221L, ARK-1250L, ARK-1551
- Note: ARK-1123C and ARK-1123L had no spec content (cookie wall only) — created stubs; re-ingest needed
- Pages created (sources): ARK-10, ARK-11, ARK-1123H, ARK-1123C-stub, ARK-1123L-stub, ARK-1124C, ARK-1124H, ARK-1125C, ARK-1125H, ARK-1220F, ARK-1220L, ARK-1221L, ARK-1250L, ARK-1551
- Pages created (entities): Intel Atom E3825, Intel Celeron N3350, Intel Atom E3940, Intel Atom x6413E, Intel Atom x7211E, Intel N200, Intel Core i5-1145G7E, Intel Core i5-8365UE
- Pages created (concepts): DIN-Rail Mounting, CAN Bus, Isolated I/O, DeviceOn, SUSIAccess, IEC 62443
- Pages created (synthesis): advantech-ark-series-comparison (master comparison table)
- Pages updated: Advantech (entity — full product line table added)
- Index updated: 44 total pages
- Contradictions found: none
- Open questions flagged: ARK-1123C/L need re-ingest; CAN Bus version unspecified across all models; WISE-PaaS vs DeviceOn naming inconsistency across generations; iDoor module compatibility matrix missing; ARK-1220F power consumption TBD

---

## [2026-04-16] schema-update | CLAUDE.md v1.3 — Split index into indexs/ directory

- Action: Restructured index system into `indexs/` directory with separate topic files
- Files created: `indexs/main.md`, `indexs/sources.md`, `indexs/sources-ark1000.md`, `indexs/entities.md`, `indexs/concepts.md`, `indexs/synthesis.md`
- Files updated: `index.md` (vault root) — replaced with redirect stub pointing to `indexs/main.md`
- Files updated: `CLAUDE.md` v1.3 — Index Maintenance section rewritten to document `indexs/` structure, section file table, chained sub-index naming convention (`parent-child.md`), breadcrumb navigation rule
- Structure: `main.md` is entry point; section files cover sources/entities/concepts/synthesis; `sources-ark1000.md` is first chained sub-index; new sub-indexes follow `[parent]-[child].md` naming

---

## [2026-04-16] schema-update | CLAUDE.md v1.2 — Index template and sub-series hub rules

- Action: Updated `CLAUDE.md` to v1.2
- Changes: Replaced flat "Index Maintenance" section with full index template, grouping rules, and sub-series hub page pattern
- New sections added: Index Template (full markdown template), Index Grouping Rules (sources/entities/concepts), Sub-series Hub Pages (when to create, required content, link wiring, naming)
- Rationale: Codifies the grouped index structure and knowledge-graph hub pattern established this session so future ingests follow the same conventions automatically

---

## [2026-04-16] schema-update | Knowledge graph sub-series hubs + index restructure

- Action: Added sub-series hub pages and restructured index for navigability
- Pages created: `wiki/synthesis/ARK-1123x.md`, `wiki/synthesis/ARK-1124x.md`, `wiki/synthesis/ARK-1125x.md`
- Pages updated: `wiki/sources/ARK-1123H.md`, `ARK-1123C.md`, `ARK-1123L.md`, `ARK-1124C.md`, `ARK-1124H.md`, `ARK-1125C.md`, `ARK-1125H.md` — `Sub-series:` link added to each
- Pages updated: `index.md` — Sources section restructured with series/sub-series grouping + inline tables; hub page links added above each sub-series table; Entities grouped by CPU generation; Concepts grouped by domain; total updated to 47
- Rationale: Enables knowledge-graph traversal: index → sub-series hub → individual model page (and back). Each ARK-112Xx/ARK-112x source page now links up to its hub.

---

## [2026-04-16] ingest | ARK-1123C and ARK-1123L (PDF datasheets)

- Action: Replaced stubs with full source pages from official Advantech PDF datasheets
- Source files: `raw/ARK-1123C.pdf`, `raw/ARK-1123L.pdf`
- Pages updated (promoted from stub): `wiki/sources/ARK-1123C.md`, `wiki/sources/ARK-1123L.md`
- Pages updated: `wiki/entities/Intel Atom E3825.md` (full specs added: 1.33 GHz, DDR3L 1066MHz, -30~70°C)
- Pages updated: `wiki/synthesis/advantech-ark-series-comparison.md` (ARK-1123C/L rows added, timeline updated)
- Pages updated: `index.md` (stub entries replaced with full descriptions)
- Contradictions resolved: "palm-size" stub label was incorrect — ARK-1123L is same 133.8×43.1×94.2mm as ARK-1123H
- Key finding: E3825 achieves -30~70°C (wider than J1900's -20~60°C in ARK-1123H) despite older/lower-spec CPU
- Key finding: ARK-1123L is FCC Class A only (industrial) vs ARK-1123C Class B (residential+industrial) — important deployment constraint
- Open questions resolved: dimensions, temp range, power consumption, EMC class all now known

---

## [2026-04-16] schema-update | CLAUDE.md v2.1 — Filename rules; rename Industrial IO and Isolated IO

- Action: Added Obsidian filename rules to CLAUDE.md; renamed two concept files; fixed all broken wikilinks
- Files renamed: `Industrial I⁄O.md` → `Industrial IO.md`, `Isolated I-O.md` → `Isolated IO.md`
- Files updated (wikilinks): index.md + 30 wiki files — replaced `[[Industrial I-O]]`, `[[Industrial I/O]]`, `[[Isolated I/O]]`, `[[Isolated I-O]]` with `[[Industrial IO]]` and `[[Isolated IO]]`
- CLAUDE.md v2.1: added Obsidian filename rules block — no `/` in names, IO not I/O, allowed vs forbidden characters
- Root cause: `Industrial I⁄O.md` used Unicode fraction slash (U+2044); most wikilinks used `[[Industrial I-O]]` (hyphen) → all links were broken

---

## [2026-04-16] schema-update | CLAUDE.md v2.0 — Roll back to flat index.md, remove indexs/ directory

- Action: Removed `indexs/` directory (7 files); rebuilt flat `index.md`; rewrote `CLAUDE.md` to follow original LLM Wiki pattern
- Files deleted: `indexs/main.md`, `indexs/sources.md`, `indexs/sources-ark1000.md`, `indexs/sources-ark3000.md`, `indexs/entities.md`, `indexs/concepts.md`, `indexs/synthesis.md`, `index.md` (redirect stub)
- Files created: `index.md` (new flat catalog, 56 pages)
- Files updated: `CLAUDE.md` v2.0 — simpler schema following original LLM Wiki document; single `index.md`; hotcache rules preserved; no split index complexity
- Rationale: The split `indexs/` structure added maintenance overhead and complexity beyond what the pattern requires. A single flat `index.md` is sufficient.

---

## [2026-04-16] schema-update | CLAUDE.md v1.4 — Remove index.md, point directly to indexs/main.md

- Action: Deleted `index.md` (redirect stub) from vault root; updated all references in CLAUDE.md
- Files deleted: `index.md`
- Files updated: `CLAUDE.md` v1.4 — 9 occurrences of `index.md` replaced with `indexs/main.md` or `indexs/` as appropriate; folder structure diagram updated; redirect stub note removed from Index Maintenance section
- Rationale: `index.md` was a 6-line stub that only pointed to `indexs/main.md`; CLAUDE.md already told the agent where to look, making the stub redundant

---

## [2026-04-16] ingest | ARK-3000 Series (5 files)

- Action: Ingested 5 Advantech ARK-3000 spec sheets from `raw/ark-3000series/`
- Source files: ARK-3520L, ARK-3532B, ARK-3532C, ARK-3534C, ARK-3534D
- Pages created (sources): `wiki/sources/ARK-3520L.md`, `ARK-3532B.md`, `ARK-3532C.md`, `ARK-3534C.md`, `ARK-3534D.md`
- Pages created (entities): `Intel 6th Gen Core (Skylake-H).md`, `Intel 10th Gen Xeon W (Comet Lake-S).md`, `Intel 12th-14th Gen Core (Raptor Lake LGA1700).md`
- Pages created (synthesis): `ARK-3532x.md` (hub: B vs C), `ARK-3534x.md` (hub: C vs D)
- Pages created (index): `indexs/sources-ark3000.md` (chained sub-index)
- Pages updated: `Advantech.md` (ARK-3000 product line + CPU table + related entities), `advantech-ark-series-comparison.md` (5 new rows + selection tables + timeline), `CAN Bus.md` (ARK-3534C/D added), `IEC 62443.md` (ARK-3534C/D added), `Fanless Embedded PC.md` (expansion box tier added)
- Index updated: `sources.md` (ARK-3000 section), `entities.md` (ARK-3000 tier section), `synthesis.md` (ARK-3532x/3534x hubs), `main.md` (counts: 21 sources, 15 entities, 6 synthesis, 57 total)
- Contradictions found: none
- Key finding: ARK-3000 is a fundamentally different tier — expansion box PC with PCIe x16 GPU slots and 45–65W desktop CPUs vs 5–10W SoCs in ARK-1000/1200
- Key finding: ARK-3532B is first ECC-capable model; ARK-3532B + ARK-3534D support ECC memory (not available in any ARK-1000/1200/1500 model)
- Key finding: ARK-3534C/D spec sheets are incomplete — no operating temp or power consumption listed
- Open questions flagged: ARK-3534C/D operating temperature unconfirmed; CAN Bus version (2.0A/B/FD) still unknown across all models; ARK-3532C certification status unclear; ARK-3520L certification empty

---

## [2026-04-16] ingest | ARK-7060

- Action: Ingested `raw/ark-7000series/ARK-7060.md` (Advantech ARK-7060 spec sheet)
- Pages created: `wiki/sources/ARK-7060.md`, `wiki/entities/Intel Xeon D-1700 (Ice Lake-D).md`, `wiki/concepts/IPMI.md`
- Pages updated: `wiki/entities/Advantech.md` (ARK-7000 series + Xeon D-1700 row added), `wiki/synthesis/advantech-ark-series-comparison.md` (ARK-7060 row, memory tier, temp tier, timeline), `wiki/concepts/Fanless Embedded PC.md` (fan-cooled tier note), `index.md` (ARK-7000 series section, IPMI concept, Xeon D-1700 processor)
- Contradictions found: none
- Key finding: ARK-7060 is fundamentally different from all previous ARK models — fan-cooled (active cooling), AC power input (100–240V), IPMI 2.0 server management; represents a "server-grade edge" tier above ARK-3000
- Key finding: 128GB DDR4 ECC — highest RAM capacity in this wiki; surpasses ARK-3532B/C (64GB DDR4) and ARK-3534D (64GB DDR5)
- Key finding: No COM ports listed — only ARK model with zero serial ports
- Key finding: Optional dual 10GbE (Intel X550 via AMO-I031) — first 10GbE capability in this wiki
- Open questions flagged: COM port absence (genuine zero or spec sheet omission?); U0A1 power consumption TBD; certifications not listed; ARK-7060-U0A1 TPM AMO compatibility

---

## [2026-04-16] cleanup | Remove non-Advantech content

- Action: Removed all non-Advantech wiki content; updated index.md
- Files deleted (already gone from disk, removed from index): `wiki/sources/attention-is-all-you-need.md`, `wiki/entities/Ashish Vaswani.md`, `wiki/entities/Google Brain.md`, `wiki/concepts/Transformer Architecture.md`, `wiki/concepts/Self-Attention.md`, `wiki/concepts/Multi-Head Attention.md`, `wiki/concepts/Positional Encoding.md`
- Pages updated: `index.md` — removed AI/ML Papers section, AI/ML Concepts section, People section, Google Brain from Organisations; updated total page count to 52
- Rationale: Wiki scope is now exclusively Advantech ARK hardware per user instruction

---

## [2026-04-17] ingest | MIC-7 Series (8 files)

- Action: Ingested 8 Advantech MIC-series source files from `raw/MIC-series/`
- Source files: High Performance Embedded Box IPC (MIC-7000).md, MIC-760.md, MIC-770.md, MIC-770 V2.md, MIC-770 V3.md, MIC-7700.md, MIC-780.md, MIC-785.md
- Pages created (sources): `wiki/sources/mic-7000-series-overview.md`, `MIC-760.md`, `MIC-770.md`, `MIC-770-V2.md`, `MIC-770-V3.md`, `MIC-7700.md`, `MIC-780.md`, `MIC-785.md`
- Pages created (entities): `Intel Core Ultra Series 2.md`, `Intel 8th-9th Gen Core (LGA1151).md`, `Intel 6th-7th Gen Core Desktop (LGA1151).md`, `AMD Ryzen Embedded AM5.md`
- Pages created (concepts): `i-Module.md`, `NPU.md`, `ROS2.md`, `FlexIO.md`, `AMR MMR.md`, `EtherCAT.md`
- Pages created (synthesis): `MIC-770x.md` (generational hub), `MIC-78x.md` (Intel vs AMD hub), `mic-series-comparison.md` (master MIC comparison)
- Pages updated: `Advantech.md` (MIC product lines + CPU table + related entities), `Intel 12th-14th Gen Core (Raptor Lake LGA1700).md` (MIC-760 + MIC-770 V3 added), `Intel 10th Gen Xeon W (Comet Lake-S).md` (MIC-770 V2 added), `CAN Bus.md` (MIC-760 added), `SUSIAccess.md` (full MIC coverage + SUSI API clarification), `iDoor.md` (MIC-770 V2/V3 + MIC-785 added), `index.md` (21 entries added, total 73 pages)
- Contradictions found: none with ARK series; MIC-7 is a parallel product line, not overlapping
- Key finding: MIC-780 is the first fanless industrial box PC with integrated NPU (Intel Core Ultra Series 2 AI Boost) — unique in this entire wiki
- Key finding: MIC-785 is the first and only AMD-based product in this wiki (Ryzen Embedded / EPYC 4005, AM5)
- Key finding: MIC-760 is the only model in wiki with Industrial WiFi and ROS2 readiness — purpose-built for AMR/MMR mobile robotics
- Key finding: MIC-7700 (DVI + CFast), MIC-760 (full specs), MIC-785 (full specs) have incomplete raw data — feature lists only, no spec tables
- Open questions flagged: MIC-760/7700/785 detailed specs (RAM, temp, dimensions) missing; i-Module cross-generation compatibility unconfirmed; iBMC 1.2 vs IPMI 2.0 capability gap; NPU TOPS rating for MIC-780 not specified
