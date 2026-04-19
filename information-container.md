---
title: "Information Container"
aliases: ["information container", "Information Container", "container thông tin"]
tags: ["#bim", "#iso-19650", "#concept", "#information-container"]
type: concept
source: "[[raw/core/ISO_19650-1]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# Information Container

> **TL;DR:** Information container là đơn vị lưu trữ thông tin cơ bản trong BIM — bất kỳ file, model, schedule, hay tài liệu nào có tên xác định và có thể truy xuất; được gán status code và managed trong CDE.

## Khái niệm cốt lõi

- **Định nghĩa (3.3.12):** Named persistent set of information retrievable from within a file, system or application storage hierarchy `[ISO-CORE:verified]`
- **Ví dụ:** Sub-directory, information file (model, document, table, schedule), hoặc distinct sub-set như chapter, section, layer, symbol
- **Hai loại:**
  - **Structured:** Geometrical models, schedules, databases — có cấu trúc dữ liệu rõ ràng
  - **Unstructured:** Documentation, video clips, sound recordings — dạng tự do
- **Metadata tối thiểu bắt buộc:** Unique ID (filename theo convention), revision code, status code (3.3.13), classification code
- **Status code (3.3.13):** Metadata mô tả suitability của nội dung container — cho agent biết container đang ở trạng thái nào trong CDE workflow (WIP/Shared/Published/Archive) và được dùng cho mục đích gì
- **Persistent:** Thông tin tồn tại đủ lâu để phải quản lý — excludes transient info (search results...). `[ISO-CORE:verified]`
- **Naming convention:** Naming của container phải theo agreed convention từ [[eir]] và [[bim-delivery-roles]] (Lead Appointed Party định nghĩa, Appointing Party phê duyệt)

## Chi tiết / Triển khai

### Information Container Breakdown Structure (ICBS)

`[ISO-CORE:structure]` Cách chia nhỏ thông tin thành manageable units theo 3 kiểu phân cấp (kết hợp lại được):

| Loại | Chia theo | Ví dụ |
|------|-----------|-------|
| **Spatial** | Vị trí vật lý | Building → Floor/Level → Zone → Room |
| **Functional** | Hệ thống/discipline | Structural / Mechanical / Electrical / Architectural |
| **Form-based** | Loại biểu diễn | 3D Model / 2D Drawing / Schedule / Specification |

Ví dụ combined: `"Level 03 — Mechanical — 3D Model"` = spatial + functional + form.

**Mục đích ICBS:** Xác định ai chịu trách nhiệm produce container nào (Responsibility Matrix), tổ chức TIDP/MIDP, và định nghĩa [[federation]] strategy.

### Vòng đời trong CDE

Container di chuyển qua 4 trạng thái trong [[cde]]:

```
WIP → (Gate 1: Check/Review/Approve) → Shared
                                             ↓
                                  (Gate 2: Review/Authorize)
                                             ↓
                                         Published
                                             ↓
                                         Archive (audit trail)
```

Khi modification cần thiết: Published → WIP → ... → re-Published với revision mới.

### Revision vs Version
- **Version:** Iteration trong 1 state (WIP/Shared) — internal tracking
- **Revision:** Formal iteration sau khi Published — externally visible, contractual

## Quan hệ

- **Parent:** [[bim]]
- **Managed in:** [[cde]] — CDE quản lý toàn bộ lifecycle của containers
- **Organized by:** [[federation]] — multiple containers từ nhiều task teams được federate thành composite model
- **Planned in:** [[midp-tidp]] — TIDP list tất cả containers task team sẽ produce; MIDP aggregate
- **Defined by:** [[eir]] — EIR specify containers nào cần produce, LOIN của từng container, format/naming convention

## Nguồn

- [[raw/core/ISO_19650-1]] — Clauses 3.3.12 (verified), 9, 10, 12 — [[summary_iso-19650-1]]
- [[raw/core/ISO_19650-4]] — Introduction `[ISO-CORE:verified]` — Định nghĩa Container bắt buộc phải retrievable và persistent (thông qua revisioning & archiving), bổ sung thêm các ràng buộc open schema cho file định dạng (phục vụ Criterion 7.2) — [[summary_iso-19650-4]]
