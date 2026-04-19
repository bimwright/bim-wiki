---
title: "Sensitivity Assessment"
aliases: ["Sensitivity Assessment", "Đánh giá mức độ nhạy cảm", "Security triage"]
tags: ["#bim", "#iso-19650", "#iso-19650-5", "#concept", "#security"]
type: concept
source: "[[raw/core/ISO_19650-5]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# Sensitivity Assessment (Đánh giá mức độ nhạy cảm)

> **TL;DR:** Là bước đầu tiên và quan trọng nhất của quy trình chuẩn ISO 19650-5. Bước Triage (phân loại) này giúp định đoạt xem dự án, hoặc thông tin thuộc tài sản đó CÓ CẦN hay KHÔNG CẦN áp dụng tiêu chuẩn bảo mật (Security-minded approach).

## Khái niệm cốt lõi

- **Mục tiêu:** Nhận diện 6 nguồn nguy cơ: Rủi ro kinh tế, uy tín, chính trị, thương mại, bảo mật dữ liệu cá nhân (GDPR), và cơ sở hạ tầng trọng yếu (Critical infrastructure).
- **Security Triage (Phân loại bảo mật):** Cổng ra quyết định (Decision gate, nằm tại Sub-clauses 4.7–4.10) được xem xét dựa trên các nguy cơ tìm thấy.
  - Nhánh **NO** (Không cần Security Approach): Được quyền miễn trừ 100% các Phase còn lại của ISO 19650-5. Chỉ cần lập Audit Log và cài đặt hẹn lịch review lại trong tương lai để đề phòng thông tin đổi bản chất.
  - Nhánh **YES** (Cần Security Approach): Buộc phải thực hiện Clause 5 đến 9 (Khởi động Governance, xây Strategy, lập Plan).
- **Đối tượng áp dụng:** Bất kỳ tổ chức nào nắm quyền sở hữu tài sản hoặc bắt đầu chuẩn bị một dự án xây dựng/Vận hành (Appointing Party/Client).

## Chi tiết / Triển khai

- **Reviews theo chu kỳ định kỳ (Clause 4.6):** Ngay cả khi ra quyết định NO ở bước Security Triage, bước đánh giá này vẫn bắt buộc phải Review lại khi có các thay đổi trigger (Ví dụ: môi trường ngoại cảnh thay đổi, pháp luật đổi, hoặc tài sản đổi công năng dẫn đến risk về nhạy cảm cao hơn).
- **Tính Tương xứng (Proportionality):** Một đánh giá Sensitivity Assessment tốt sẽ không yêu cầu siết chặt mức độ bảo mật cao nhất một cách phi thực tế cho tất cả thông tin, mà nó chia tách độ nhạy cảm của từng gói Info / Asset nhằm nới lỏng cho SME tham gia thầu thoải mái.

## Quan hệ

- **Parent:** [[iso-19650]] (Cụ thể là Part 5)
- **Gatekeeper cho:** Việc kích hoạt Security Strategy và Security Management Plan.
- **Relates to:** [[eir]] — Kết quả quyết định Cần bảo mật sẽ làm thay đổi và chèn thêm yêu cầu về bảo mật sâu vào bên trong tài liệu EIR.

## Nguồn

- [[raw/core/ISO_19650-5]] — Nền tảng cốt lõi của Clause 4 `[ISO-CORE:structure]`.
