---
title: "bim-wiki"
updated: 2026-04-20
---

<p align="center">
  <img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" width="360" />
</p>

<p align="center">
  📖 <a href="README.md">English</a> · <a href="README.vi.md">Tiếng Việt</a> · 简体中文
</p>

> 🇨🇳 **先说清楚：** 这个 README 是简体中文，但 wiki 里的 52 篇内容页是**越南语**写的（对照 ISO 19650 英文原文）。本 README 让你先判断 scope 合不合用，再决定要不要读下去。

---

# bim-wiki

我一开始写这些 note 是给自己看的。每次写 BEP，都要把 ISO 19650 跟 4 个越南总理决定（QĐ 347、QĐ 348、QĐ 1057、QĐ 2500）交叉对照，才能搞清楚某个术语到底对应项目里的哪一个概念 — 然后合上电脑的那一刻，mapping 就又忘光了。

这个 repo 就是把那个 mapping 写下来。

**bim-wiki** 是一个 curated 的 BIM 知识库。越南语优先的 ISO 19650 Parts 1–6 摘要，并排对照越南 BIM 法规体系（上面 4 个 QĐ + 越南国会 60/2024 号法律 + 政府 111/2024 和 175/2024 号议定 + 建设部 09/2024 和 24/2025 号通知）。外加概念页 — CDE、LOIN、PIM/AIM、EIR cascade、BEP 模板 — 在国际标准和本地实践之间建 cross-link。

52 个 markdown 页，CC-BY-SA 4.0，从原文 paraphrase（不是逐字复制）。如果你要 ISO 的规范原文，去 iso.org 买 — 这个 wiki 不是它的替代品。

## 这个仓给谁看

- 在越南做 BIM 的从业者，手里同时拿着 ISO 19650 和越南国内法规。
- 按 QĐ 348 模板写 BEP / pre-BEP 的协调员。
- 总记不住哪个术语对应哪个概念的学生和工程师（LOIN vs LOD、PIM vs AIM、federation vs aggregation、CDE states vs revision states）。
- 需要 BIM 领域 grounding 的 AI agent — 所有页都写成"人和 LLM 都能读"的样子。

**内容页的语言：** 越南语写的。如果你不读越南语，可以把具体页扔进 Claude / DeepL / GPT 之类的翻译成中文或英文读 — 越南语和 ISO 19650 英文术语之间的 mapping 就是这个 wiki 的核心贡献。

## 里面都有什么

- **`summary_*.md`** — 每份源文档的章节级摘要（ISO 19650 的每一个 Part、越南的每一份 QĐ / Luật / NĐ / TT）。
- **概念页** — `cde.md`、`eir.md`、`pim.md`、`loin.md`、`bep.md`、`lod-vn.md`，再加 ~30 个页。一页一个 topic，互相 cross-link。
- **VN delta 页** — `lod-vn.md`、`bim-applicability-matrix-vn.md`、`bep-template-qd348-variants.md`：越南实践跟 ISO 不一样的地方，以及为什么不一样。
- **`iso-19650.md`** — 系列的父页。
- **`index.md`** — 总 catalog。

## 怎么读

从 [`index.md`](index.md) 开始看完整 catalog，或者你知道自己要什么就直接跳到那页。

### 溯源标签

每一页都带标签，这样你知道每个命题背后有什么 evidence：

- `[ISO-CORE:verified]` — 跟 ISO 原文核对过（我们本地有一份参考副本；这里只是把 *事实* 重新表达，不是复制 wording）。
- `[ISO-CORE:structure]` — 沿用 ISO 的 clause 结构，但没有逐字核对。
- `[VN-BXD:verified]` — 跟越南源 PDF 核对过。
- `[COMMENTARY]` — bimwright 自己的综合 / 对比。
- `[INFERRED]` — 逻辑推导，原文没有直接写。

如果某个命题对你的项目很关键，用它之前先 trace 回 tag 对应的 source。

## License & attribution

**CC-BY-SA 4.0** — 见 [`LICENSE`](LICENSE)。

这个 license 覆盖 bimwright 的**原创贡献**：摘要、paraphrase、挑选、编排、commentary。它**不**授权你用原始标准文本。详细的 per-source 政策看 [`NOTICE.md`](NOTICE.md) — 哪些源是按 fair-use / fair-dealing paraphrase 的、哪些是越南政府公开文件（公有）、哪些还是原权利人的。

要 ISO 规范原文，去 iso.org 买。这个 wiki 不是替代。

## Contributing

开 issue 提新页面或者报错。PR 先看 [`NOTICE.md`](NOTICE.md)。核心规则：**paraphrase，不要 paste。** 从有版权的标准里逐字摘的东西会被 reject，哪怕 edit 是善意的、内容是对的。dual-tier 模式只有在 public tier 保持干净的时候才工作。

---

属于 [bimwright](https://github.com/bimwright) 家族 —
[rvt-mcp](https://github.com/bimwright/rvt-mcp)（Revit ↔ LLM 桥）· bim-wiki（这个仓）· 还有更多在炉上。

---

<p align="center">
  一个 <a href="https://github.com/bimwright">bimwright</a> 项目 —
  <a href="https://github.com/bimwright"><img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" height="24" align="middle" /></a>
</p>
