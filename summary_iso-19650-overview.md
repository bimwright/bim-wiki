---
title: "ISO 19650 Series — Overview (Summary)"
aliases: ["ISO 19650 tổng quan", "ISO 19650 series overview"]
tags: ["#bim", "#iso-19650", "#standard", "#summary"]
type: summary
source: "[[raw/core/ISO_19650_Overview]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# ISO 19650 Series — Overview

> **TL;DR:** Bộ tiêu chuẩn quốc tế 6 phần về quản lý thông tin BIM trong toàn vòng đời tài sản xây dựng; Part 1 là nền tảng khái niệm, Parts 2–6 là yêu cầu bắt buộc từng giai đoạn.

## Nội dung tóm tắt

### Về bộ tiêu chuẩn

ISO 19650 có tiêu đề đầy đủ: *"Organization and digitization of information about buildings and civil engineering works, including building information modelling (BIM) — Information management using building information modelling"*. Được phát triển bởi ISO/TC 59/SC 13. Thay thế toàn bộ cho bộ tiêu chuẩn PAS 1192 (mô hình BIM Level 2 của UK trước đây). Xem [[pas-1192-mapping]].

- **National Annexes:** Mỗi quốc gia khi áp dụng ISO 19650 có khả năng phát hành một Phụ lục Quốc gia (National Annex) để quy định mã trạng thái, phân loại và naming riêng (ví dụ: [[uk-national-annex]]).

### Sáu phần và vai trò

| Phần | Năm | Loại | Phạm vi |
|------|-----|-------|---------|
| Part 1 | 2018 | Guidance ("should") | Khái niệm & nguyên tắc — nền tảng cho toàn bộ series |
| Part 2 | 2018 | Requirements ("shall") | Giai đoạn thiết kế và thi công |
| Part 3 | 2020 | Requirements ("shall") | Giai đoạn vận hành & bảo trì |
| Part 4 | 2022 | Requirements ("shall") | Trao đổi thông tin — tiêu chí chất lượng "6 Cs" |
| Part 5 | 2020 | Requirements ("shall") | Bảo mật thông tin (overlay trên Parts 2, 3, 4) |
| Part 6 | 2025 | Requirements ("shall") | Thông tin An toàn & Sức khỏe (overlay trên Parts 2, 3) |

### Kiến trúc phụ thuộc

- **Part 1** là foundation — không có requirement, chỉ recommendation.
- **Parts 2 & 3** là hai nhánh chính theo vòng đời tài sản (delivery → operation). PIM từ Part 2 handover thành AIM ở Part 3.
- **Part 4** bổ sung tiêu chí chất lượng cho mọi trao đổi thông tin trong Parts 2 & 3.
- **Parts 5 & 6** là overlay — bọc quanh quy trình Parts 2 & 3 ở mỗi giai đoạn (không thay thế, chỉ bổ sung lớp bảo mật / H&S).

### Quy trình 8 giai đoạn (Parts 2 & 3)

Part 2 định nghĩa 8-stage information delivery cycle (Clause 5):
1. Assessment & need → 2. Invitation to tender → 3. Tender response → 4. Appointment → 5. Mobilization → 6. Collaborative production → 7. Information model delivery → 8. Project close-out.
Stages 5.1 và 5.8 chỉ xảy ra 1 lần/project; stages 5.2–5.7 lặp lại theo từng appointment.

Part 3 tái dùng cùng 8-stage (~75% nội dung trùng) nhưng thêm khái niệm **trigger event** (planned / unplanned / asset acquisition) thay cho project inception.

### Tiêu chí chất lượng "6 Cs" (Part 4)

CDE · Conformance · Continuity · Communication · Consistency · Completeness.

### Quy trình bảo mật 4 bước (Part 5)

Security triage → Security strategy → Security management plan → Breach/incident management plan.

### Chu trình H&S 5 bước (Part 6)

Adopt schema → Record risk types → Link risks to models → Take action → Share via CDE.

### Hệ thống từ viết tắt cốt lõi

[[aim]] · [[bep]] · [[bim]] · [[bim-delivery-roles]] · [[cde]] · [[eir]] · [[information-requirements-hierarchy]] (OIR/AIR/PIR/EIR) · [[loin]] · [[pim]] · MIDP · TIDP

### Out-of-scope themes (flagged, not filed)

- ISO 9001 quality management (cross-industry standard — defer; promote on 2nd source mention)
- ISO 21500 project management (quá rộng, không BIM-specific — defer)
- ISO 55000 asset management (promote when Part 3 ingested)
- ISO 12006-2/3 classification, ISO 29481-1 IDM, ISO 31000 risk (widely-known standards — defer)
- EN 17412-1:2020 LOIN methodology (promote when Part 1 ingested)

## Quan hệ

- **Children:** [[iso-19650]] (entity — toàn series), [[cde]], [[bim]], [[pim]], [[aim]], [[loin]], [[bep]], [[eir]], [[information-requirements-hierarchy]], [[bim-delivery-roles]]
- **Related:** [[legacy/PAS_1192_Mapping]] — predecessor standard mapping

## Nguồn

- [[raw/core/ISO_19650_Overview]] — toàn bộ file (~1,800 words, compiled 2026-03-31, tag `[ISO-CORE:structure]`)
