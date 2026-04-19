---
title: "CDE — Common Data Environment"
aliases: ["Common Data Environment", "CDE", "Môi trường dữ liệu chung"]
tags: ["#bim", "#iso-19650", "#concept", "#cde"]
type: concept
source: "[[raw/core/ISO_19650_Overview]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# CDE — Common Data Environment

> **TL;DR:** Môi trường dữ liệu chung (CDE) là hệ thống quản lý và chia sẻ thông tin của dự án BIM, với workflow 4 trạng thái: WIP → Shared → Published → Archive.

## Khái niệm cốt lõi

- **Định nghĩa:** Nguồn thông tin duy nhất (single source of truth) được thỏa thuận để thu thập, quản lý và phổ biến mọi tài liệu, mô hình thông tin cho toàn dự án/tài sản (ISO 19650-1, clause 3.3.15)
- **4 trạng thái CDE workflow:**
  1. **WIP (Work In Progress):** Thông tin đang được tạo/chỉnh sửa — chỉ tác giả truy cập
  2. **Shared:** Thông tin đã chia sẻ để review/tham chiếu bởi delivery team
  3. **Published:** Thông tin được phê duyệt chính thức — Appointing Party truy cập
  4. **Archive:** Thông tin đã kết thúc vòng đời hoạt động — lưu trữ tham chiếu
- **Vai trò trong ISO 19650:** CDE là xương sống của mọi trao đổi thông tin — mọi state transition (WIP→Shared→Published) đều phải đi qua CDE với tiêu chí "6 Cs" (Part 4)
- **Không bắt buộc là 1 phần mềm cụ thể:** CDE là *concept* — có thể triển khai bằng nhiều platform khác nhau

## Chi tiết / Triển khai

- **State transition criteria (Part 4):** Mỗi transition có tiêu chí kiểm tra: Conformance, Continuity, Communication, Consistency, Completeness, và CDE status codes đúng
- **Security overlay (Part 5):** CDE phải tuân thủ security management plan — thông tin nhạy cảm cần kiểm soát truy cập bổ sung
- **H&S integration (Part 6):** Risk register và H&S data được share qua CDE theo 5-step cycle

## Quan hệ

- **Parent:** [[iso-19650]]
- **Used by:** [[pim]], [[aim]] — cả hai đều được quản lý trong CDE
- **Related:** [[bim-delivery-roles]] — Appointing Party nhận thông tin từ Published state; [[eir]] — Exchange Information Requirements định nghĩa cái gì được publish lên CDE

## Nguồn

- [[raw/core/ISO_19650_Overview]] — [[summary_iso-19650-overview]]
- [[raw/core/ISO_19650-1]] — Clause 12 `[ISO-CORE:verified/structure]` — cụ thể hóa **CDE Solution** (technology platform) vs **CDE Workflow** (organizational process); Clause 3.3.15 definition verified; status code scheme reference sang [[uk-national-annex]] — [[summary_iso-19650-1]]
- [[raw/core/ISO_19650-2]] — Clauses 5.1.7 (establish CDE workflow) và 5.6, 5.7 (State mapping) `[ISO-CORE:verified]` — [[summary_iso-19650-2]]
- [[raw/core/ISO_19650-3]] — Clause 5.1.9 và 5.1.10 (tích hợp enterprise systems CAFM/CMMS vào CDE) `[ISO-CORE:structure]` — CDE phục vụ như lõi Published chứa AIM liên tục, phải giao tiếp với hệ thống doanh nghiệp — [[summary_iso-19650-3]]
- [[raw/core/ISO_19650-4]] — Định nghĩa quá trình thay đổi trạng thái trong CDE phải đi qua 2 mốc Decision A & Decision B (Clause 6), thông qua sự giám định của 6 tiêu chuẩn 6 Cs (Clause 7) `[ISO-CORE:structure]` — [[summary_iso-19650-4]]
- [[raw/national-standards/VN/QD_348_BXD]] — Khoản 3.2 `[VN-BXD:verified]` — Chuẩn hóa Workflow 4 vùng CDE tại Việt Nam kèm theo hệ mã trạng thái kiểm định riêng (S0-S4, A1-An, B1-Bn) — [[summary_qd-348]]
- [[raw/guidance/Revit-File-Handover-Guide]] — Thực địa hóa CDE vào môi trường thao tác phần mềm: Gate 1 (WIP → Shared) Audit & rọn rác nội bộ; Gate 2 (Shared → Published) xử lý Sheet Sets, Design options để bảo vệ legal form. — [[summary_revit-handover]]
- [[raw/national-standards/VN/templates/BEP_Template_QD348]] `[VN-BXD:verified]` — Biểu mẫu 05 quy định ma trận phân quyền CDE theo các vùng WIP/Shared/Published/Archived và theo chủ thể tham gia — [[summary_bep-template-qd348]]
- [[raw/national-standards/VN/templates/Pre_BEP_Template_QD348]] `[VN-BXD:verified]` — Mẫu Pre-BEP có mục quản lý thông tin/CDE, làm rõ platform, workflow và access control trước khi chốt BEP — [[summary_pre-bep-template-qd348]]
