---
title: "BIM Delivery Roles (Appointing Party / Lead Appointed Party / Appointed Party)"
aliases: ["BIM roles", "Appointing Party", "Lead Appointed Party", "Appointed Party", "Vai trò BIM", "Bên chỉ định", "Bên được chỉ định"]
tags: ["#bim", "#iso-19650", "#concept", "#roles"]
type: concept
source: "[[raw/core/ISO_19650_Overview]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# BIM Delivery Roles

> **TL;DR:** ISO 19650-2 định nghĩa 3 vai trò cốt lõi trong delivery: Appointing Party (chủ — phát hành EIR), Lead Appointed Party (tổng thầu thông tin — lập BEP, MIDP), và Appointed Party (thầu phụ — thực hiện TIDP).

## Khái niệm cốt lõi

- **Appointing Party (Bên chỉ định):** Tổ chức/cá nhân có tài sản xây dựng, hoặc được ủy quyền quản lý tài sản. Phát hành [[eir]] và [[information-requirements-hierarchy]] (OIR/AIR/PIR). Nhận thông tin ở trạng thái Published từ [[cde]]. *Tương đương: chủ đầu tư, asset owner, client.*
- **Lead Appointed Party (Bên được chỉ định chính):** Tổ chức ký hợp đồng trực tiếp với Appointing Party. Chịu trách nhiệm tổng thể về thông tin: lập [[bep]], lập MIDP (Master Information Delivery Plan), phối hợp các Appointed Parties. *Tương đương: tổng thầu, principal designer, lead consultant.*
- **Appointed Party (Bên được chỉ định):** Tổ chức ký hợp đồng với Lead Appointed Party. Thực hiện TIDP (Task Information Delivery Plan) cho phạm vi công việc của mình. *Tương đương: thầu phụ, sub-consultant, specialist contractor.*

### Chuỗi chỉ định (appointment chain)

```
Appointing Party
  └── (appoints) Lead Appointed Party
        └── (appoints) Appointed Party 1
        └── (appoints) Appointed Party 2
        └── ...
```

- **Trong dự án lớn:** Có thể có nhiều chuỗi appointment song song (e.g., architect + engineer + contractor đều là Lead Appointed Parties riêng biệt)
- **Trong dự án nhỏ:** Có thể chỉ có Appointing Party + một Lead Appointed Party duy nhất

## Chi tiết / Triển khai

- **MIDP (Master Information Delivery Plan):** Lead Appointed Party lập — tổng hợp toàn bộ TIDPs thành lịch giao nộp thông tin tổng thể cho dự án
- **TIDP (Task Information Delivery Plan):** Appointed Party lập — chi tiết hóa thông tin họ sẽ tạo, format, timeline
- **Responsibility matrix:** Lead Appointed Party lập sau appointment (Stage 4) — map deliverables với người/tổ chức chịu trách nhiệm

## Quan hệ

- **Parent:** [[bim]]
- **Issues:** [[eir]] (Appointing Party), [[bep]] (Lead Appointed Party)
- **Works within:** [[cde]] — mọi thông tin đều chảy qua CDE

## Nguồn

- [[raw/core/ISO_19650_Overview]] — [[summary_iso-19650-overview]]
- [[raw/core/ISO_19650-1]] — Clauses 3.2.3–3.2.7 `[ISO-CORE:verified]` + Clause 8 `[ISO-CORE:structure]` — xác nhận definitions; task team (3.2.7); delivery team có thể assembled by appointing party; capability vs capacity distinction (3.3.18/19); 8 assessment criteria — [[summary_iso-19650-1]]
- [[raw/core/ISO_19650-2]] — Annex A `[ISO-CORE:verified]` — Information management assignment matrix map toàn bộ các Activity 5.1-5.8 cho 4 roles — [[summary_iso-19650-2]]
- [[raw/core/ISO_19650-3]] — Introduction `[ISO-CORE:structure]` — Vị trí Appointing party trong Part 3 lúc này là Asset owner, nhà vận hành hoặc outsourced FM — [[summary_iso-19650-3]]
- [[raw/core/ISO_19650-5]] — Clause 5.1 và Clause 9 `[ISO-CORE:structure]` — Khẳng định cần một "security governance lead" riêng có trách nhiệm đè trên lên framework thông thường. Quy định rõ nghĩa vụ áp tải Security requirement xuống cho các Appointed Parties. — [[summary_iso-19650-5]]
- [[raw/core/ISO_19650-6]] — Introduction `[ISO-CORE:verified]` — Định nghĩa khía cạnh H&S (chống thương vong, nguy hiểm) là một "collective responsibility" (trách nhiệm tập thể) do toàn bộ supply chain thực thi chung chứ không giao khoán cho duy nhất một role Appointed party nào — [[summary_iso-19650-6]]
- [[raw/national-standards/VN/QD_347_BXD]] — Khoản 4.1 `[VN-BXD:verified]` — Rẽ nhánh Appointed Party ra 2 chức danh thực thi: Kỹ thuật viên BIM (Modeller cho việc vẽ model cập nhật sau va chạm) và Điều phối BIM (Coordinator cho việc đầm chéo báo cáo giao cắt và chủ trì họp dung sai) — [[summary_qd-347]]
- [[raw/guidance/Revit-File-Handover-Guide]] — Quy định phân quyền rõ rệt lúc giao thoa CDE: Chỉ Kỹ thuật viên BIM (Modeler) có quyền thao tác kỹ thuật rọn rác trước cửa Gate; Cấp Quản lý (Leader hoặc BIM Coordinator) là người nắm quyền cầm "Checklist" soát thẻ Approve mở cho qua cửa Gate (WIP → Shared, Shared → Published). — [[summary_revit-handover]]
- [[raw/national-standards/VN/templates/BEP_Template_QD348]] `[VN-BXD:verified]` — Mẫu BEP cung cấp ma trận RACI và danh mục liên hệ/vai trò BIM để vận hành trách nhiệm theo từng bên tham gia dự án — [[summary_bep-template-qd348]]
- [[raw/national-standards/VN/templates/Pre_BEP_Template_QD348]] `[VN-BXD:verified]` — Mẫu Pre-BEP cũng có phần tổ chức BIM / trách nhiệm, dùng để chốt vai trò trước khi lập BEP đầy đủ — [[summary_pre-bep-template-qd348]]
