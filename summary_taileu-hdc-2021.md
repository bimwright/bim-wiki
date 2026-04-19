---
title: "Tài liệu Hướng dẫn chung áp dụng BIM (Bộ XD 2021)"
aliases: ["Tai lieu HDC 2021", "Hướng dẫn chung BIM 2021", "HDC QĐ 348 body"]
tags: ["#bim", "#qd348", "#vietnam", "#guidance", "#summary"]
type: summary
source: "[[raw/national-standards/VN/TaiLieu_HDC_2021]]"
status: draft
created: 2026-04-19
updated: 2026-04-19
---

# Tài liệu Hướng dẫn chung áp dụng BIM (Bộ XD 2021)

> **TL;DR:** Tài liệu do Viện KTXD biên soạn, Bộ XD công bố 04/2021, là hướng dẫn body đính kèm [[summary_qd-348]]. PDF 64+ trang chi tiết 3 phần + 4 phụ lục, bảng mã CDE S0-S4/A1/B1, naming ISO 19650-2, 9 use case BIM, LOD per component.

## Nội dung tóm tắt

### 1. Quan hệ với QĐ 348

`[VN-BXD:verified]` (Mở đầu, trang 1) "Hướng dẫn này thay thế Hướng dẫn tạm thời áp dụng BIM được công bố kèm theo QĐ 1057/QĐ-BXD ngày 11/10/2017" — là hướng dẫn body mà QĐ 348 (02/04/2021) ra quyết định công bố. Cùng nội dung với [[summary_qd-348]] nhưng PDF 6.5 MB với cấu trúc + ví dụ chi tiết hơn.

### 2. Thuật ngữ chuẩn (Bảng 1 — 18 thuật ngữ)

`[VN-BXD:verified]` Định nghĩa VN-EN-Abbr cho: BEP, Pre-BEP, EIR, CDE, LOD, MIDP, TIDP, IFC, BIM Model, BIM Manager, BIM Coordinator, BIM Modeler, Task Team, Project Team, Employer, etc. Đây là **từ điển BIM chính thức** của Bộ Xây dựng.

### 3. Tiến trình 6 bước (Hình 1.1)

Xác định nội dung → Lựa chọn đơn vị thực hiện → Chuẩn bị cho nhóm dự án → Xây dựng mô hình → Kiểm tra/phê duyệt → Lưu trữ + đánh giá.

### 4. Trách nhiệm Chủ đầu tư vs Đơn vị thực hiện (Bảng 1.1-1.2)

Ma trận RACI cho 8 nhiệm vụ: mức độ tham gia Cao/Trung bình/Thấp. CĐT chủ trì đánh giá năng lực + kiểm tra nghiệm thu + lưu trữ. Đơn vị thực hiện chủ trì dự thầu + tạo lập mô hình.

### 5. CDE (Phần 3.2) — citation UK BIM Framework

`[VN-BXD:verified]` 3 loại CDE (Dự án/Chủ đầu tư/Đơn vị); 4 vùng (WIP/SHARED/PUBLISHED/ARCHIVED); mã phiên bản `P01.01` / `C01.01`; **Bảng 3.1 mã trạng thái** S0-S4, A1, B1 với matrix áp dụng cho dữ liệu hình học / phi hình học / tài liệu. Danh sách 16 giải pháp CDE thương mại.

### 6. Naming convention (Phần 3.4.4) — theo ISO 19650-2:2018

Format 7 trường bắt buộc: `Dự án-Đơn vị-Khối tích-Cao trình-Loại-Vai trò-SốTT` (+ 3 tùy chọn). Mã chuẩn per field (AR/ST/ME... cho Khối tích; A/S/C... cho Vai trò; M2/M3/DR/BQ... cho Loại).

### 7. Yêu cầu kỹ thuật (Phần 3.4)

- Định dạng: gốc + mở (**IFC bắt buộc** cho chuyển giao)
- Tỷ lệ 1:1, SI, **mm cho dân dụng** / **m cho hạ tầng**
- **Hệ tọa độ quốc gia VN-2000** là chuẩn
- Phân loại bộ phận: **OmniClass** khi không có hướng dẫn khác
- **LOD áp dụng cho từng thành phần mô hình cụ thể, không cho toàn mô hình** — xem [[lod-vn]]

### 8. Use case BIM (Phụ lục 01 — 9 mục)

Xây dựng mô hình hiện trạng · Tạo lập BIM 3D · Phân tích năng lượng · Phân tích kết cấu · Phân tích ánh sáng · Đánh giá thiết kế · Dự toán chi phí (5D) · Phối hợp 3D · Lập tiến độ (4D).

## Quan hệ

- **Body of:** [[summary_qd-348]] (QĐ 348 = quyết định công bố).
- **Replaces:** [[summary_qd-1057]] (hướng dẫn tạm thời giai đoạn thí điểm).
- **Companion:** [[summary_qd-347]] (hướng dẫn chi tiết dân dụng + hạ tầng KT đô thị với LOD tables).
- **Overlays on:** [[summary_iso-19650-2]] (naming + status codes); [[summary_uk-bim-framework]] (CDE citation).
- **Defines:** [[cde]], [[bep]], [[eir]], [[midp-tidp]], [[lod-vn]], [[bim-delivery-roles]], [[information-container]].

## Nguồn

- [[raw/national-standards/VN/TaiLieu_HDC_2021]] — PDF 6.5 MB `ReferencesPDF/Tai_lieu_HHuong_dan_chung.pdf_20210415083307.pdf`. Đã extract pages 1-56/64 (phần còn lại là Phụ lục 01 use cases 1.4-1.9 + PL02-04, ngắn).
