---
title: "EIR — Exchange Information Requirements"
aliases: ["Exchange Information Requirements", "EIR", "Yêu cầu trao đổi thông tin"]
tags: ["#bim", "#iso-19650", "#concept", "#eir", "#information-requirements"]
type: concept
source: "[[raw/core/ISO_19650_Overview]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# EIR — Exchange Information Requirements

> **TL;DR:** EIR là tài liệu do Appointing Party lập, specify chính xác thông tin nào (LOIN, format, timing) cần nhận từ delivery team tại từng giai đoạn giao nộp.

## Khái niệm cốt lõi

- **Định nghĩa:** Yêu cầu thông tin được lập bởi hoặc thay mặt cho Appointing Party, định nghĩa thông tin cần được trao đổi trong quá trình delivery (ISO 19650-1, clause 3.3.6)
- **Vị trí trong hierarchy:** OIR → [AIR/PIR] → **EIR** → BEP (EIR là cầu nối giữa yêu cầu tổ chức và deliverables dự án)
- **Nội dung điển hình:**
  - [[loin]] cho từng information container / deliverable
  - Định dạng file và naming convention
  - CDE platform và workflow yêu cầu
  - Timeline giao nộp (coordination với MIDP/TIDP)
  - Tiêu chí acceptance (liên kết với "6 Cs" của Part 4)
- **Khi phát hành:** Được đính kèm trong tender documentation (Stage 2) — mỗi appointment có thể có EIR riêng trong dự án phức tạp
- **Delivery team dùng EIR để lập:** [[bep]] — BEP là response chính thức đối với EIR

## Quan hệ

- **Parent:** [[information-requirements-hierarchy]]
- **Issued by:** [[bim-delivery-roles]] — Appointing Party phát hành EIR
- **Responded to by:** [[bep]] — Lead Appointed Party lập BEP đáp ứng EIR
- **Specifies:** [[loin]] — LOIN trong EIR xác định mức độ thông tin yêu cầu

## Nguồn

- [[raw/core/ISO_19650_Overview]] — [[summary_iso-19650-overview]]
- [[raw/core/ISO_19650-1]] — Clause 5.5 `[ISO-CORE:verified/structure]` — 3 content categories: Technical (software, LOIN, formats) · Management (protocols, CDE) · Commercial (deliverables, milestones); lean principle: chỉ yêu cầu thông tin tối thiểu; EIR developed per appointment — [[summary_iso-19650-1]]
- [[raw/core/ISO_19650-2]] — Clauses 5.2.1 (Appointing party EIR), 5.4.3 (Lead appointed party EIR) `[ISO-CORE:verified]` — Thêm khái niệm EIR cascade xuyên suốt chuỗi cung ứng (supply chain) — [[summary_iso-19650-2]]
- [[raw/core/ISO_19650-3]] — Clause 5.2 (EIR cho vận hành) EIR được xây dựng từ AIR (thay vì PIR) cho mỗi lần phục vụ trigger event `[ISO-CORE:structure]` — [[summary_iso-19650-3]]
- [[raw/core/ISO_19650-4]] — Clause 7.6 `[ISO-CORE:structure]` — EIR đóng vai trò là thước đo đối chiếu (benchmark) cho mức độ Completeness của gói thông tin trao đổi — [[summary_iso-19650-4]]
- [[raw/national-standards/VN/QD_348_BXD]] — Phụ lục 02 `[VN-BXD:verified]` — Cung cấp Template EIR (7 hạng mục) theo biểu mẫu quy chuẩn quốc gia — [[summary_qd-348]]
- [[raw/national-standards/VN/templates/BEP_Template_QD348]] `[VN-BXD:verified]` — Mẫu BEP có trường tham chiếu EIR và liên kết trực tiếp giữa yêu cầu EIR với kế hoạch thực thi BIM — [[summary_bep-template-qd348]]
- [[raw/national-standards/VN/templates/Pre_BEP_Template_QD348]] `[VN-BXD:verified]` — Mẫu Pre-BEP giữ trường `Căn cứ EIR` và gắn mục tiêu BIM với hồ sơ mời thầu / EIR đầu vào — [[summary_pre-bep-template-qd348]]
