---
title: "ISO 19650-2 — Delivery Phase of the Assets"
aliases: ["ISO 19650 Part 2 summary", "ISO 19650-2:2018 tóm tắt"]
tags: ["#bim", "#iso-19650", "#iso-19650-2", "#standard", "#summary"]
type: summary
source: "[[raw/core/ISO_19650-2]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# ISO 19650-2 — Delivery Phase of the Assets

> **TL;DR:** Part 2 là phần "Requirements document" (sử dụng "shall"), xác định quy trình 8 bước bắt buộc cho việc quản lý thông tin trong suốt giai đoạn delivery (thiết kế và thi công) của tài sản, tập trung mạnh vào các mốc đấu thầu, chỉ định, và sản xuất thông tin cộng tác.

## Nội dung tóm tắt

### Tổng quan quy trình 8 bước (Clause 4)

`[ISO-CORE:verified]` ISO 19650-2 phân chia quá trình thành 8 sub-processes.
**Rule quan trọng:** Bước 5.1 và 5.8 diễn ra **một lần** cho mỗi dự án (Project level). Bước 5.2 đến 5.7 **lặp lại** cho mỗi lần bổ nhiệm/hợp đồng (Appointment level).

1. **5.1 Assessment and Need:** Appointing party thiết lập project-level framework (PIR, information standard, CDE, protocol).
2. **5.2 Invitation to Tender:** Appointing party phát hành EIR và tài nguyên tham chiếu để đấu thầu.
3. **5.3 Tender Response:** Prospective lead appointed party nộp pre-appointment BEP, đánh giá năng lực, mobilization plan, risk register.
4. **5.4 Appointment:** Lead appointed party xác nhận BEP (thành post-appointment BEP), lập MIDP, TIDPs, và phân bổ detailed responsibility matrix. Cascade EIR xuống task teams.
5. **5.5 Mobilization:** Các team huy động nguồn lực, IT, và test thử quy trình sản xuất (test CDE workflow).
6. **5.6 Collaborative Production:** Sản xuất, QA nội bộ, và model review chéo giữa các teams (WIP → Shared).
7. **5.7 Information Model Delivery:** Two-step authorization: Lead Appointed Party ủy quyền nội bộ, sau đó Appointing Party chấp thuận (Shared → Published).
8. **5.8 Project Close-out:** Lưu trữ PIM (chuyển sang AIM) và đúc kết bài học.

### Các tài liệu quản lý cốt lõi (5.1)

Bước 5.1 định nghĩa các tài nguyên nền tảng mà Appointing Party phải chuẩn bị:
- **Project's information standard (5.1.4):** Quy định naming conventions, metadata, classification, và LOIN specification.
- **Production methods and procedures (5.1.5):** Quy trình tạo, duyệt, bảo mật và giao nộp thông tin.
- **Information protocol (5.1.8):** Các điều khoản pháp lý về nghĩa vụ, IP, v.v.
- **CDE (5.1.7):** Thiết lập môi trường dữ liệu chung đáp ứng requirements của Clause 12 (Part 1).

### EIR Cascade (5.4.3)

`[ISO-CORE:verified]` Appointing party ban hành EIR ban đầu. Sau đó, **Lead Appointed Party sẽ thiết lập EIR của riêng mình** cho từng appointed party tiếp theo (nhà thầu phụ/tư vấn phụ), tạo thành hiệu ứng thác nước (cascade) xuyên suốt chuỗi cung ứng.

### CDE State Mapping trong quá trình sản xuất (5.6 - 5.7)

Quy trình quản lý WIP → Shared → Published được map cụ thể vào Part 2:
- **WIP:** Tương ứng bước *5.6.2 (Generate)* và *5.6.3 (QA check)*.
- **WIP → Shared:** Tương ứng *5.6.4 (Approve for sharing)* do Task information manager thực hiện.
- **Shared:** *5.6.5 (Model review - cross team coordination)* và *5.7.1-5.7.2 (Lead Appointed Party review)*.
- **Shared → Published:** *5.7.4 (Appointing party acceptance)* — thông tin chính thức được chấp thuận.
- **Published → Archive:** *5.8.1 (Archive PIM)* khi Project close-out.

### Two-Step Authorization (Cấp quyền 2 bước - 5.7)

ISO 19650-2 có thiết kế ủy quyền nổi bật cho Information Model:
1. **Supply chain gate (Internal):** Task teams nộp cho Lead appointed party. Nếu Lead duyệt, mô hình mới được chuyển sang cấp 2. (Không làm thay đổi CDE state sang Published).
2. **Client gate (External):** Lead appointed party nộp cho Appointing party. Nếu Client accept, các containers chính thức chuyển sang trạng thái **Published** trong CDE.

### Phân công trách nhiệm (Annex A)

`[ISO-CORE:verified]` Ma trận phân quyền (RACI) của 8 bước cho 4 nhóm: Appointing party, Lead appointed party, Appointed party, Task team. Appointing party hoạt động cao nhất ở mốc đầu (5.1, 5.2) và cuối (5.8), còn nhóm Appointed/Task teams sẽ gánh phần lớn việc sản xuất (5.6, 5.7).

## Quan hệ

- **Parent:** [[iso-19650]]
- **Updated concepts:** [[bep]], [[eir]], [[cde]], [[midp-tidp]], [[bim-delivery-roles]], [[pim]]

## Nguồn

- [[raw/core/ISO_19650-2]] — Toàn bộ document đã được `[ISO-CORE:verified]` với bản raw ISO text.
