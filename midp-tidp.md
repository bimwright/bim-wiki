---
title: "MIDP & TIDP — Information Delivery Plans"
aliases: ["MIDP", "TIDP", "Master Information Delivery Plan", "Task Information Delivery Plan", "Kế hoạch giao nộp thông tin"]
tags: ["#bim", "#iso-19650", "#concept", "#midp", "#tidp", "#delivery-planning"]
type: concept
source: "[[raw/core/ISO_19650-1]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# MIDP & TIDP — Information Delivery Plans

> **TL;DR:** TIDP (per task team) và MIDP (aggregated by Lead Appointed Party) là hai tài liệu lập kế hoạch giao nộp thông tin — định nghĩa AI produce WHAT containers, WHEN, và HOW trong suốt dự án.

## Khái niệm cốt lõi

### TIDP — Task Information Delivery Plan

`[ISO-CORE:structure]` Mỗi task team lập 1 TIDP cho phạm vi công việc của mình:

| Element | Nội dung |
|---------|---------|
| **Container list** | Tất cả [[information-container]] task team sẽ produce |
| **Sequence** | Thứ tự production |
| **Dependencies** | Dependency nội bộ và từ external sources |
| **Duration** | Thời gian production |
| **Format** | Định dạng deliverable |
| **Dates** | Ngày giao nộp |
| **Responsibilities** | Assigned individuals |
| **LOIN** | [[loin]] cho từng container (per [[eir]]) |

### MIDP — Master Information Delivery Plan

`[ISO-CORE:structure]` Lead Appointed Party aggregate tất cả TIDPs thành 1 tài liệu trung tâm:

- Combine ALL task teams' TIDPs
- Show complete sequence of all deliverables
- Identify WHEN information is exchanged (aligned với key decision points)
- Serve as project's **information roadmap**

### Planning sequence (Clause 10)

```
Federation Strategy
    ↓
ICBS (Information Container Breakdown Structure)
    ↓
High-Level Responsibility Matrix (Lead Appointed Party level)
    ↓
Detailed Responsibility Matrix (task team level)
    ↓
TIDPs (per task team) ← Appointed Party
    ↓
MIDP (aggregate) ← Lead Appointed Party
```

## Chi tiết / Triển khai

### Khi nào lập MIDP/TIDP

`[ISO-CORE:structure]` Established tại **Part 2 Stage 5.4** (Appointment):
- Stage 5.3 (Tender response): Pre-appointment BEP đã có draft MIDP sơ bộ
- Stage 5.4 (Appointment): Confirmed BEP → MIDP + TIDPs được finalize
- Stage 5.5 (Mobilization): Mobilize resources theo MIDP
- Stage 5.6–5.7: Execute và deliver theo MIDP/TIDP schedule

### Information exchanges và Key Decision Points

`[ISO-CORE:structure]` Exchanges xảy ra tại pre-defined decision points (3.2.14) aligned với:
- Project stage gates
- Contractual deliverable dates
- Key decision points in [[eir]]

MIDP phải sync với project programme — thường tích hợp với project management schedule.

### Responsibility Matrix (liên quan)

Hai cấp (per Clause 10.3):
- **High-level:** Which Lead Appointed Party chịu trách nhiệm major components
- **Detailed:** Which task team chịu trách nhiệm từng individual container

RACI-type: Responsible · Accountable · Consulted · Informed.

## Quan hệ

- **Parent:** [[bim-delivery-roles]] — Lead Appointed Party lập MIDP; Appointed Party lập TIDP
- **Contains:** [[information-container]] — TIDP list các containers cần produce
- **References:** [[loin]] — LOIN được specify per container trong TIDP
- **Part of:** [[bep]] — MIDP/TIDP là output của confirmed BEP (Stage 4)
- **Operationalized in:** Part 2 Stage 5.4 — see [[summary_iso-19650-2]]

## Nguồn

- [[raw/core/ISO_19650-1]] — Clauses 10.2–10.4 `[ISO-CORE:structure]` — [[summary_iso-19650-1]]
- [[raw/core/ISO_19650-2]] — Clauses 5.4.4 (TIDP), 5.4.5 (MIDP) `[ISO-CORE:verified]` — cụ thể hóa quy trình lập kế hoạch giao nộp — [[summary_iso-19650-2]]
- [[raw/national-standards/VN/templates/BEP_Template_QD348]] `[VN-BXD:verified]` — Mẫu BEP yêu cầu tham chiếu trực tiếp Biểu mẫu 04 (MIDP) và nơi lưu MIDP trên CDE — [[summary_bep-template-qd348]]
