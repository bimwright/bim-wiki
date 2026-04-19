---
title: "Quyết định 347/QĐ-BXD (Hướng dẫn chi tiết BIM)"
aliases: ["QD 347", "QĐ 347/QĐ-BXD", "Vietnam BIM Guide 347"]
tags: ["#bim", "#qd347", "#vietnam", "#standard", "#summary"]
type: summary
source: "[[raw/national-standards/VN/QD_347_BXD]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# Quyết định 347/QĐ-BXD — Hướng dẫn chi tiết áp dụng BIM

> **TL;DR:** QĐ 347/QĐ-BXD (2021) là hướng dẫn chi tiết BIM tại Việt Nam cho Dân dụng + Hạ tầng đô thị: mã màu MEP, quy trình clash detection có dung sai, và hệ LOD Việt hóa (hình học tách khỏi phi hình học) ánh xạ vào 4 giai đoạn thiết kế bản địa.

## Nội dung tóm tắt

### 1. Dân dụng: Kiến trúc - Kết cấu - Cơ điện
`[VN-BXD:verified]` Cung cấp bộ quy định cứng tay cho nhóm làm nghề:
- **Định dạng mở:** IFC/DXF (Kiến trúc, kết cấu), BCF (phối hợp va chạm), gbXML (năng lượng).
- **Mã màu MEP:** Gắn mã màu RGB cụ thể (vd: nước lạnh 0,63,255; nước nóng 255,60,60; báo cháy 255,0,0) tham khảo từ chuẩn GSA Mỹ.
- **Xử lý xung đột (Clash detection):** Lập quy trình 7 bước, quy định dung sai va chạm hợp pháp (±100mm ở TK Kỹ Thuật, ±50mm lúc Đấu thầu). Quy định loại trừ ống <50mm khỏi clash check MEP.

### 2. Hạ tầng kỹ thuật (Giao thông, Cấp thoát nước)
Quy định cực kỳ tỉ mỉ về mô hình bề mặt (Surface topology): 
- Điểm Breaklines tại các nút cong phải dưới cự ly tối đa (vd R<39 thì điểm cách 0.5m), không cho tam giác lưới cắt qua Breakline.
- **Giao thông** là bộ môn khắt khe nhất, yêu cầu LOD 300 từ Thiết kế cơ sở và LOD 400 từ Bản vẽ thi công.
- Có thư viện quy chuẩn phụ lục riêng phục vụ hệ thống Cầu tĩnh (Phụ lục 04).

### 3. Vấn đề LOD 
Trong khi thế giới theo ISO 19650 đang chuyển sang LOIN, QĐ 347 dựa vững chắc vào **BIMForum (2019) Level of Development Specification**. Sự sáng tạo là nó chẻ phân định riêng bảng LOD Không Gian Hình Học (Phụ lục 1 & 3) và LOD Thông tin Phi Hình học (Phụ lục 2 & 4). 
- *(Xem chi tiết tại [[lod-vn]])*

## Quan hệ

- **Companion:** QĐ 348/QĐ-BXD (Văn bản vĩ mô về khung quản lý - ISO 19650).
- **Relates to:** [[bim-delivery-roles]] (Vai trò thành viên), [[loin]].
- **New concepts:** [[lod-vn]]

## Nguồn

- [[raw/national-standards/VN/QD_347_BXD]] — Nguồn nội dung pháp lý chính để lập hướng dẫn này.
