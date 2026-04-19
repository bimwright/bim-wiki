---
title: "ISO 19650-5 — Security-Minded Approach"
aliases: ["ISO 19650 Part 5 summary", "ISO 19650-5:2020 tóm tắt"]
tags: ["#bim", "#iso-19650", "#iso-19650-5", "#standard", "#summary", "#security"]
type: summary
source: "[[raw/core/ISO_19650-5]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# ISO 19650-5 — Security-Minded Approach

> **TL;DR:** Part 5 không phải là một quy trình hoạt động độc lập mà là một "Lớp phủ bảo mật" (Security Overlay) được áp dụng đè lên các quy trình của Part 2 và Part 3, hướng dẫn tổ chức cách tiếp cận rủi ro an ninh thông tin một cách có ý thức (security-minded) đối với môi trường BIM.

## Nội dung tóm tắt

### Sự khác biệt cốt lõi (Overlay Framework)

`[ISO-CORE:verified]` Khác với ISO/IEC 27001 vốn chỉ bọc bảo mật cho nội bộ một tổ chức, BIM đòi hỏi làm việc liên tổ chức (collaborative sharing cross-organizations). Do đó, Part 5 đưa ra framework để đảm bảo thông tin nhạy cảm chia sẻ qua Chuỗi cung ứng (Supply chain) vẫn an toàn nhưng không thiết lập rào cản quá lớn khiến các doanh nghiệp vừa và nhỏ (SME) không thể bước vào dự án. 

Bảo mật ở đây không chỉ là "Mật của quốc gia" mà bao gồm 6 rủi ro: National security, Commercial (thương mại), Personal data (dữ liệu cá nhân), Reputational (danh tiếng), Financial (Tài chính), và Operational.

### Khung quy trình 4 giai đoạn bảo mật

Được thẩm định liên tục trong suốt vòng đời của dự án hoặc tài sản:

1. **Bước 1: [[sensitivity-assessment]] (Clause 4)**
   - Bước Triage quyết định: Đánh giá xem dự án/tài sản có cần lớp bảo vệ security-minded không? Nếu bước này chốt là "Không", thì dưng toàn bộ Part 5, chỉ cần lưu hồ sơ (Record review lại sau).
2. **Bước 2: Security Strategy (Clause 5 & 6)**
   - Nếu "Có" ở Bước 1. Bắt đầu thiết lập tính chịu trách nhiệm (Governance).
   - Đánh giá Risk và đề ra các chiến lược giảm thiểu rủi ro (Mitigation measures) và lập hồ sơ rủi ro chấp nhận được (Tolerated risks).
3. **Bước 3: Security Management Plan (Clause 7)**
   - Bản kế hoạch Vận hành - áp dụng kiểm soát Logistics (nhân sự, vật lý, IT), kiểm soát việc chia sẻ thông tin cho bên thứ 3 và quy trình Audit/Monitoring.
4. **Bước 4: Breach/Incident Management Plan (Clause 8)**
   - Lập kịch bản rủi ro: Quy trình phát hiện, khoanh vùng cô lập (containment), phục hồi và hậu xét nghiệm (review after breach).

### Chuỗi cung ứng và Các bên (Clause 9)

Part 5 có một Clause quy định đặc quyền riêng cho việc đùn các yêu cầu bảo mật xuống phía dưới Supply Chain: Trước hợp đồng (Tender) → Trong tài liệu hợp đồng (Nạp vào [[eir]]) → Suốt quá trình cấp quyền truy cập → Và quy trình tước quyền ở lúc kết thúc hợp đồng (Thu hồi tài liệu, rà soát Retentions).

## Quan hệ

- **Parent:** [[iso-19650]]
- **Overlays on:** [[summary_iso-19650-2]], [[summary_iso-19650-3]]
- **New concepts:** [[sensitivity-assessment]]

## Nguồn

- [[raw/core/ISO_19650-5]] — Tổng hợp các clause, Annex A-D về Open CDE risk và Built environment context `[ISO-CORE:structure]`.
