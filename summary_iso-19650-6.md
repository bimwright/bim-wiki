---
title: "ISO 19650-6 — Health and Safety Information"
aliases: ["ISO 19650 Part 6 summary", "ISO 19650-6:2025 tóm tắt"]
tags: ["#bim", "#iso-19650", "#iso-19650-6", "#standard", "#summary", "#health-and-safety"]
type: summary
source: "[[raw/core/ISO_19650-6]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# ISO 19650-6 — Health and Safety Information

> **TL;DR:** Part 6 (2025) là lớp phủ thông tin An toàn và Sức khỏe (H&S Overlay) trên vòng đời tài sản. Trái với Part 5 (thiên về quy trình), Part 6 áp dụng hệ thống quản trị rủi ro bằng cơ sở dữ liệu **hướng Schema** (Schema-driven), tích hợp chặt chẽ việc ghi nhận Risk, Incident vào mô hình BIM (IFC).

## Nội dung tóm tắt

### Bản chất của H&S Overlay

`[ISO-CORE:verified]` Trong khi các Part khác giao khoán deliverable cho Appointed Parties, quản lý An toàn Sức khỏe (Health and safety) được quy định rõ là **Trách nhiệm tập thể (Collective responsibility)**. 
- Nó có thể áp dụng cho dự án dùng BIM hoặc truyền thống.
- Kéo dài trọn bộ vòng đời tài sản (kể cả bước end-of-life / phá dỡ).

### Cấu trúc cơ sở dữ liệu (Clause 4)

Trái tim của tiêu chuẩn là **[[hs-schema]]** chia thông tin định dạng H&S thành các cấu trúc để dễ quản lý và giao tiếp xuyên suốt quá trình thiết kế - thi công - vận hành. Mục đích là để học hỏi từ các incident chèn lại vào yếu tố thiết kế.

### Vòng đời sử dụng thông tin (Clause 4.5)

Toàn bộ luồng hoạt động thông tin H&S đi qua 5 giai đoạn:
1. **Generate:** Tạo.
2. **Share:** Chia sẻ.
3. **Present:** Trình bày/Cảnh báo trực quan.
4. **Use:** Đưa vào quyết định.
5. **Generalize:** Khái quát hóa — trừu tượng/tổng hợp hóa thông tin an toàn thu thập được để chia sẻ kinh nghiệm tránh rủi ro cho các dự án sau (điểm độc đáo của Part 6).

### Sự giao thoa (Clause 5 & 6)

`[ISO-CORE:structure]` Part 6 tích hợp trực tiếp vào 8 bước của Part 2 và Part 3, bổ sung tiêu chí H&S vào OIR/AIR/PIR/EIR. Đặc biệt, **Annex D** cung cấp chỉ dẫn chuẩn xác để mapping các dữ liệu H&S này vào định dạng IFC — chuẩn openBIM quốc tế.

## Quan hệ

- **Parent:** [[iso-19650]]
- **Overlays on:** [[summary_iso-19650-2]], [[summary_iso-19650-3]]
- **New concepts:** [[hs-schema]]

## Nguồn

- [[raw/core/ISO_19650-6]] — Tổng quan Scope, schema và nguyên lý.
