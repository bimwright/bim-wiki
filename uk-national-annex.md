---
title: "UK National Annex (Phụ lục Quốc gia Anh)"
aliases: ["UK National Annex", "UK NA", "BS EN ISO 19650 NA"]
tags: ["#bim", "#iso-19650", "#uk", "#annex", "#standard"]
type: concept
source: "[[raw/national-annexes/UK_NA]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# UK National Annex (Phụ lục Quốc gia Anh)

> **TL;DR:** Phụ lục Quốc gia của Vương quốc Anh quy định các mã trạng thái CDE (S0-S7, A1-An), hệ thống phân loại tiêu chuẩn (Uniclass 2015) và các quy tắc đặc thù để triển khai ISO 19650. Đây là bản phụ lục có mức độ trưởng thành cao nhất và là hình mẫu tham chiếu cho quá trình quốc tế hóa BIM.

## Khái niệm cốt lõi

- **Mục đích:** ISO 19650 cung cấp khung quy trình chung, trong khi National Annex (NA) cung cấp các quy chuẩn kỹ thuật cụ thể (mã trạng thái, classification, đặt tên file) phù hợp với hạ tầng pháp lý và kỹ thuật của từng quốc gia.
- **Tiêu chuẩn đi kèm:** BS EN ISO 19650-2 National Annex là tài liệu trọng tâm nhất, định nghĩa chi tiết workflow trao đổi thông tin.
- **Uniclass 2015:** Hệ thống phân loại được UK NA chỉ định sử dụng để gắn nhãn các đối tượng và tài liệu trong mô hình.

## Mã trạng thái CDE (Status Codes)

Tại Anh, mã trạng thái đóng vai trò then chốt trong quy trình luân chuyển thông tin trên CDE:

### Trạng thái WIP (Work In Progress)
- **S0:** Bản phác thảo khởi tạo -- không chia sẻ ngoài nhóm tác giả.

### Trạng thái Shared (Chia sẻ - Chưa có giá trị hợp đồng)
- **S1:** Phù hợp để phối hợp (chỉ tham chiếu).
- **S2:** Phù hợp để cung cấp thông tin (mid-stage reviews).
- **S3:** Phù hợp để phê duyệt nội bộ (review and comment).
- **S4:** Phù hợp để phê duyệt giai đoạn bởi lãnh đạo dự án.
- **S5:** Phê duyệt cuối cùng bởi CĐT trước khi chuyển sang Published.
- **S6-S7:** Phù hợp để ủy quyền PIM/AIM.

### Trạng thái Published (Phát hành - Có giá trị hợp đồng)
- **A1, A2, An:** Đã được ủy quyền và chấp thuận (contractual).
- **B1, B2, Bn:** Chấp thuận có lưu ý (không khuyến nghị sử dụng tiếp nếu chưa sửa).
- **CR:** Hồ sơ hoàn công chính thức.

## Bối cảnh Đặc thù UK

- **Golden Thread:** Phối hợp với Đạo luật An toàn Tòa nhà 2022 để duy trì "luồng thông tin vàng" minh bạch xuyên suốt vòng đời tòa nhà cao tầng.
- **CDE Technical Solutions:** Được hướng dẫn sâu hơn tại Part C của **UK BIM Framework**.

## Việc áp dụng trên thế giới (CEN & Quốc tế)

| Quốc gia/Khu vực | Đặc điểm triển khai |
|------------------|---------------------|
| **Ireland** | Đã ban hành Irish NA (IS EN ISO 19650-2). |
| **Australia** | Áp dụng qua ủy ban BD-104; tiêu chuẩn AS ISO 19650. |
| **New Zealand** | Áp dụng qua NZ BIM Handbook. |
| **Germany / Italy** | Áp dụng qua chuẩn CEN (DIN/UNI EN ISO 19650). |
| **Singapore** | Tích hợp vào khung BIM quốc gia của BCA. |
| **Peru** | Nằm trong chiến lược Plan BIM Peru. |

*Lưu ý: Các quốc gia thành viên CEN bắt buộc phải áp dụng chuẩn EN ISO 19650 và thường tự xây dựng National Annex riêng.*

## Quan hệ

- **Supplement to:** [[iso-19650]]
- **Parent of:** [[summary_uk-bim-framework]]
- **Related:** [[cde]] — cung cấp bảng mã trạng thái thực tế.

## Nguồn

- [[raw/national-annexes/UK_NA]] — Tài liệu gốc quy định các mã trạng thái và phân loại chuẩn của Anh.
