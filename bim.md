---
title: "BIM — Building Information Modelling"
aliases: ["Building Information Modelling", "Building Information Modeling", "BIM", "Mô hình thông tin công trình"]
tags: ["#bim", "#concept", "#iso-19650"]
type: concept
source: "[[raw/core/ISO_19650_Overview]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# BIM — Building Information Modelling

> **TL;DR:** BIM là cách tiếp cận quản lý thông tin trong toàn vòng đời tài sản xây dựng dựa trên mô hình số phối hợp; ISO 19650 là tiêu chuẩn quốc tế quy định cách triển khai BIM.

## Khái niệm cốt lõi

- **Định nghĩa ISO:** "Use of a shared digital representation of a built asset to facilitate design, construction and operation processes to form a reliable basis for decisions" (ISO 19650-1, clause 3.3.14)
- **Bản chất:** Không chỉ là phần mềm — là *quy trình, thông lệ, và giao thức* để tạo, quản lý, và chia sẻ thông tin số về tài sản xây dựng
- **Hai sản phẩm thông tin cốt lõi:** [[pim]] (Project Information Model) trong giai đoạn thiết kế/thi công → handover thành [[aim]] (Asset Information Model) khi vận hành
- **Tiêu chuẩn điều chỉnh:** [[iso-19650]] là framework quốc tế; các tiêu chuẩn quốc gia tham chiếu trong `raw/national-standards/` — chưa ingest
- **Điều kiện triển khai:** Cần [[cde]] (Common Data Environment) làm hạ tầng chia sẻ; cần [[eir]] (Exchange Information Requirements) để định nghĩa thông tin cần trao đổi; cần các vai trò rõ ràng (xem [[bim-delivery-roles]])

## Chi tiết / Triển khai

- **Việt Nam:** Các tiêu chuẩn quốc gia trong `raw/national-standards/VN/` (QĐ 347, QĐ 348) — nội dung chi tiết chưa ingest; không thể phát biểu claim cụ thể từ source hiện tại
- **Cấp độ thông tin:** Khái niệm "Level of Detail/Development" (LOD) trong thực hành; ISO 19650 dùng [[loin]] (Level of Information Need) thay LOD
- **Predecessor:** PAS 1192 (UK) — tiền thân của ISO 19650, xem [[pas-1192-mapping]]

## Quan hệ

- **Parent:** [[iso-19650]] — tiêu chuẩn quy định BIM framework
- **Children:** [[pim]], [[aim]], [[cde]], [[loin]], [[bep]]
- **Related:** [[bim-delivery-roles]] — các vai trò trong dự án BIM

## Nguồn

- [[raw/core/ISO_19650_Overview]] — [[summary_iso-19650-overview]]
