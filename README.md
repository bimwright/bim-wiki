---
title: "bim-wiki"
updated: 2026-04-20
---

<p align="center">
  <img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" width="360" />
</p>

<p align="center">
  📖 English · <a href="README.vi.md">Tiếng Việt</a> · <a href="README.zh-CN.md">简体中文</a>
</p>

---

# bim-wiki

I started writing these notes for myself. Every BEP meant cross-referencing ISO 19650 against four Vietnamese circulars (QĐ 347, QĐ 348, QĐ 1057, QĐ 2500) to figure out which term actually applied to the project in front of me — and every time I closed the laptop, I forgot the mapping.

This is that mapping, written down.

**bim-wiki** is a curated BIM knowledge base. Vietnamese-first summaries of ISO 19650 Parts 1–6, side-by-side with the Vietnamese regulatory landscape (the four QĐ above plus Luật 60/2024, Nghị định 111/2024 và 175/2024, and the Circulars 09/2024 and 24/2025). Plus the concept pages — CDE, LOIN, PIM/AIM, EIR cascade, BEP templates — cross-linked between the standard and local practice.

52 markdown pages, CC-BY-SA 4.0, paraphrased from sources (not verbatim). If you need normative ISO text, buy it from iso.org — this wiki is not a substitute.

## Who this is for

- BIM practitioners in Vietnam juggling ISO 19650 and the domestic regulations in the same document.
- Coordinators writing BEPs / pre-BEPs against QĐ 348 templates.
- Students and engineers who keep losing track of what term means what (LOIN vs LOD, PIM vs AIM, federation vs aggregation, CDE states vs revision states).
- AI agents that need BIM domain grounding — the pages are written so both humans and LLMs can read them.

## What's inside

- **`summary_*.md`** — chapter-level summaries of source documents (each ISO 19650 part, each Vietnamese circular).
- **Concept pages** — `cde.md`, `eir.md`, `pim.md`, `loin.md`, `bep.md`, `lod-vn.md`, and ~30 more. One topic per page, cross-linked.
- **VN-specific deltas** — `lod-vn.md`, `bim-applicability-matrix-vn.md`, `bep-template-qd348-variants.md`: where Vietnamese practice differs from ISO, and why.
- **`iso-19650.md`** — parent page for the series.
- **`index.md`** — master catalog.

## How to read

Start with [`index.md`](index.md) for the full catalog, or jump straight to a concept page if you already know what you're looking for.

### Source-attribution tags

Every page carries tags so you know what evidence each statement has behind it:

- `[ISO-CORE:verified]` — cross-checked against the raw ISO text (we hold a local reference copy; only the *fact* is re-expressed here, not the wording).
- `[ISO-CORE:structure]` — follows ISO clause structure but not verbatim-verified.
- `[VN-BXD:verified]` — cross-checked against the Vietnamese source PDF.
- `[COMMENTARY]` — bimwright's synthesis or comparison.
- `[INFERRED]` — logical deduction not directly stated in any source.

If a claim matters for your project, trace it to the tagged source before you rely on it.

## License & attribution

Licensed **CC-BY-SA 4.0** — see [`LICENSE`](LICENSE).

The license covers bimwright's **original contributions**: summaries, paraphrases, selection, arrangement, commentary. It does **not** grant rights over the underlying source standards. See [`NOTICE.md`](NOTICE.md) for the per-source policy — which sources are paraphrased under fair-use / fair-dealing, which are Vietnamese government works (public), and which still belong to the original rights-holder.

If you need normative ISO text, buy it from iso.org. This wiki is not a substitute.

## Contributing

Open an issue for a new page or a correction. For pull requests — see [`NOTICE.md`](NOTICE.md). Key rule: **paraphrase, don't paste.** Verbatim extracts from licensed standards get rejected, even if the edit is well-intended and the content is correct. The dual-tier model only works if the public tier stays clean.

---

Part of the [bimwright](https://github.com/bimwright) family —
[rvt-mcp](https://github.com/bimwright/rvt-mcp) (Revit ↔ LLM bridge) · bim-wiki (this repo) · more on the forge.

---

<p align="center">
  A <a href="https://github.com/bimwright">bimwright</a> project —
  <a href="https://github.com/bimwright"><img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" height="24" align="middle" /></a>
</p>
