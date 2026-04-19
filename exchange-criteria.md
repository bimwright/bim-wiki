---
title: "Exchange Criteria (6 Cs)"
aliases: ["6 Cs", "Exchange Criteria", "Criteria for reviewing an information exchange"]
tags: ["#bim", "#iso-19650", "#iso-19650-4", "#concept"]
type: concept
source: "[[raw/core/ISO_19650-4]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# Exchange Criteria (6 Cs)

> **TL;DR:** "6 Cs" là thuật ngữ thực hành phổ biến chỉ 6 tiêu chuẩn chất lượng (CDE, Conformance, Continuity, Communication, Consistency, Completeness) áp dụng bắt buộc tại Decision A và Decision B trong quá trình trao đổi thông tin thuộc chuẩn ISO 19650-4.

## Khái niệm cốt lõi

- **Định nghĩa:** Bộ tiêu chí phục vụ cho việc ra quyết định chuyển tiếp trạng thái (từ WIP → Shared và Shared → Published) của một [[information-container]]. Đảm bảo chất lượng của Exchange đúng cam kết từ [[eir]].
- Trong ISO 19650-4 (Clause 7), chúng bao gồm:
  1. **CDE (7.1):** Các attributes có được gán đủ trên CDE không? Phải kèm Unique ID tĩnh, Metadata, Status Code, Revision và theo tuân thủ quy trình CDE Workflow.
  2. **Conformance (7.2):** Tính tuân thủ. Data Format có open và matching với schema yêu cầu từ EIR không (VD: IFC, XLSX)? Đã được validate phần mềm chưa?
  3. **Continuity (7.3):** Đặc trưng về tính xuyên suốt/liên tục — IDs đối tượng (object IDs) của lần giao nộp này có mapping với các bản nộp trước (ví dụ lúc PIM sang AIM) không? Khái niệm/Định nghĩa có bị thay đổi đột ngột làm dứt gãy chuỗi dữ liệu?
  4. **Communication (7.4):** Sự rõ ràng truyền đạt. Người dùng phía nhận có mở được đọc thông tin không? Bảng biểu có tường minh không? Kèm đủ Document note/metadata diễn giải?
  5. **Consistency (7.5):** Tính nhất quán bên trong và bên ngoài — Thống nhất giữa các bộ phận: Xử lý Clash Detection (không gian hẹp), thống nhất đơn vị SI, và dung hòa Spec Conflict.
  6. **Completeness (7.6):** Tính đầy đủ — Check xem List Object, LOIN, Metadata, Attributes đã đủ (100% fulfill) so với yêu cầu ban đầu của EIR hay chưa.

## Chi tiết / Triển khai

- **Proportionality (Tương xứng với mức độ):** Theo thiết kế chuẩn ISO, một dự án nhỏ mức độ áp dụng của 6 tiêu chí này có thể được lược bớt nhanh nếu thấy "not applicable", tuy nhiên luôn phải qua list này để đánh giá rủi ro (Clause 6.3).
- **Exceptions (6.4):** Khi rơi vào diện khẩn cấp (Emergency / cần ra quyết định đột xuất không thể chờ đủ 6 tiêu chí), thì exception phải được log lại và trở thành một issue theo change action, ngăn chặn việc lợi dụng exception bỏ qua workflow chuẩn.

## Quan hệ

- **Parent:** [[iso-19650]]
- **Applies to:** [[information-container]] và [[cde]] workflow
- **Checks against:** [[eir]]
- **Provides input to:** Clause 5.4 Change Actions khi phát hiện lỗi qua việc checking 6 Cs.

## Nguồn

- [[raw/core/ISO_19650-4]] — Nền tảng cốt lõi của Clause 7 (Criteria for reviewing an information exchange). Note: 6 Cs là từ lóng ngành công nghiệp, không phải thuật ngữ ISO chính quy nhưng concept hoàn toàn ánh xạ chuẩn `[ISO-CORE:structure]`.
