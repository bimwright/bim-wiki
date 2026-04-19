---
title: "ISO 19650-3 — Operational Phase of the Assets"
aliases: ["ISO 19650 Part 3 summary", "ISO 19650-3:2020 tóm tắt"]
tags: ["#bim", "#iso-19650", "#iso-19650-3", "#standard", "#summary"]
type: summary
source: "[[raw/core/ISO_19650-3]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# ISO 19650-3 — Operational Phase of the Assets

> **TL;DR:** Part 3 điều chỉnh quy trình 8 bước của Part 2 để áp dụng cho giai đoạn vận hành tài sản, sử dụng mô hình vòng lặp vô tận kích hoạt bởi các [[trigger-event]]. Nó yêu cầu AIM phải kết nối trực tiếp với các hệ thống quản trị doanh nghiệp (CAFM, CMMS).

## Nội dung tóm tắt

### Tổng quan quy trình vòng lặp (Clause 4)

Khác với Part 2 (tuyến tính, dự án có bắt đầu và kết thúc), quy trình Part 3 là **vòng lặp vô hạn**:
1. **Bước thiết lập (5.1):** Hoạt động như một "standing organizational framework" (khung tổ chức thường trực). Thiết lập một lần và duy trì liên tục trong suốt vòng đời tài sản.
2. **Vòng lặp sự kiện (5.2 - 5.7):** Diễn ra mỗi khi có một [[trigger-event]] xảy ra.
3. **Tiếp nhận vào hệ thống (5.8):** Aggregation — dữ liệu mới được hợp nhất (aggregate) vào AIM, và chu trình chờ trigger event tiếp theo.

### Framework bảo trì và vận hành (Clause 5.1)

Bước *5.1 Assessment and Need* của Part 3 mở rộng từ 9 sub-clauses (Part 2) lên **14 sub-clauses**, tập trung mạnh vào vòng đời dài hạn và tổ chức:
- Nhấn mạnh vào **OIR (Organizational Information Requirements)** và **AIR (Asset Information Requirements)** thay cho PIR tĩnh. 
- Yêu cầu cấu trúc **AIM (Asset Information Model)** phải đóng vai trò vừa là đầu vào tham chiếu, vừa là đích đến liên tục cập nhật.
- `[ISO-CORE:verified]` **Clause 5.1.10:** Bắt buộc xây dựng cầu nối (links) giữa AIM/CDE với các hệ thống quản lý chuẩn của Doanh nghiệp (Enterprise systems như CAFM, CMMS, ERP, IoT nền tảng) — CDE không được đứng độc lập.

### Authorization và Acceptance (Clause 5.6 & 5.7)

Trong quá trình collaborative production:
- LAP Authorization (Lead Appointed Party Authorization) được chuyển từ giai đoạn Delivery/Acceptance (Part 2) lùi vào hẳn bước *5.6 (Production of Information)*.
- Khúc *5.7 (Information model acceptance by appointing party)* chỉ thuần túy là việc Review và Accept từ phía Chủ đầu tư (Appointing party).

### AIM Aggregation (Clause 5.8)

Trái ngược với bước Terminal "Project close-out" của Part 2, quy trình Part 3 *5.8* là **AIM Aggregation**. Dữ liệu được đưa vào AIM cũ mà không chèn đè hoàn toàn:
- Dung hợp dữ liệu mới từ Appointed parties.
- Chuyển thông tin lỗi thời thành trạng thái Archived (thay vì xóa bỏ).
- Kích hoạt việc Maintain resources & ready trạng thái cho đợt huy động (trigger event) tiếp theo.

## Quan hệ

- **Parent:** [[iso-19650]]
- **Updated concepts:** [[aim]], [[information-requirements-hierarchy]], [[cde]], [[eir]], [[pim]]
- **New concepts:** [[trigger-event]]

## Nguồn

- [[raw/core/ISO_19650-3]] — Tổng hợp các clause khác biệt so với Part 2, verified against raw ISO source `[ISO-CORE:verified]` và cấu trúc của UK BIM Framework `[ISO-CORE:structure]`.
