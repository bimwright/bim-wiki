---
title: "ISO 19650-4 — Information Exchange"
aliases: ["ISO 19650 Part 4 summary", "ISO 19650-4:2022 tóm tắt"]
tags: ["#bim", "#iso-19650", "#iso-19650-4", "#standard", "#summary"]
type: summary
source: "[[raw/core/ISO_19650-4]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# ISO 19650-4 — Information Exchange

> **TL;DR:** Part 4 (Requirement Document) quản trị cấp độ vi mô, quy định quy trình 3 bước và 6 tiêu chí chất lượng (6 Cs) áp dụng cho **mỗi lượt Information Exchange** diễn ra bên trong vòng đời của Part 2 và Part 3.

## Nội dung tóm tắt

### Sự khác biệt cốt lõi (Part 4 vs Part 2/3)

`[ISO-CORE:verified]` Trong khi Parts 2 và 3 quy định khung quy trình toàn cảnh (Governance, sequence, roles), Part 4 Focus vào Quality Assurance. Nó bổ sung trực tiếp cho khung sườn của hệ thống nhằm quy định cách thức kiểm tra mức độ đáp ứng (Verify compliance) tại mỗi lần chuyển đổi trạng thái của [[information-container]].

### Quy trình Exchange 3 bước (Clauses 5 & 6)

Quá trình chia thành 3 Step, đồng thời quy định hai mốc Quyết định (Decision Gates):

1. **Bước 1: Mobilization & Information Production (5.1)**
   - Khởi tạo và test. Sản xuất trong trạng thái WIP (Work in progress).
   - *Decision A (Approve for sharing):* Do Task team (nhà sản xuất) tự kiểm duyệt. Nếu Passed, sang bước 2.
2. **Bước 2: Shared State (5.2)**
   - Phục vụ rà soát chéo (Coordination review) giữa các Task teams và Lead Appointed Party. Thông tin ở Shared State không mang tính xác thực cuối cùng (Not authoritative).
   - *Decision B (Authorize and accept for publication):* Quyết định mang tính hai phía. Phía Lead Appointed Party ủy quyền (Authorize) + Phía Appointing Party nghiệm thu (Accept). Nếu Passed, sang bước 3.
3. **Bước 3: Published State (5.3)**
   - Trở thành record pháp lý authoritative, nạp thẳng vào PIM/AIM.
   - Được định kỳ Archive khi có Revision mới ra đời.

*(Lưu ý: Nếu không Passed ở các Decision Gates, lỗi sẽ được xử lý qua quy trình Change Actions - Clause 5.4).*

### Các tiêu chí đánh giá (Các "6 Cs" - Clause 7)

`[ISO-CORE:structure]` Ở cả hai mốc Decision A và Decision B, các container đều phải đi qua 6 tiêu chuẩn rà soát chất lượng:
1. **CDE (Common Data Environment)**
2. **Conformance** (Sự phù hợp)
3. **Continuity** (Tính liên tục)
4. **Communication** (Khả năng truyền đạt)
5. **Consistency** (Tính nhất quán)
6. **Completeness** (Tính đầy đủ)

*(Xem chi tiết tại: [[exchange-criteria]]).*

### Tiêu chuẩn Open Schema (Annex A)

`[ISO-CORE:structure]` Annex A bổ sung cho tiêu chí Conformance (7.2), nhấn mạnh khuyến nghị ưu tiên dùng 'Open schemas' (ví dụ như IFC cho 3D Model, COBie cho Construction Data). File gốc/Định dạng Proprietary chỉ nên dùng khi thực sự cần thiết về mặt hợp đồng và phải được đính kèm theo định dạng Open.

## Quan hệ

- **Parent:** [[iso-19650]]
- **Updated concepts:** [[cde]], [[eir]], [[information-container]]
- **New concepts:** [[exchange-criteria]] (6 Cs)

## Nguồn

- [[raw/core/ISO_19650-4]] — Toàn bộ tư liệu được `[ISO-CORE:verified]` scope ở mảng Exchange, Open standards được khuyến khích mạnh mẽ.
