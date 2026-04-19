---
title: "Federation (BIM)"
aliases: ["federation", "Federation", "Information Model Federation", "federated model"]
tags: ["#bim", "#iso-19650", "#concept", "#federation"]
type: concept
source: "[[raw/core/ISO_19650-1]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# Federation (BIM)

> **TL;DR:** Federation là quá trình tạo composite information model từ nhiều information containers riêng biệt của các task teams khác nhau — nền tảng cho collaborative production trong BIM.

## Khái niệm cốt lõi

- **Định nghĩa (3.3.11):** Creation of a composite information model from separate information containers. The separate information containers can come from different task teams. `[ISO-CORE:verified]`
- **Bản chất:** Thay vì 1 file monolithic duy nhất, tất cả các discipline (structural, MEP, architectural, ...) maintain containers riêng biệt → federate lại để coordination, clash detection, authorization
- **Lợi ích:**
  - Multiple task teams làm việc **song song** trên **cùng 1 project** mà không conflict
  - Containers được **kết hợp theo mục đích cụ thể** (coordination vs handover vs authorization)
  - Composite model được **assembled từ parts** — không cần file monolithic
  - Có thể **selective federation**: chọn containers liên quan theo purpose/security level
- **Federation Strategy:** Mô tả high-level HOW và WHY information model được chia nhỏ theo ICBS. Được communicate qua Standard Methods and Procedures (Appointing Party) hoặc BEP. `[ISO-CORE:structure]`
- **Security federation (Annex A):** Sensitive containers isolated với restricted access; khác nhau security classification cho khác nhau containers; federation rules control permitted combinations

## Chi tiết / Triển khai

### Federated Information Model vs Monolithic

| Approach | Điểm mạnh | Điểm yếu |
|----------|-----------|----------|
| **Federated** | Parallel work, light containers, selective sharing, clear ownership | Cần phối hợp naming/coordinates, federation overhead |
| **Monolithic** | Single file đơn giản | Conflict khi nhiều người edit, file size lớn, không scalable |

ISO 19650 (Stage 2 maturity) giả định **federated model** theo CDE workflow.

### Federation trong CDE Workflow

`[ISO-CORE:structure]` Thực hành thông thường:
1. Task teams produce containers trong WIP state riêng biệt
2. Khi ready → move sang Shared state
3. Lead Appointed Party federate containers từ Shared → coordination/clash detection
4. Approved composite → Published state cho Appointing Party
5. Superseded containers → Archive

### ICBS và Federation Strategy

[[information-container]] được tổ chức theo ICBS (Spatial + Functional + Form). Federation strategy xác định:
- Các containers nào được federate với nhau
- Tần suất federation (daily? per stage gate?)
- Ai có quyền đọc federated combinations nào

## Quan hệ

- **Parent:** [[bim]]
- **Uses:** [[information-container]] — federation tạo composite từ nhiều containers
- **Operated in:** [[cde]] — CDE là môi trường nơi containers được share và federate
- **Planned by:** [[midp-tidp]] — MIDP/TIDP coordinate timing của federation
- **Security aspect:** Referenced by Part 5 (Annex A.3 security federation)

## Nguồn

- [[raw/core/ISO_19650-1]] — Clauses 3.3.11 (verified), 9, Annex A — [[summary_iso-19650-1]]
