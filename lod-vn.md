---
title: "Mức độ phát triển thông tin (LOD) theo tiêu chuẩn Việt Nam"
aliases: ["LOD VN", "LOD", "Level of Development VN"]
tags: ["#bim", "#qd347", "#vietnam", "#concept", "#lod"]
type: concept
source: "[[raw/national-standards/VN/QD_347_BXD]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# Mức độ phát triển thông tin LOD (Tiêu chuẩn Việt Nam)

> **TL;DR:** QĐ 347 dùng hệ LOD 100-500 của BIMForum (Mỹ) thay vì LOIN của ISO 19650. Bản sắc VN: tách LOD hình học (Phụ lục 01/03) và LOD phi hình học (Phụ lục 02/04), ánh xạ vào 4 giai đoạn thiết kế bản địa.

## Khái niệm cốt lõi

- **LOD (Level of Development):** Thước đo quy định tính năng độ chi tiết cấu tạo hữu hình (có nhìn thấy được) và mức độ thông tin nhúng (metadata) mà một phần tử mô hình cần đạt được.
- Được quy chiếu từ văn bản `BIMForum, Level of Development (LOD) Specification 2019 Part I`.
- **4 Giai đoạn thiết kế Việt Nam:** (1) Thiết kế sơ bộ → (2) Thiết kế cơ sở → (3) Thiết kế Kỹ thuật  → (4) Cấp Bản vẽ thi công (BVTC).

## Chi tiết / Triển khai

`[VN-BXD:verified]`
Tại QĐ 347, thay vì định nghĩa chung chung, LOD được băm nhỏ thành các Phụ lục quy chuẩn bảng biểu:

1. **LOD Hình Học (Phụ lục 01 & 03):** 
   - Liệt kê cụ thể từng bộ phận.
   - Thường thì: Cơ sở (LOD 100-200), Kỹ thuật (LOD 200-300), BVTC (LOD 350-400). Duy nhất *Đường bộ/Đường sắt* phải đạt LOD 300 từ Thiết kế cơ sở.

2. **LOD Phi Hình Học (Phụ lục 02 & 04):** 
   - Chứa Master Attribute Palette (Tham số nhận dạng, Tham số định vị, Hình học, Quy cách Kỹ thuật, Vật liệu).
   - Đánh số Phase 2/3/4/5 lên từng thông số trên lưới Bảng phân loại chuẩn OmniClass. Chẳng hạn: Số Sê ri sản xuất hay Model Name chỉ bị bắt buộc dán vào lúc thi công as-built (Phase 5 - tức LOD 500).

3. **Mô hình đặc biệt (Cầu):** Phụ lục 4 cho hạng mục Cầu không dùng đánh số LOD 100-400 mà dùng 3 phase chuyên biệt là Design, Manufacture (Đúc sẵn dầm Super T / dự ứng lực ở xưởng), và Construction nhằm phản ánh thực tiễn thiết kế thi công công trình nhịp lớn tại Việt Nam.

## Quan hệ

- **Contradicts:** [[loin]] — QĐ 347 dùng bản chất LOD 100-500 thay thế cho LOIN (Level of Information Need) hiện đại của ISO.
- **Parent:** Hướng dẫn chính thức tại [[summary_qd-347]].
- **Detail:** [[lod-levels-vn]] — Định nghĩa LOD 100-500 BIMForum, ánh xạ Phase 2-5 (QĐ 347 Phụ lục 02) ↔ LOD, Bảng 7.4 %MEP, pattern phụ kiện trễ 1 phase, worked example "MEP LOD 400".

## Nguồn

- [[raw/national-standards/VN/QD_347_BXD]] — Các phụ lục 01, 02, 03, 04 mô tả hệ quy chiếu chuẩn chỉnh cho Việt Nam.
- [[raw/national-standards/VN/templates/BEP_Template_QD348]] `[VN-BXD:verified]` — Mục 6 và Biểu mẫu 03 trong mẫu BEP thể hiện bảng LOD theo cấu kiện, bám theo khung chuẩn vận hành dự án — [[summary_bep-template-qd348]]
- [[raw/national-standards/VN/templates/Pre_BEP_Template_QD348]] `[VN-BXD:verified]` — Mẫu Pre-BEP có mục LOD theo hạng mục / giai đoạn, dùng làm khung xác nhận mức độ chi tiết mô hình trước khi chốt BEP — [[summary_pre-bep-template-qd348]]
- [[raw/national-standards/VN/TaiLieu_HDC_2021]] `[VN-BXD:verified]` (Section 3.4.7) — Thuật ngữ chính thức là **"Mức độ phát triển thông tin (LOD)"** (ánh xạ Level of Development, BIMForum); LOD áp dụng cho **từng thành phần mô hình cụ thể, không cho toàn bộ mô hình**; 4 mục đích: định nghĩa thông tin đầu vào, giải thích cho bên liên quan, xác định khả năng sử dụng, tham chiếu trong Hợp đồng và BEP. LOD **bổ sung** cho BEP, không thay thế — [[summary_taileu-hdc-2021]]
- [[raw/national-standards/VN/QD_1057_BXD]] `[VN-BXD:web-verified]` — QĐ 1057 Phần V (2017) dùng thuật ngữ cũ **"Mức độ phát triển (LOD) 100-400"** (không có "thông tin" trong tên); chính thức được đổi thành "Mức độ phát triển thông tin" khi công bố bộ hướng dẫn 2021 — [[summary_qd-1057]]

## LOID / biến thể thuật ngữ gần

`[COMMENTARY]` Khảo sát toàn bộ 13 raw VN cấp quốc gia (2026-04): **KHÔNG có thuật ngữ "LOID"** trong bất kỳ văn bản nào. Các biến thể gần LOD có thể dễ nhầm:

| Thuật ngữ | Định nghĩa | Nguồn | Có trong repo? |
|---|---|---|---|
| **LOD** — Level of Development | Chất lượng + số lượng + mức chi tiết thông tin mô hình tại từng giai đoạn | BIMForum | ✅ QĐ 347, 348, 1057, TaiLieu_HDC |
| **LOIN** — Level of Information Need | Mức thông tin cần cho mục đích cụ thể | ISO 19650-1 | ✅ Tại [[loin]] (ISO-core); TCVN 14177-1:2024 có thuật ngữ VN nhưng raw TCVN không trong repo |
| **LOI** — Level of Information | Phần phi hình học của LOD | BIMForum (tiền thân) | Gián tiếp trong QĐ 347 Phụ lục 02/04 (LOD phi hình học) |
| **LoD** — Level of Definition | Biến thể UK (PAS 1192) | PAS 1192 | Gián tiếp trong [[pas-1192-mapping]] |
| **LoMD** — Level of Model Detail | Biến thể (ít dùng) | — | ❌ |
| **LOID** | — (không phải thuật ngữ tiêu chuẩn) | — | ❌ |

Nếu văn bản VN cấp ngành khác ban hành sau 2026-04 có dùng LOID hoặc biến thể, cần bổ sung raw + cập nhật bảng này.
