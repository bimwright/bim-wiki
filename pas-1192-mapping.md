---
title: "Mapping PAS 1192 sang ISO 19650"
aliases: ["PAS 1192 Mapping", "BIM Level 2 Mapping"]
tags: ["#bim", "#legacy", "#standard", "#comparison"]
type: comparison
source: "[[raw/legacy/PAS_1192_Mapping]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# Mapping từ PAS 1192 sang ISO 19650

> **TL;DR:** Tài liệu đối chiếu sự chuyển đổi từ bộ tiêu chuẩn PAS 1192 của Vương quốc Anh sang tiêu chuẩn quốc tế ISO 19650. Đây là nguồn tham khảo lịch sử để hiểu rõ sự thay đổi thuật ngữ và triết lý quản lý thông tin.

## Khái niệm cốt lõi

- **Lịch sử:** Bộ BS/PAS 1192 là nền tảng của chiến lược BIM tại Anh (BIM Level 2). Khi đưa lên quy mô quốc tế, ISO đã trích xuất các quy trình lõi này để tạo thành series ISO 19650.
- **Tính kế thừa:** Tài liệu chuyển đổi **PD 19650-0:2019** đã được BSI phát hành nhằm cung cấp hướng dẫn chi tiết cho quá trình chuyển giao này.
- **Sự khác biệt chính:** Chuyển từ các khái niệm đặc thù của Anh (UK-centric) sang ngôn ngữ trung lập, linh hoạt hơn cho thị trường toàn cầu.

## Bảng đối chiếu tiêu chuẩn

| Tiêu chuẩn cũ (UK PAS) | Tiêu chuẩn thay thế (ISO) | Trạng thái |
|-------------------------|--------------------------|------------|
| BS 1192:2007+A2:2016    | ISO 19650-1:2018         | Đã bị thu hồi |
| PAS 1192-2:2013         | ISO 19650-2:2018         | Đã bị thu hồi |
| PAS 1192-3:2014         | ISO 19650-3:2020         | Đã bị thu hồi |
| PAS 1192-5:2015         | ISO 19650-5:2020         | Đã bị thu hồi |
| PAS 1192-6:2018         | ISO 19650-6:2025         | Đã bị thu hồi |

## Thay đổi thuật ngữ (Terminology Changes)

| PAS 1192 (Cũ) | ISO 19650 (Mới) | Ghi chú |
|---------------|-----------------|---------|
| Employer / Client | **Appointing party** | Rộng hơn, dành cho mọi đối tượng giao việc |
| Supplier | **Appointed party** | Bên được giao việc |
| Tier 1 Supplier | **Lead appointed party** | Bên được ủy quyền chính |
| Pre-contract BEP | **Pre-appointment BEP** | "Contract" → "Appointment" |
| Post-contract BEP | **Post-appointment BEP** | |
| LOD / LOI | **Level of information need** | Hợp nhất thành khung LOIN linh hoạt |
| Graphical / Non-graphical | **Geometrical / Alphanumerical** | Hình học / Phi hình học |
| Data Drop | **Information exchange** | Trao đổi thông tin |
| File / Document | **Information container** | Đơn vị lưu trữ thông tin (technology-neutral) |
| Volume Strategy | **Federation strategy** | Chiến lược phối hợp mô hình |
| Capital/Delivery Phase | **Delivery phase** | Giai đoạn thực hiện |
| BIM Level 2 | **"BIM according to ISO 19650"** | Bỏ hệ thống phân cấp maturity levels cũ |
| Pathways | **Trigger events** | Các sự kiện kích hoạt (trong Part 3) |
| The "Racetrack" | **CDE workflow** | Sơ đồ luân chuyển trạng thái dữ liệu |

## Các điểm khác biệt cốt lõi

1. **Quốc tế hóa:** Loại bỏ hoàn toàn các tham chiếu đặc thù của chính phủ Anh và chiến lược xây dựng nội địa.
2. **National Annex:** Các quy ước kỹ thuật riêng như Uniclass hay quy tắc đặt tên được đưa vào Phụ lục Quốc gia thay vì nằm trong lõi tiêu chuẩn.
3. **LOIN (Level of information need):** Thay thế LOD/LOI cứng nhắc bằng hệ thống 4 thành phần: Mục đích · Nội dung · Hình thức · Định dạng.
4. **Phạm vi mở rộng:** Áp dụng cho mọi loại tài sản hạ tầng và công trình dân dụng, không chỉ giới hạn ở tòa nhà.
5. **Hài hòa hóa thuật ngữ:** Đảm bảo tính nhất quán xuyên suốt tất cả các phần của bộ tiêu chuẩn.

## Quan hệ

- **Successor:** [[iso-19650]]
- **Relates to:** [[summary_uk-bim-framework]], [[uk-national-annex]]

## Nguồn

- [[raw/legacy/PAS_1192_Mapping]] — Tài liệu gốc ghi nhận mối quan hệ giữa các tiêu chuẩn predecessor.
