---
title: "H&S Schema (ISO 19650-6)"
aliases: ["H&S Schema", "Health and Safety Schema"]
tags: ["#bim", "#iso-19650", "#iso-19650-6", "#concept", "#schema", "#health-and-safety"]
type: concept
source: "[[raw/core/ISO_19650-6]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# H&S Schema

> **TL;DR:** Là bộ khung dữ liệu mẫu (schema) được ISO 19650-6 thiết kế riêng cho việc quản trị rủi ro An toàn và sức khỏe (H&S). Nó cho phép liên kết trực giác giữa đối tượng, rủi ro, sự cố và biện pháp xử lý.

## Khái niệm cốt lõi

- **Định nghĩa:** Bộ kiến trúc phân mảnh dữ liệu thuộc Clause 4.3 của tiêu chuẩn ISO 19650-6.
- **Thành phần:** Tổ chức thành 4 phân hệ (sub-schemas) giao tiếp chéo bằng hệ thống mã nhận dạng (Identifiers):
  1. **Context sub-schema:** Bối cảnh (Vị trí, đặc điểm vật lý, tính chất công việc hoặc môi trường liên đới sinh ra risk).
  2. **Risk sub-schema:** Hồ sơ rủi ro H&S độc lập.
  3. **Incident sub-schema:** Hồ sơ sự cố — Ghi nhận biến cố thực tế đã xảy ra (Sự cố có hại, tai nạn). Liên kết ngược lại Context để người thiết kế rút kinh nghiệm.
  4. **Risk & Incident Treatment sub-schema:** Phương án xử lý và kiểm soát (Ưu tiên các kết quả an toàn từ trong trứng nước - inherently safer outcomes).

## Chi tiết / Triển khai

- **Tích hợp phần mềm:** Do thiết kế dạng database schema, hệ thống này hoàn toàn có thể lập trình tích hợp vào phần mềm authoring, hoặc CDE.
- **IFC Representation:** Sự đặc biệt của Part 6 nằm ở **Annex D**, cung cấp luồng mapping chi tiết bộ Schema này vào chuẩn IFC (Industry Foundation Classes) của buildingSMART, giúp gán cứng rủi ro vào các object 3D cụ thể (dầm, cột, phòng) thay vì chỉ nằm trong tài liệu text độc lập.

## Quan hệ

- **Parent:** [[iso-19650]] (Part 6)
- **Implemented via:** Các file/model định dạng hệ thống mở (vd: IFC, xem [[exchange-criteria]] ở Part 4).

## Nguồn

- [[raw/core/ISO_19650-6]] — Clause 4.3 & Annex D `[ISO-CORE:structure]`.
