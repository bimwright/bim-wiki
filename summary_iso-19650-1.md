---
title: "ISO 19650-1 — Concepts and Principles (Summary)"
aliases: ["ISO 19650 Part 1 summary", "ISO 19650-1:2018 tóm tắt"]
tags: ["#bim", "#iso-19650", "#iso-19650-1", "#standard", "#summary"]
type: summary
source: "[[raw/core/ISO_19650-1]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# ISO 19650-1 — Concepts and Principles

> **TL;DR:** Part 1 là tài liệu guidance (dùng "should", không phải "shall") đặt nền khái niệm và nguyên tắc cho toàn bộ series ISO 19650; bao gồm 13 clauses từ information requirements hierarchy đến CDE workflow.

## Nội dung tóm tắt

### Tổng quan và phạm vi (Clause 1)

`[ISO-CORE:verified]` Phác thảo các khái niệm và nguyên tắc quản lý thông tin ở mức trưởng thành được mô tả là "BIM theo ISO 19650 series". Áp dụng cho **toàn vòng đời** của bất kỳ tài sản xây dựng nào từ quy hoạch chiến lược đến kết thúc vòng đời. Có thể áp dụng cho tài sản/dự án ở bất kỳ quy mô nào.

**Lưu ý quan trọng:** Part 1 chỉ gồm khuyến nghị — không có nghĩa vụ áp dụng Part 2 hoặc các phần khác của series.

### 3 nhóm thuật ngữ cốt lõi (Clause 3) `[ISO-CORE:verified]`

**3.1 General:** responsibility matrix (3.1.1), space (3.1.2)

**3.2 Assets & Projects:** actor, appointment, appointed party, appointing party, client, delivery team, task team, asset, project information, life cycle, delivery phase, operational phase, trigger event, key decision point

**3.3 Information Management:**

> Bảng dưới đây là **tóm lược bằng tiếng Việt** của bimwright, không phải trích nguyên văn ISO. Về ngữ nghĩa chuẩn tắc (normative), tham khảo bản ISO 19650-1:2018 chính thức tại iso.org.

| Term | Clause | Tóm lược (paraphrase) |
|------|--------|----------------------|
| information | 3.3.1 | Biểu diễn dữ liệu có thể diễn giải lại, phù hợp để truyền đạt |
| information requirement | 3.3.2 | Đặc tả thông tin được tạo: nội dung gì, khi nào, cách nào, cho ai |
| OIR | 3.3.3 | Yêu cầu thông tin gắn với mục tiêu của tổ chức |
| AIR | 3.3.4 | Yêu cầu thông tin gắn với việc vận hành tài sản |
| PIR | 3.3.5 | Yêu cầu thông tin gắn với quá trình bàn giao tài sản |
| EIR | 3.3.6 | Yêu cầu thông tin gắn với một lần bổ nhiệm/hợp đồng |
| information exchange | 3.3.7 | Hành vi đáp ứng một yêu cầu thông tin (hoặc một phần của nó) |
| information model | 3.3.8 | Tập hợp các information container có cấu trúc và phi cấu trúc |
| AIM | 3.3.9 | Information model gắn với giai đoạn vận hành |
| PIM | 3.3.10 | Information model gắn với giai đoạn bàn giao |
| federation | 3.3.11 | Việc ghép các container rời thành một information model tổng hợp |
| information container | 3.3.12 | Tập thông tin có tên, bền vững, truy xuất được từ file/hệ thống/ứng dụng |
| status code | 3.3.13 | Metadata mô tả mức độ phù hợp của một information container |
| BIM | 3.3.14 | Việc dùng một biểu diễn số dùng chung cho công trình xây dựng… |
| CDE | 3.3.15 | Nguồn thông tin được thống nhất để thu thập, quản lý và phân phối container |
| LOIN | 3.3.16 | Khung xác định phạm vi và độ chi tiết của thông tin |
| capability | 3.3.18 | Đo lường năng lực thực thi (kỹ năng, kiến thức, chuyên môn) |
| capacity | 3.3.19 | Nguồn lực sẵn có để thực thi (phương tiện, tài nguyên, quy trình) |

### Perspectives và collaborative working (Clause 4) `[ISO-CORE:structure]`

**Stage 2 maturity:** ISO 19650 đặt BIM tại Stage 2 trong 3 cấp độ trưởng thành thông tin:
- Stage 1: File-based, 2D CAD standalone
- **Stage 2: BIM per ISO 19650** — federated model, CDE workflow, mixed manual/automated
- Stage 3: Integrated/networked databases, immediately interrogable models

**4 perspectives (Table 1):** Asset Owner · Asset User · Project Delivery/Asset Management · Society — mọi yêu cầu thông tin phải xem xét cả 4 góc nhìn này.

### Information Requirements Cascade (Clause 5) `[ISO-CORE:verified]`

Hierarchy: OIR → AIR/PIR → EIR → tạo ra PIM (delivery phase) và AIM (operational phase). Xem chi tiết: [[information-requirements-hierarchy]].

**PIM có 2 giai đoạn phát triển:**
1. **Design Intent Model** — ý định thiết kế về geometry, spatial, performance
2. **Virtual Construction Model** — kế hoạch thi công của contractor

**EIR — 3 nhóm nội dung (COMMENTARY):**
- Technical: software platforms, LOIN, file formats
- Management: protocols, CDE processes
- Commercial: deliverables list, milestones

Nguyên tắc lean: chỉ yêu cầu thông tin tối thiểu cần thiết (over-specification = lãng phí).

### Information Delivery Cycle (Clause 6) `[ISO-CORE:structure]`

Chu trình tuần hoàn qua 3 điểm quyết định:
- **Point A:** Operational → Delivery (trigger event kích hoạt dự án mới)
- **Point B:** Trong delivery (stage gates — information được exchange và authorize)
- **Point C:** Delivery → Operational (project completion, PIM → AIM handover)

4 nguyên tắc: lifecycle need · progressive specification · delivery routing · coordinated exchange via CDE.

**Verification vs Validation (6.3.3):**
- Verification: "Deliverable có đúng với yêu cầu không?"
- Validation: "Nó có đủ hỗ trợ quyết định không?"

Multi-level review: Task team (WIP) → Lead Appointed Party (Shared) → Appointing Party (Published).

### Information Management Functions (Clause 7) `[ISO-CORE:structure]`

3 cấp: Asset Info Mgmt (7.2 — scope Part 3) · Project Info Mgmt (7.3 — scope Part 2 Stage 5.1) · Task Info Mgmt (7.4 — per TIDP).

### Capability & Capacity (Clause 8) `[ISO-CORE:verified]`

**Capability** (3.3.18): skill/knowledge/expertise — time-independent.  
**Capacity** (3.3.19): resources/means/procedures — changes with concurrent workload.  
8 criteria assessment được đánh giá bởi appointing party, prospective team, hoặc independent party.

### Information Container-Based Collaborative Working (Clause 9) `[ISO-CORE:structure]`

6 principles (a–f): Authorship · Clarity of requirements · Capability · CDE · Technology conformance · Information security.

**3 loại ICBS (Information Container Breakdown Structure):**
- Spatial (building/floor/zone/room)
- Functional (discipline: structural/MEP/architectural)
- Form-based (3D model/2D drawing/schedule/specification)

→ Xem chi tiết: [[information-container]], [[federation]]

### Information Delivery Planning (Clause 10) `[ISO-CORE:structure]`

Planning sequence: Federation Strategy → ICBS → High-Level Responsibility Matrix → Detailed Responsibility Matrix → TIDPs (per task team) → MIDP (aggregated).

→ Xem chi tiết: [[midp-tidp]]

### Managing Collaborative Production (Clause 11) `[ISO-CORE:structure]`

**LOIN (3.3.16):** 4 components — Purpose · Content (geometrical + alphanumerical + documentation) · Form · Format. LOIN is identified per information container, recorded in TIDPs.

**Information quality:** Fit for purpose → QA by originator (WIP→Shared gate) → QC by lead (Shared→Published gate).

### CDE Solution and Workflow (Clause 12) `[ISO-CORE:verified]`

**CDE Solution** (technology platform, e.g., ProjectWise, BIM 360) vs **CDE Workflow** (organizational process với states và gates).

**Version vs Revision:**
- Version: iteration within a state (internal tracking)
- Revision: formal iteration of published information (contractual)

→ Xem chi tiết: [[cde]]

### Out-of-scope themes (flagged, not filed)

- ISO 9001, ISO 21500, ISO 55000, ISO 12006-2/3, ISO 29481-1, ISO 31000 — referenced in Bibliography; out-of-scope (đã flagged trong [[summary_iso-19650-overview]])
- EN 17412-1:2020 LOIN methodology — referenced tại Clause 11.2; promote sang trang riêng khi Part 1 ingest xong (thực ra **đây** là lần ingest đó → promote: xem [[loin]] đã cập nhật)
- National Annexes (UK_NA.md) — status codes scheme; sẽ cover khi ingest `national-annexes/UK_NA.md`

## Quan hệ

- **Parent:** [[iso-19650]]
- **Children (concepts defined here):** [[information-container]], [[federation]], [[midp-tidp]]
- **Updated by this ingest:** [[cde]], [[loin]], [[eir]], [[pim]], [[aim]], [[bim-delivery-roles]], [[information-requirements-hierarchy]]

## Nguồn

- [[raw/core/ISO_19650-1]] — ~13,000 words; Clause 3 định nghĩa `[ISO-CORE:verified]` từ `text-raw/iso-19650-1-2018.txt`; Clauses 4–13 `[ISO-CORE:structure]` (compiled 2026-03-31)
