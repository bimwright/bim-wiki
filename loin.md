---
title: "LOIN — Level of Information Need"
aliases: ["Level of Information Need", "LOIN", "Level of Detail", "LOD", "Level of Development"]
tags: ["#bim", "#iso-19650", "#concept", "#loin"]
type: concept
source: "[[raw/core/ISO_19650_Overview]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# LOIN — Level of Information Need

> **TL;DR:** LOIN (ISO 19650-1) thay thế khái niệm "Level of Detail/Development" (LOD) trong thực hành BIM, định nghĩa chính xác mức độ thông tin cần thiết cho từng mục đích sử dụng cụ thể.

## Khái niệm cốt lõi

- **Định nghĩa:** Mức độ thông tin cần thiết để phục vụ một mục đích cụ thể (ISO 19650-1, clause 3.3.16); được xác định bởi Appointing Party trong [[eir]]
- **Khác với LOD:** LOD (Level of Detail/Development) là khái niệm thực hành phổ biến (AIA, BIMForum) nhưng không phải thuật ngữ ISO. LOIN là chuẩn hóa quốc tế — dùng "need" (nhu cầu) thay "detail" (chi tiết) để nhấn mạnh mục đích sử dụng thúc đẩy yêu cầu thông tin
- **Ba loại thông tin trong LOIN (EN 17412-1):**
  - **Geometrical information:** Hình dạng, vị trí, kích thước, góc nghiêng (theo 5 cấp độ)
  - **Alphanumerical information:** Thuộc tính, tham số, phân loại, tài liệu
  - **Documentation:** Văn bản, bản vẽ 2D, bảng biểu
- **Thời điểm xác định:** Được specify trong [[eir]] trước khi tender — delivery team phải đáp ứng LOIN này trong [[bep]]

## Chi tiết / Triển khai

- **Cách dùng thực tế:** Appointing Party điền LOIN vào EIR theo từng information container (Revit model, clash report, COBie data...) cho từng giai đoạn delivery
- **Standard method:** EN 17412-1:2020 cung cấp methodology chi tiết cho LOIN — được referenced trong ISO 19650-1 nhưng là out-of-scope cho ingest này; promote khi Part 1 được ingest

## Quan hệ

- **Parent:** [[bim]]
- **Defined in:** [[eir]] — Exchange Information Requirements chứa LOIN cho từng exchange
- **Related:** [[information-requirements-hierarchy]] — LOIN là output của EIR, được khai báo trong PIR/AIR
- **Contradicts:** [[lod-vn]] — Hệ tiêu chuẩn Việt Nam QĐ 347 vẫn sử dụng triết lý LOD 100-500 của Mỹ thay vì chuyển đổi sang khái niệm LOIN của ISO.

## Nguồn

- [[raw/core/ISO_19650_Overview]] — [[summary_iso-19650-overview]]
- [[raw/core/ISO_19650-1]] — Clause 11.2 `[ISO-CORE:verified/structure]` — xác nhận definition (3.3.16 verified); 4 components: Purpose (WHY) · Content (WHAT: geometrical + alphanumerical + documentation) · Form (HOW presented) · Format (technical format for exchange); LOIN identified per [[information-container]] và recorded trong TIDPs — [[summary_iso-19650-1]]
- [[raw/national-standards/VN/QD_347_BXD]] — `[VN-BXD:verified]` — Quyết định số 347/QĐ-BXD của Việt Nam chưa dùng chuẩn LOIN, vẫn giữ vững bảng mapping the LOD (Level of Development) 100-500 của BIMForum. — [[lod-vn]]
