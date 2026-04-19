---
title: "AIM — Asset Information Model"
aliases: ["Asset Information Model", "AIM"]
tags: ["#bim", "#iso-19650", "#concept", "#information-model"]
type: concept
source: "[[raw/core/ISO_19650_Overview]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# AIM — Asset Information Model

> **TL;DR:** AIM là mô hình thông tin của tài sản trong giai đoạn vận hành và bảo trì; được khởi tạo từ PIM khi bàn giao và duy trì cập nhật suốt vòng đời tài sản.

## Khái niệm cốt lõi

- **Định nghĩa:** Information model tích lũy và cập nhật trong giai đoạn vận hành, bảo trì, và kết thúc vòng đời tài sản (ISO 19650-1, clause 3.3.9)
- **Giai đoạn:** Tương ứng ISO 19650-3 (Operational phase) — liên tục trong suốt vòng đời tài sản
- **Nguồn gốc:** Được init từ authorized [[pim]] tại thời điểm bàn giao (stage 5.8 của ISO 19650-2)
- **Cập nhật:** Mỗi lần có trigger event (planned maintenance, unplanned repair, asset acquisition), AIM được cập nhật thông qua quy trình ISO 19650-3
- **Yêu cầu thông tin:** Được định nghĩa bởi AIR (Asset Information Requirements) trong [[information-requirements-hierarchy]]

## Chi tiết / Triển khai

- **Trigger events (Part 3):** 3 loại kích hoạt cập nhật AIM:
  - **Planned:** Bảo trì định kỳ — có thể bỏ qua tender nếu dùng framework agreement
  - **Unplanned:** Sự cố khẩn cấp — phải đi qua đầy đủ quy trình 8 giai đoạn
  - **Asset acquisition:** Mua/chuyển nhượng tài sản — verify thông tin rồi proceed to acceptance
- **Phân biệt với PIM:** AIM là thông tin *thực tế* của tài sản đang tồn tại (as-maintained); PIM là thông tin *dự án* đang xây dựng

## Quan hệ

- **Parent:** [[bim]]
- **Alternative:** [[pim]] — PIM và AIM là hai trạng thái của cùng một tài sản theo vòng đời
- **Managed in:** [[cde]]
- **Defined by:** [[information-requirements-hierarchy]] — AIR (Asset Information Requirements) quy định thông tin nào phải có trong AIM

## Nguồn

- [[raw/core/ISO_19650_Overview]] — [[summary_iso-19650-overview]]
- [[raw/core/ISO_19650-1]] — Clauses 5.6 + 3.3.9 `[ISO-CORE:verified]` — AIM là living model cập nhật qua operational life; receives info từ PIM khi close-out; comprises graphical models, non-graphical data, documentation — [[summary_iso-19650-1]]
- [[raw/core/ISO_19650-3]] — Toàn bộ quy trình cập nhật AIM qua trigger events, và aggregation sau mỗi chu kỳ (clause 5.8) `[ISO-CORE:structure]` — [[summary_iso-19650-3]]
