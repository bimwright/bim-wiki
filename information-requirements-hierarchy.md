---
title: "Information Requirements Hierarchy (OIR / AIR / PIR / EIR)"
aliases: ["Information Requirements", "OIR", "AIR", "PIR", "Information Requirements Hierarchy", "Hệ thống yêu cầu thông tin"]
tags: ["#bim", "#iso-19650", "#concept", "#information-requirements"]
type: concept
source: "[[raw/core/ISO_19650_Overview]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# Information Requirements Hierarchy

> **TL;DR:** ISO 19650-1 định nghĩa hierarchy 4 tầng OIR → AIR/PIR → EIR để cascade yêu cầu thông tin từ cấp tổ chức xuống cấp trao đổi cụ thể trong dự án.

## Khái niệm cốt lõi

- **OIR — Organizational Information Requirements** (clause 3.3.3): Yêu cầu thông tin cấp tổ chức — *"Tổ chức cần biết gì để quản lý danh mục tài sản?"*. Là nguồn gốc của toàn bộ hierarchy.
- **AIR — Asset Information Requirements** (clause 3.3.4): Yêu cầu thông tin cấp tài sản trong giai đoạn vận hành — *"Cần thông tin gì để vận hành & bảo trì tài sản này?"*. Deriving từ OIR, phục vụ [[aim]].
- **PIR — Project Information Requirements** (clause 3.3.5): Yêu cầu thông tin cấp dự án — *"Cần thông tin gì để ra quyết định cho dự án này?"*. Deriving từ OIR, phục vụ [[pim]].
- **EIR — Exchange Information Requirements** (clause 3.3.6): Yêu cầu trao đổi cụ thể cho từng appointment — *"Deliver team phải nộp gì, ở mức nào, khi nào?"*. Deriving từ AIR/PIR. Xem trang riêng: [[eir]].

### Mối quan hệ cascade

```
OIR (Organizational)
├── AIR (Asset) ──→ định nghĩa yêu cầu cho AIM
│     └── EIR (Exchange) ──→ phát hành trong tender
└── PIR (Project) ──→ định nghĩa yêu cầu cho PIM
      └── EIR (Exchange) ──→ phát hành trong tender
```

- **Nguyên tắc:** EIR không được yêu cầu thông tin vượt ngoài phạm vi AIR/PIR; AIR/PIR không vượt OIR. Hierarchy đảm bảo "information pull" (kéo thông tin theo nhu cầu) thay vì "information push" (đẩy thông tin theo thói quen).
- **Phát hành:** Appointing Party lập OIR/AIR/PIR; phát hành EIR trong Stage 1 (project-level) và Stage 2 (per-appointment)

## Quan hệ

- **Parent:** [[iso-19650]]
- **Children:** [[eir]] — EIR là tầng cuối cùng trong hierarchy
- **Defines content of:** [[pim]] (qua PIR), [[aim]] (qua AIR)
- **Issued by:** [[bim-delivery-roles]] — Appointing Party

## Nguồn

- [[raw/core/ISO_19650_Overview]] — [[summary_iso-19650-overview]]
- [[raw/core/ISO_19650-1]] — Clause 5.1–5.6 `[ISO-CORE:verified/structure]` — Figure 2 diagrams hóa full cascade; xác nhận AIR ≠ PIR (aím vs project); PLQ concept (Plain Language Questions) cho OIR; lean EIR principle (minimum info only) — [[summary_iso-19650-1]]
- [[raw/core/ISO_19650-3]] — Clauses 5.1.2 (OIR) và 5.1.4 (AIR) khẳng định khác biệt chính so với Part 2. OIR là vĩnh viễn, EIR được suy ra trực tiếp từ AIR trong giai đoạn vận hành `[ISO-CORE:structure]` — [[summary_iso-19650-3]]
