---
title: "Comparison — Pre-BEP Template QĐ 348 Variants"
aliases: ["pre-bep template qd348 variants comparison", "pre_bep_template_qd348_variants"]
tags: ["#bim", "#vietnam", "#qd348", "#comparison", "#pre-bep-template"]
type: comparison
source: "[[raw/national-standards/VN/templates/Pre_BEP_Template_QD348_V1_StandardFit]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# Comparison — Pre-BEP Template QĐ 348 Variants

> **TL;DR:** So sánh hai biến thể Pre-BEP QĐ 348: base (Markdown developer-friendly với bảng `Thông tin tài liệu`, sub-section 7.1/7.2, signature block, `[COMMENTARY]`) và V1_StandardFit (bám sát Mẫu số 6a gốc, placeholder kiểu giấy điền tay, không signature/commentary). Cùng 7 mục nội dung tối thiểu.

## Side-by-Side Comparison

| Khía cạnh | Base (`Pre_BEP_Template_QD348.md`, ~1,273 words) | V1_StandardFit (`Pre_BEP_Template_QD348_V1_StandardFit.md`, ~1,291 words) |
|---|---|---|
| **Placeholder syntax** | `{{PLACEHOLDER_NAME}}` (ALL_CAPS, descriptive — extract-friendly) | `___ [Ghi <hint>]` (underscore + tiếng Việt hint — paper-form, in điền tay) |
| **Khối thông tin mở đầu** | `## Thông tin tài liệu` — Markdown table 10 trường (Tên dự án, Gói thầu, Chủ đầu tư, Đơn vị lập Pre-BEP, Người phụ trách, Phiên bản, Ngày lập, Tình trạng, Căn cứ EIR, Ghi chú) | KHÔNG có table — chỉ 5 inline fields (Tên dự án, Chủ đầu tư, Nhà thầu/Đơn vị lập, Ngày lập, Phiên bản) theo phong cách Mẫu số 6a |
| **Section 1 (Mục tiêu BIM)** | Markdown table 5 cột (STT / Mục tiêu / Nguồn từ EIR / Chấp thuận-sửa đổi / Ghi chú) | Bullet list 3 dòng "Mục tiêu do CĐT nêu" + 1 inline "Chấp thuận / sửa đổi" — không bảng |
| **Section 2 (Nội dung áp dụng BIM)** | Markdown table 5 cột (STT / Nội dung / Tính chất / Chấp nhận-xác nhận / Ghi chú) | Markdown table 4 cột (bỏ cột Ghi chú) |
| **Section 3.2 (Phối hợp + xung đột)** | Markdown table 6 hàng (federation / chu kỳ / phần mềm / phương pháp clash / ngưỡng ưu tiên / ghi nhận issue) | 4 inline fields (phần mềm, tần suất, phương pháp clash, quy trình issue) — bỏ "ngưỡng ưu tiên" |
| **Section 6 (Quy trình QLTT)** | 6.1 (4 cột table cộng tác) + 6.2 (5 cột table CDE) + 6.3 (5 cột table QA) | 6.1 (1 inline field) + 6.2 (2 inline fields CDE) + 6.3 (1 inline field QA) — bỏ table |
| **Section 7 sub-sections** | `### 7.1 Sơ đồ tổ chức BIM` + `### 7.2 Hồ sơ năng lực nhân sự BIM chủ chốt` | KHÔNG có sub-sections — chỉ 1 table tổ chức |
| **Signature block** | `## Xác nhận` 5 cột × 3 hàng (Đơn vị lập / Đơn vị kiểm tra / Chủ đầu tư) | KHÔNG có signature block |
| **`[COMMENTARY]` tags** | 4 occurrences (lines 5 / 79 / 126 / 144) — giải thích placeholder, ma trận RACI rút gọn, sơ đồ tổ chức trong `.md`, signature block | 0 (verified by grep) |
| **`[VN-BXD:verified]` tags** | Có rải đều mọi section (preserved từ Mẫu số 6a) | Có rải đều mọi section (preserved) |
| **Tổng word count** | ~1,273 words | ~1,291 words (gần tương đương — placeholder dài hơn cân bằng với việc V1 bỏ commentary + signature) |

## Khi nào dùng base, khi nào dùng V1?

- **Dùng base** khi: cần extract field qua script (regex `\{\{(\w+)\}\}`), cần `### 7.2 Hồ sơ năng lực nhân sự` để chứng minh capability trong tender response, cần signature block khi nộp formal cho Chủ đầu tư.
- **Dùng V1_StandardFit** khi: workflow giấy/in điền tay; cần baseline bám đúng Mẫu số 6a QĐ 348 để đối chiếu khi audit; tender response sơ bộ chưa cần chứng minh năng lực nhân sự chi tiết.

## Khái niệm cốt lõi

- Cả hai biến thể có **cùng 7 mục nội dung tối thiểu** theo Mẫu số 6a (mục tiêu BIM, nội dung áp dụng, chiến lược mô hình, LOD, ma trận trách nhiệm, quy trình QLTT, vai trò BIM). Khác biệt nằm ở **mức độ Markdown-hóa** và **bổ sung thực hành** ngoài Mẫu số 6a.
- Base **bổ sung** so với Mẫu số 6a gốc: bảng `## Thông tin tài liệu` 10 trường, sub-section `7.2 Hồ sơ năng lực nhân sự`, signature block `## Xác nhận`, và 4 `[COMMENTARY]` blocks. V1 **bỏ tất cả các bổ sung này** để bám sát Mẫu số 6a.
- Khác mẫu BEP variant: word count Pre-BEP V1 ≈ base (1.4% diff) — không có hiện tượng V1 phình ra như BEP V1_StandardFit (gấp 2× base). Nguyên nhân: Pre-BEP base đã rất gọn (1,273 words); V1 bỏ một số table nhưng placeholder paper-form dài hơn `{{...}}` → bù trừ.

## Quan hệ

- **Parent:** [[summary_pre-bep-template-qd348]]
- **Sibling variant comparison:** [[bep-template-qd348-variants]] — comparison cùng pattern cho mẫu BEP đầy đủ (base vs V1_StandardFit). Pre-BEP variant có cùng 5 differences (placeholder, bảng mở đầu, sub-sections, signature, commentary) nhưng word count gần bằng nhau thay vì gấp đôi.
- **Implements:** [[bep]], [[eir]], [[cde]], [[lod-vn]]
- **Operational roles:** [[bim-delivery-roles]]

## Nguồn

- [[raw/national-standards/VN/templates/Pre_BEP_Template_QD348]] — Base (Markdown developer-friendly, ~1,273 words, 4 `[COMMENTARY]`). `[VN-BXD:verified]` + `[COMMENTARY]`.
- [[raw/national-standards/VN/templates/Pre_BEP_Template_QD348_V1_StandardFit]] — V1 Standard-Fit (paper-form, bám Mẫu số 6a, ~1,291 words, 0 `[COMMENTARY]`). `[VN-BXD:verified]`.
