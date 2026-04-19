---
title: "Trigger Event (Sự kiện kích hoạt)"
aliases: ["Trigger Event", "Trigger Events", "Sự kiện kích hoạt"]
tags: ["#bim", "#iso-19650", "#iso-19650-3", "#concept"]
type: concept
source: "[[raw/core/ISO_19650-3]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# Trigger Event

> **TL;DR:** Sự kiện kích hoạt (Trigger Event) là các sự kiện trong quá trình vận hành, bảo trì tài sản khởi chạy vòng lặp cập nhật thông tin cho AIM (theo ISO 19650-3).

## Khái niệm cốt lõi

- **Định nghĩa:** Một sự kiện lên lịch trước hoặc bất khả kháng tạo ra nhu cầu cập nhật/tạo mới thông tin tài sản lưu trữ trong [[aim]]. (ISO 19650-1, clause 3.2.14)
- **Cơ chế:** Kích hoạt quá trình Procurement và Delivery (bước 5.2 đến 5.7 trong ISO 19650-3). Khi quy trình quy định thông tin hoàn tất, thông tin sẽ được aggregate về chức năng duy trì của AIM ở bước 5.8.
- **Phân loại 3 nhóm chính (Part 3):**
  1. **Type 1 (Scheduled/Foreseeable - Theo kế hoạch):** Bảo trì định kỳ. Cho phép dùng framework agreement để bypass thủ tục mời thầu → Đi thẳng vào tạo lập (5.5, 5.6).
  2. **Type 2 (Unscheduled - Ngoại lệ/Bất khả kháng):** Tai nạn, lũ lụt, hỏng hóc khẩn trương. Đòi hỏi chạy full vòng quy trình (5.2 – 5.8). Có thể gọi vốn lập dự án lớn (kích hoạt chạy Part 2 PIM delivery).
  3. **Type 3 (Asset Acquisition - Sáp nhập):** Tiếp nhận thông tin khi mua lại tài sản. Khởi chạy 5.7 (Verify & Acceptance) và 5.8 (Aggregation) ngay lập tức.

## Chi tiết / Triển khai

- **Duy trì mức độ sẵn sàng:** Chức năng 5.5.4 đòi hỏi Lead appointed party phải duy trì nguồn lực resources sẵn sàng để ứng phó với trigger events tiếp theo, do sự cách biệt về thời gian chờ giữa các kỳ bảo trì.
- **Identify foreseeable trigger events:** Clause 5.1.5 bắt buộc Tổ chức Appointing party phải vạch sẵn ra các sự kiến loại 1 trong Framework tĩnh để lập EIR template, ngân sách sớm.

## Quan hệ

- **Parent:** [[iso-19650]]
- **Triggers:** Quá trình Information Delivery của [[aim]]
- **Relates to:** [[information-requirements-hierarchy]] (AIR đáp ứng cho Trigger events)

## Nguồn

- [[raw/core/ISO_19650-3]] — Mô tả cơ chế Type 1, 2, 3 và luồng framework đi qua 8 giai đoạn trong giai đoạn Operational phase `[ISO-CORE:structure]`.
