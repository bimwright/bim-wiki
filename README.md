---
title: "bim-wiki"
updated: 2026-04-20
---

<p align="center">
  <img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" width="360" />
</p>

# bim-wiki

A BIM domain knowledge base curated by [bimwright](https://github.com/bimwright) —
Vietnamese-first summaries and cross-referenced commentary on ISO 19650, the
Vietnamese BIM regulatory landscape (QĐ 347/348/1057/2500, Luật 60/2024, Nghị định
111/2024), Revit handover workflows, and adjacent standards.

## Who this is for

- BIM practitioners in Vietnam navigating both ISO 19650 and domestic regulations
- BIM coordinators writing BEPs / pre-BEPs against Vietnamese templates
- Engineers needing a single cross-referenced map of terminology (LOIN vs LOD,
  PIM vs AIM, EIR cascade, CDE states)
- AI agents grounded on BIM domain context (this wiki is designed to be readable
  by both humans and LLMs)

## What's inside

- **`summary_*.md`** — chapter-level summaries of source documents
- **Concept pages** (`cde.md`, `eir.md`, `pim.md`, `loin.md`, `bep.md`, …) — one
  topic per page, cross-linked
- **VN-specific pages** (`lod-vn.md`, `bim-applicability-matrix-vn.md`,
  `bep-template-qd348-variants.md`) — Vietnamese regulatory deltas vs ISO
- **`iso-19650.md`** — parent entity page for the series
- **`index.md`** — master catalog

## How to read

Start with [`index.md`](index.md) for the full catalog, or jump straight to a
concept page if you know what you're looking for.

Each page uses source-attribution tags:
- `[ISO-CORE:verified]` — cross-checked against raw ISO text (we hold a local
  reference copy; only the FACT is re-expressed here, not the wording)
- `[ISO-CORE:structure]` — follows ISO clause structure but not verbatim-verified
- `[VN-BXD:verified]` — cross-checked against the Vietnamese source PDF
- `[COMMENTARY]` — bimwright's synthesis or comparison
- `[INFERRED]` — logical deduction not directly stated in any source

## License & attribution

This repository is licensed **CC-BY-SA 4.0** — see [`LICENSE`](LICENSE).

The license covers bimwright's **original contributions** (Vietnamese summaries,
paraphrases, selection, arrangement, commentary). It does **not** grant rights to
the underlying source standards. See [`NOTICE.md`](NOTICE.md) for the full source
attribution policy — including which sources are paraphrased under fair-use /
fair-dealing principles vs which are Vietnamese government works (public).

**If you need normative ISO text**, purchase the standards directly from iso.org.
This wiki is not a substitute.

## Contributing

Open an issue to suggest a new page or correction. For pull requests, see
[`NOTICE.md`](NOTICE.md) — key rule: **paraphrase, don't paste**.

---

Part of the [bimwright](https://github.com/bimwright) family —
[rvt-mcp](https://github.com/bimwright/rvt-mcp) (Revit ↔ LLM bridge) · bim-wiki
(this repo) · more to come.

---

<p align="center">
  A <a href="https://github.com/bimwright">bimwright</a> project —
  <a href="https://github.com/bimwright"><img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" height="24" align="middle" /></a>
</p>
