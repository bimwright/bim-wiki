---
title: "BEP — BIM Execution Plan"
aliases: ["BIM Execution Plan", "BEP", "Kế hoạch thực hiện BIM"]
tags: ["#bim", "#iso-19650", "#concept", "#bep"]
type: concept
source: "[[raw/core/ISO_19650_Overview]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# BEP — BIM Execution Plan

> **TL;DR:** BEP là tài liệu do delivery team lập, mô tả cách họ sẽ đáp ứng yêu cầu thông tin của Appointing Party; có hai phiên bản (pre-appointment và post-appointment).

## Khái niệm cốt lõi

- **Định nghĩa:** Tài liệu chi tiết hóa cách delivery team (lead appointed party) sẽ thực hiện quản lý thông tin, đáp ứng [[eir]] và [[information-requirements-hierarchy]] cho dự án (ISO 19650-2)
- **Hai phiên bản:**
  - **Pre-appointment BEP (Stage 3):** Lập trong giai đoạn tender response — chứa assessment về năng lực, phương pháp, kế hoạch tổng thể
  - **Post-appointment / Confirmed BEP (Stage 4):** Ký kết sau khi được chỉ định — chi tiết hóa với TIDP, MIDP, responsibility matrix cụ thể
- **Nội dung điển hình:**
  - Project standards và naming conventions
  - Software, hardware, CDE platform được sử dụng
  - [[loin]] cho từng deliverable
  - Roles & responsibilities (xem [[bim-delivery-roles]])
  - MIDP (Master Information Delivery Plan) và TIDPs
  - Quality control procedures
- **Bối cảnh Việt Nam:** Tài liệu QĐ 348/BXD đã được Việt hóa và đính kèm BEP Template (Phụ lục 03) (Xem QĐ 348).
- **Bối cảnh Việt Nam:** QĐ 348 còn chuẩn hóa mẫu Pre-BEP rút gọn cho tender / pre-appointment; tài liệu này tập trung vào control table, 7 nhóm nội dung tối thiểu và khối xác nhận để điền trực tiếp rồi xuất sang `.docx`. (source: [[summary_pre-bep-template-qd348]])

## Quan hệ

- **Parent:** [[bim]]
- **Responds to:** [[eir]] — BEP là response của delivery team đối với EIR
- **Contains:** MIDP (Master Information Delivery Plan), TIDPs (Task Information Delivery Plans)
- **Involves:** [[bim-delivery-roles]] — Lead Appointed Party chịu trách nhiệm lập BEP

## Nguồn

- [[raw/core/ISO_19650_Overview]] — [[summary_iso-19650-overview]]
- [[raw/core/ISO_19650-2]] — Clauses 5.3.2 (Pre-appointment), 5.4.1 (Post-appointment/confirmed) `[ISO-CORE:verified]` — cập nhật definition và quy định BEP là living document — [[summary_iso-19650-2]]
- [[raw/national-standards/VN/QD_348_BXD]] — Phụ lục 03 `[VN-BXD:verified]` — Cung cấp sẵn 8 biểu mẫu BEP (Pre-BEP và BEP) mẫu quốc gia dùng chung cho mọi dự án ở VN — [[summary_qd-348]]
- [[raw/national-standards/VN/templates/BEP_Template_QD348]] `[VN-BXD:verified]` — Mẫu điền sẵn chi tiết hóa toàn bộ khung BEP vận hành (biểu mẫu 01-08, placeholders triển khai) — [[summary_bep-template-qd348]]
- [[raw/national-standards/VN/templates/Pre_BEP_Template_QD348]] `[VN-BXD:verified]` — Mẫu Pre-BEP rút gọn cho tender / pre-appointment, gồm control table, 7 mục chính và khối xác nhận — [[summary_pre-bep-template-qd348]]
