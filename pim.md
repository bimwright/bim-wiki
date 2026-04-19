---
title: "PIM — Project Information Model"
aliases: ["Project Information Model", "PIM"]
tags: ["#bim", "#iso-19650", "#concept", "#information-model"]
type: concept
source: "[[raw/core/ISO_19650_Overview]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# PIM — Project Information Model

> **TL;DR:** PIM là mô hình thông tin được tích lũy trong giai đoạn thiết kế và thi công; khi bàn giao vận hành, PIM được chuyển đổi thành AIM.

## Khái niệm cốt lõi

- **Định nghĩa:** Information model phát triển trong giai đoạn delivery (thiết kế, thi công, commissioning) của dự án (ISO 19650-1, clause 3.3.10)
- **Giai đoạn:** Tương ứng ISO 19650-2 (Delivery phase) — từ assessment & need đến project close-out
- **Nội dung:** Toàn bộ thông tin của dự án tích lũy qua 8 giai đoạn — bao gồm mô hình, tài liệu, dữ liệu, bản vẽ, thông số kỹ thuật
- **Quản lý qua:** [[cde]] — CDE lưu trữ và quản lý tất cả container thông tin của PIM với 4 trạng thái (WIP→Shared→Published→Archive)
- **Kết quả cuối:** Authorized PIM (stage 5.7) → handover sang [[aim]] (stage 5.8 / đầu ISO 19650-3)

## Chi tiết / Triển khai

- **Authorized PIM (Stage 5.7):** PIM đã được Appointing Party phê duyệt — đây là milestone chính trước close-out
- **PIM → AIM transition:** Xảy ra tại stage 5.8 (project close-out); AIM được init từ PIM và tiếp tục được cập nhật trong suốt vòng đời vận hành
- **Định nghĩa thông tin cần có trong PIM:** Thông qua [[information-requirements-hierarchy]] (OIR → PIR → EIR)

## Quan hệ

- **Parent:** [[bim]]
- **Alternative:** [[aim]] — AIM là "PIM phiên bản vận hành"; PIM handover thành AIM
- **Managed in:** [[cde]]
- **Defined by:** [[information-requirements-hierarchy]] — EIR và PIR quy định thông tin nào phải có trong PIM

## Nguồn

- [[raw/core/ISO_19650_Overview]] — [[summary_iso-19650-overview]]
- [[raw/core/ISO_19650-1]] — Clause 5.7 + 3.3.10 `[ISO-CORE:verified]` — xác nhận 2-stage PIM: Design Intent Model (design phase) và Virtual Construction Model (construction phase); PIM evolves progressively qua delivery process — [[summary_iso-19650-1]]
- [[raw/core/ISO_19650-2]] — Clause 5.8.1 `[ISO-CORE:verified]` — quy định Archive PIM vào cuối dự án để tạo record as-delivered và chuyển sang AIM — [[summary_iso-19650-2]]
- [[raw/core/ISO_19650-3]] — Clause 4.2 `[ISO-CORE:structure]` — PIM được produced bởi sự kiện trigger kích hoạt một delivery phase (Part 2), làm input gộp vào AIM tại lúc handover — [[summary_iso-19650-3]]
