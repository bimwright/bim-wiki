---
title: "Comparison — BEP Template QĐ 348 Variants"
aliases: ["bep template qd348 variants comparison", "bep_template_qd348_variants"]
tags: ["#bim", "#vietnam", "#qd348", "#comparison", "#bep-template"]
type: comparison
source: "[[raw/national-standards/VN/templates/BEP_Template_QD348_V1_StandardFit]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# Comparison — BEP Template QĐ 348 Variants

> **TL;DR:** So sánh hai biến thể mẫu BEP theo QĐ 348: base (Markdown developer-friendly, có `[COMMENTARY]` và signature block) và V1_StandardFit (bám sát Phụ lục 03 gốc, dùng placeholder kiểu giấy điền tay, không commentary).

## Side-by-Side Comparison

| Khía cạnh | Base (`BEP_Template_QD348.md`, ~4,689 words) | V1_StandardFit (`BEP_Template_QD348_V1_StandardFit.md`, ~9,210 words) |
|---|---|---|
| **Placeholder syntax** | `{{PLACEHOLDER_NAME}}` (ALL_CAPS, descriptive — extract-friendly cho script) | `___ [Ghi <hint>]` (underscore + tiếng Việt hint — paper-form style, in điền tay) |
| **Bảng mở đầu** | `## Kiểm soát tài liệu` 10 trường (Tên dự án, Chủ đầu tư, Đơn vị lập BEP, EIR tham chiếu, CDE tham chiếu, Mã tài liệu, …) + `### Nhật ký phiên bản` 5 cột | Không có "Kiểm soát tài liệu". Chỉ có `### Phiên bản tài liệu` 4 cột (Hiệu chỉnh, Người lập, Phê duyệt, Ngày tháng) — bám đúng layout Phụ lục 03 |
| **Section 1 (Quy định áp dụng)** | Bảng 9 cột; cùng nhóm "trong nước" + "nước ngoài" | Cùng cấu trúc 9 cột; cùng nhóm |
| **Section 2 (Thông tin dự án)** | 2.1 Thông tin chung (5 trường) + 2.2 Tiến độ (4 cột có cột Ghi chú) | 2.1 (5 trường) + 2.2 (3 cột, không có Ghi chú) |
| **Section 3 (Mục tiêu BIM)** | 3.1 (4 cột: Mục tiêu / Chỉ số / Ghi chú) + 3.2 (5 cột có Giai đoạn + Đầu ra) | 3.1 (2 cột) + 3.2 (2 cột) — gọn hơn |
| **Section 4 (Tổ chức)** | `### 4.1 Danh sách liên hệ` + `### 4.2 Sơ đồ tổ chức BIM` (sub-section riêng) | Chỉ có `### Bảng 6. Danh sách liên hệ` — KHÔNG có sub-section "Sơ đồ tổ chức BIM" |
| **Section 5 — 7** | Cùng cấu trúc 5.1/5.2/5.3 + 6 (LOD) + 7.1–7.9 (9 sub-sections phối hợp) | Cùng cấu trúc 5.1/5.2/5.3 + 6 + 7.1–7.9 |
| **Biểu mẫu 01–08** | 8 biểu mẫu (RACI, MIDP, LOD, CDE, Naming, Tần suất họp, Kiểm tra mô hình) | 8 biểu mẫu cùng tên, cùng số thứ tự |
| **Signature block** | `## Xác nhận` cuối tài liệu (bảng chữ ký các bên) | KHÔNG có signature block |
| **`[COMMENTARY]` tags** | Có (giải thích placeholder syntax, layout Markdown vs `.docx`, bảng tổ chức trong `.md`) | Không có (verified: grep `[COMMENTARY]` returns 0 matches) |
| **`[VN-BXD:verified]` tags** | Có rải đều mọi section | Có rải đều mọi section (preserved) |
| **Tổng word count** | ~4,689 words | ~9,210 words (gấp ~2× base do placeholder `___ [Ghi <hint>]` dài hơn `{{NAME}}` và nhiều cell hơn) |

## Khi nào dùng base, khi nào dùng V1?

- **Dùng base** khi: team có IT support muốn extract field qua script (regex `\{\{(\w+)\}\}`); cần `[COMMENTARY]` để onboarding/documenting; cần signature block cho formal submission ra cơ quan thẩm quyền.
- **Dùng V1_StandardFit** khi: workflow giấy/in điền tay; cần baseline bám đúng layout Phụ lục 03 QĐ 348 để dễ đối chiếu khi audit; không cần extraction qua script.

## Khái niệm cốt lõi

- Cả hai biến thể có **cùng cấu trúc logic** — 8 sections (1–7 + Biểu mẫu) và 8 biểu mẫu vận hành (01–08). Khác biệt nằm ở **presentation layer**, không ở thông tin yêu cầu BIM.
- Base **bổ sung** so với Phụ lục 03 gốc: bảng `## Kiểm soát tài liệu` 10 trường, `### 4.2 Sơ đồ tổ chức BIM`, `## Xác nhận` (signature block), và rải `[COMMENTARY]` để hướng dẫn cách dùng. V1 **bỏ tất cả các bổ sung này** để bám sát Phụ lục 03.
- Word count V1 lớn hơn base ~2× **không** phản ánh thông tin nhiều hơn — phản ánh placeholder `___ [Ghi <hint>]` dài hơn (mỗi cell có hint tiếng Việt) cộng các bảng có nhiều dòng mẫu hơn (vd. Biểu mẫu 01 RACI).

## Quan hệ

- **Parent:** [[summary_bep-template-qd348]]
- **Implements:** [[bep]], [[eir]], [[cde]], [[midp-tidp]], [[lod-vn]]
- **Operational roles:** [[bim-delivery-roles]]

## Nguồn

- [[raw/national-standards/VN/templates/BEP_Template_QD348]] — Base (Markdown developer-friendly, ~4,689 words). `[VN-BXD:verified]` + `[COMMENTARY]`.
- [[raw/national-standards/VN/templates/BEP_Template_QD348_V1_StandardFit]] — V1 Standard-Fit (paper-form, bám Phụ lục 03, ~9,210 words). `[VN-BXD:verified]`.
