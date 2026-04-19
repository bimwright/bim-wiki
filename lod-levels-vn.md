---
title: "Các mức LOD — Định nghĩa và Ánh xạ Việt Nam"
aliases: ["LOD levels", "LOD 100-500", "Mức LOD VN", "LOD definitions"]
tags: ["#bim", "#qd347", "#vietnam", "#concept", "#lod", "#reference"]
type: concept
source: "[[raw/national-standards/VN/QD_347_BXD]]"
status: draft
created: 2026-04-19
updated: 2026-04-19
---

# Các mức LOD — Định nghĩa và Ánh xạ Việt Nam

> **TL;DR:** QĐ 347 viện dẫn BIMForum 2019 LOD Spec (100-500) và triển khai qua Phụ lục 02 (Phase 2-5 ↔ LOD 200-500). Riêng MEP dùng song song **Bảng 7.4** với **% mức mô hình hoá** (10/30/60/90/100%) khác biệt — phụ kiện ống luôn trễ hơn ống chính 1 phase.

## Khái niệm cốt lõi

### 1. LOD 100-500 theo BIMForum 2019 (QĐ 347 viện dẫn)

`[COMMENTARY]` Tóm tắt định nghĩa chuẩn BIMForum, QĐ 347 không quote verbatim mà dùng làm tham chiếu cho Phụ lục 01-02.

| Mức | Tên tiếng Việt | Nội dung hình học | Nội dung phi hình học |
|---|---|---|---|
| **LOD 100** | Ý tưởng (Conceptual) | Ký hiệu / khối tổng quát (massing) — chưa có kích thước, vị trí xác định | Rất hạn chế |
| **LOD 200** | Tổng quát (Generic / Approximate) | Placeholder generic; kích thước, hình dáng, vị trí, số lượng xấp xỉ | Có thể gắn thông tin |
| **LOD 300** | Chính xác (Specific) | Cấu kiện cụ thể theo thiết kế; kích thước-vị trí-số lượng chính xác | Thuộc tính kỹ thuật đầy đủ theo TKKT |
| **LOD 350** | Có kết nối (Interface) | LOD 300 + **interfaces/kết nối** với các hệ thống khác | Như LOD 300 + data kết nối |
| **LOD 400** | Chế tạo (Fabrication) | Shop drawing level — sẵn sàng chế tạo + lắp đặt; chi tiết lắp ghép, dung sai | Manufacturer cụ thể (có thể), chi tiết kỹ thuật thi công |
| **LOD 500** | Hoàn công (As-built) | Field-verified sau thi công | Manufacturer data, số serial, ngày lắp đặt, as-built |

### 2. Ánh xạ Phase (QĐ 347 Phụ lục 02) ↔ LOD

`[VN-BXD:verified]` (QĐ 347 PDF page 55-56, Phụ lục 02 Master Attribute Palette)

| Phase | Giai đoạn VN | LOD tương đương | Nội dung điển hình |
|---|---|---|---|
| **2** | Thiết kế cơ sở (TKCS) | ~**LOD 200** | Mác bê tông, tiết diện, vật liệu, biện pháp thi công |
| **3** | Thiết kế kỹ thuật (TKKT) | ~**LOD 300** | Chi tiết liên kết, lớp hoàn thiện, sleeve/ống chờ, chống thấm |
| **4** | Thiết kế bản vẽ thi công (TKBVTC) | ~**LOD 400** | ID sản phẩm nhà sản xuất (**hiếm, chủ yếu cho cladding**) |
| **5** | Thi công | ~**LOD 500** | Tên nhà sản xuất, số serial, số định danh sản xuất (as-built) |

**Lưu ý quan trọng:** LOD 400 tại QĐ 347 **HIẾM khi bắt buộc có manufacturer ID** — chỉ "chủ yếu cho cladding" (ốp mặt dựng). Manufacturer data thật sự được yêu cầu ở **Phase 5 = LOD 500 (thi công/as-built)**.

### 3. MEP: Hai hệ thống song song

`[VN-BXD:verified]` QĐ 347 áp dụng **hai thang đo riêng biệt** cho MEP, không thay thế nhau:

**(a) Bảng 7.4 — Mức mô hình hoá MEP theo %** (PDF page 39, cho Phần 1 dân dụng):

| Giai đoạn | Mức MEP (%) | Clash tolerance |
|---|---|---|
| Thiết kế sơ bộ | **10%** | (không clash) |
| Thiết kế cơ sở | **30%** | (không clash) |
| Thiết kế kỹ thuật | **60%** | **±100mm** |
| **Giai đoạn đấu thầu** | **90%** | **±50mm** |
| Giai đoạn thi công | **100%** | **Triệt để** |

**(b) Phase 2-5 của Phụ lục 02** (áp dụng cho tất cả bộ môn gồm MEP, về thuộc tính phi hình học):
- Phase 2 (TKCS) ≈ LOD 200
- Phase 3 (TKKT) ≈ LOD 300
- Phase 4 (TKBVTC) ≈ LOD 400
- Phase 5 (Thi công) ≈ LOD 500

## Chi tiết / Triển khai

### 4. Pattern thuộc tính MEP theo Phase

`[VN-BXD:verified]` (QĐ 347 Phụ lục 02, PDF page 82+)

| Đối tượng | Phase chủ đạo (đầy đủ thuộc tính) | Đặc điểm |
|---|---|---|
| **MEP thiết bị** (chiller, AHU, FCU, máy phát, biến áp...) | **Phase 2 (TKCS)** | Sớm — vì cần tính toán công suất, lưu lượng, điện áp ngay từ TKCS để sizing hệ thống |
| **MEP phụ kiện ống** (co, tê, van, cút, bẫy) | **Phase 3 (TKKT)** | **Trễ hơn ống chính 1 phase** — khi có tuyến chính mới specify phụ kiện |
| **Tất cả** | **Phase 5 (thi công)** | Tên nhà sản xuất, số serial, số định danh — chỉ bắt buộc ở as-built |

### 5. Cấu trúc bảng MEP (Bảng 21.04 Phụ lục 02)

`[VN-BXD:verified]` (PDF page 82) Bảng MEP có header **khác biệt** so với Kiến trúc-Kết cấu:

**Thêm cột:** Phân loại hệ thống · Loại hệ thống · Tên hệ thống · Công suất · Công suất lạnh/sưởi · Điện áp · Tốc độ động cơ · Áp suất tĩnh Pa · Lưu lượng gió/nước · Loại bóng đèn

**Bỏ cột:** Cao độ chân/đỉnh · Diện tích · Khối tích · Chống cháy/Cách nhiệt/Cách âm

### 6. Per-discipline LOD ceiling

`[VN-BXD:verified]` (từ [[summary_qd-347]] + raw bảng Phụ lục 03)

| Bộ môn | Ceiling LOD | Ghi chú |
|---|---|---|
| Đường bộ / đường sắt | **LOD 300 từ TKCS; LOD 400 từ BVTC** | Khắt khe nhất trong hạ tầng (cao hơn mặc định 1 bậc) |
| Móng BT đúc sẵn | LOD 400 | + cốt thép (LOD 300), cường độ BT (LOD 350), dung sai cao độ + nhà sản xuất (LOD 400) |
| Đường ống hạ tầng | LOD 400 | LOD 350: vật liệu + công suất + hệ thống; LOD 400: + chiều dày vật liệu + vị trí van |
| Hệ thống thoát nước | LOD 400 | Trễ hơn ống hiện trạng 1 bậc |
| MEP dân dụng | (dùng Bảng 7.4 %) | **KHÔNG dùng LOD 100-500 trực tiếp** — dùng thang % mức mô hình hoá |

### 7. Worked example — "MEP LOD 400" nghĩa là gì?

`[COMMENTARY]` Khi stakeholder yêu cầu "MEP thiết kế theo LOD 400", theo QĐ 347 cần resolve thành:

**Về hình học (Phụ lục 01 — LOD hình học):**
- Cấu kiện MEP đạt chi tiết shop drawing — sẵn sàng chế tạo/lắp đặt
- Bao gồm: thiết bị chính + tuyến chính + **phụ kiện ống đầy đủ** (không còn trễ 1 phase)
- Kết nối liên bộ môn đã xử lý (interfaces)
- Theo Bảng 7.4: tương đương mức **90% (đấu thầu)** hoặc **100% (thi công)**
- Clash detection **±50mm** (đấu thầu) hoặc **triệt để** (thi công)

**Về phi hình học (Phụ lục 02 — Phase 4):**
- Các thuộc tính của Phase 2 + 3 đã có (công suất, lưu lượng, điện áp, áp suất tĩnh, vật liệu, kết nối, sleeve)
- Bổ sung **ID sản phẩm nhà sản xuất** — **nhưng QĐ 347 nói rõ "hiếm, chủ yếu cho cladding"**
- Nhà sản xuất cụ thể, số serial — **chưa bắt buộc** (đó là LOD 500/Phase 5)

**Ambiguity cần làm rõ trong BEP:**

QĐ 347 có **2 thang đo song song** cho MEP (% Bảng 7.4 vs Phase/LOD Phụ lục 02). Nếu hợp đồng nói "MEP LOD 400", phải xác định trong BEP/EIR:
1. Thang nào là chuẩn chính? (LOD 400 hay 90% hay 100%?)
2. Manufacturer data có bắt buộc không? (QĐ 347: không — trừ khi CĐT yêu cầu riêng)
3. Connections/kết nối xử lý triệt để chưa? (LOD 350 vs LOD 400)
4. Clash tolerance áp dụng ngưỡng nào?

**Khuyến nghị thực tiễn:** Thay vì dùng "LOD 400" một mình cho MEP, specify rõ trong EIR: *"MEP đạt mức mô hình hoá 90% theo Bảng 7.4 QĐ 347 tại giai đoạn đấu thầu, clash tolerance ±50mm, thuộc tính phi hình học đạt Phase 4 Phụ lục 02 ngoại trừ manufacturer ID (hoãn đến Phase 5)."*

## Quan hệ

- **Parent:** [[lod-vn]] (triết lý tách hình học/phi hình học; trang này cung cấp chi tiết levels).
- **Defined in:** [[summary_qd-347]] Phụ lục 01-04 + Section 7.4.
- **Contradicts:** [[loin]] (ISO 19650 dùng LOIN per-purpose thay vì LOD tiering).
- **Applied in:** [[summary_bep-template-qd348]], [[summary_pre-bep-template-qd348]] (template có mục LOD theo cấu kiện/giai đoạn).
- **Context:** [[summary_taileu-hdc-2021]] Section 3.4.7 (LOD là khung chung; per-component; 4 mục đích).

## Nguồn

- [[raw/national-standards/VN/QD_347_BXD]] `[VN-BXD:verified]`:
  - Section 2 "Mức độ phát triển thông tin (LOD)" (PDF page 8) — reference BIMForum 2019
  - Section 7 "Yêu cầu thông tin Bộ môn Cơ điện (MEP)" (PDF page 31-39) — Bảng 7.4
  - Phụ lục 02 Master Attribute Palette (PDF page 55-114 partial) — ánh xạ Phase 2-5 ↔ LOD 200-500
  - Phụ lục 03 LOD hạ tầng — per-discipline LOD ceilings
- BIMForum 2019 LOD Specification — ngoài phạm vi repo, chỉ được QĐ 347 viện dẫn. Không có raw file.
- [[raw/national-standards/VN/TaiLieu_HDC_2021]] `[VN-BXD:verified]` Section 3.4.7 — confirm "LOD áp dụng cho từng thành phần mô hình cụ thể, không cho toàn mô hình".
