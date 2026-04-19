---
title: "Summary — BEP Template theo QĐ 348"
aliases: ["summary BEP template QĐ 348", "summary_bep-template-qd348"]
tags: ["#bim", "#vietnam", "#qd348", "#summary", "#bep-template"]
type: summary
source: "[[raw/national-standards/VN/templates/BEP_Template_QD348]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# Summary — BEP Template theo QĐ 348

> **TL;DR:** Mẫu BEP theo QĐ 348 chuẩn hoá đầy đủ cấu trúc lập kế hoạch BIM cho dự án Việt Nam: kiểm soát tài liệu, mục tiêu áp dụng BIM, vai trò trách nhiệm, CDE, MIDP/TIDP, LOD, naming convention, tần suất phối hợp và kiểm tra mô hình.

## Nội dung tóm tắt

- Tài liệu là mẫu điền sẵn theo `Phụ lục 03` của `QĐ 348/QĐ-BXD`, nhấn mạnh BEP phải được chủ đầu tư phê duyệt và TIDP/MIDP được quản lý trên CDE.
- Cấu trúc mẫu gồm 8 mục chính theo workflow triển khai thực tế:
  - Quy định áp dụng
  - Thông tin dự án
  - Mục tiêu và nội dung áp dụng BIM
  - Tổ chức và trách nhiệm
  - Phạm vi công việc, sản phẩm, kế hoạch chuyển giao
  - LOD
  - Quy định phối hợp
  - Bộ biểu mẫu vận hành
- Nhóm biểu mẫu đính kèm rất đầy đủ cho thực hành dự án:
  - Biểu mẫu 01: ma trận phân công trách nhiệm (RACI)
  - Biểu mẫu 02: kế hoạch trao đổi thông tin phối hợp
  - Biểu mẫu 03: bảng LOD theo cấu kiện
  - Biểu mẫu 04: MIDP tổng thể
  - Biểu mẫu 05: phân quyền CDE theo vùng dữ liệu
  - Biểu mẫu 06: quy ước đặt tên (tham chiếu ISO 19650-2)
  - Biểu mẫu 07: tần suất họp/trao đổi thông tin
  - Biểu mẫu 08: checklist kiểm tra mô hình
- Mẫu này là khung triển khai thực thi (implementation-ready), dùng nhiều placeholder `{{...}}` để đội dự án điền trực tiếp mà không cần thiết kế lại biểu mẫu tài liệu.
- Nguồn có gắn rõ các nhãn provenance:
  - `[VN-BXD:verified]` cho các nội dung bám sát QĐ 348.
  - `[COMMENTARY]` cho các phần chuẩn hóa markdown/phần bổ sung nhằm tăng khả năng dùng trong repo và khi xuất `.docx`.

## Chi tiết / Triển khai

- Về logic quản lý thông tin, mẫu giữ đúng đường dây ISO 19650 nhưng diễn giải theo ngữ cảnh Việt Nam:
  - EIR làm đầu vào yêu cầu.
  - BEP là kế hoạch phản hồi và tổ chức thực thi.
  - TIDP/MIDP quản lý timeline và trách nhiệm chuyển giao.
  - CDE là nền tảng điều phối dữ liệu và quyền truy cập.
- Về quản trị dữ liệu, mẫu tách rõ:
  - Quy định phối hợp kỹ thuật (phần mềm, hệ tọa độ, đơn vị đo, cấu trúc bản vẽ).
  - Quy định trao đổi dữ liệu (format gốc/trao đổi, naming, retention, tần suất chia sẻ).
  - Quy trình kiểm tra và nghiệm thu mô hình trước khi phát hành.
- Về naming convention, mẫu đặt khung mã hóa nhiều thành phần (project, originator, level/location, role, number, suitability, revision), tạo nền để đồng bộ quản lý tài liệu giữa các bên.

## Quan hệ

- **Parent:** [[summary_qd-348]]
- **Related standards context:** [[iso-19650]]
- **Implements:** [[bep]], [[eir]], [[cde]], [[midp-tidp]], [[lod-vn]]
- **Operational roles:** [[bim-delivery-roles]]

## Nguồn

- [[raw/national-standards/VN/templates/BEP_Template_QD348]] — Mẫu BEP đầy đủ theo QĐ 348, gồm 8 mục chính và 8 biểu mẫu vận hành.
- [[raw/national-standards/VN/QD_348_BXD]] — Văn bản quyết định và khung yêu cầu chuẩn hoá cấp quốc gia — [[summary_qd-348]]

### Biến thể

- **V1_StandardFit:** So sánh chi tiết tại [[bep-template-qd348-variants]] — bám sát Phụ lục 03 hơn (placeholder `___ [Ghi <hint>]` thay vì `{{...}}`, không có `## Kiểm soát tài liệu`, không có `### 4.2 Sơ đồ tổ chức BIM`, không có signature block, không có `[COMMENTARY]`) (source: [[raw/national-standards/VN/templates/BEP_Template_QD348_V1_StandardFit]]).
