---
title: "Hướng dẫn chuyển giao file Revit"
aliases: ["Revit Handover", "Revit Handover Practice"]
tags: ["#bim", "#guidance", "#revit", "#cde", "#summary"]
type: summary
source: "[[raw/guidance/Revit-File-Handover-Guide]]"
status: draft
created: 2026-04-18
updated: 2026-04-18
---

# Hướng dẫn xử lý file Revit trước chuyển giao

> **TL;DR:** Hướng dẫn thực hành nội bộ thực địa hóa hệ thống CDE (WIP → Shared → Published) qua các thao tác phần mềm Revit: quản trị Worksets, Purge rác, Audit lỗi, loại bỏ Link rác và cô lập (Detach) file gửi bên thứ 3 nhằm bảo mật cấu trúc thiết kế.

## Nội dung tóm tắt

Văn bản này chuyển giao các kiến thức vĩ mô từ [[iso-19650]] và tài liệu [[summary_qd-348]] (CDE) thành 3 kịch bản thao tác thực tiễn qua cổng CDE Gate:

### Scenario 1: WIP → Shared (Cổng Gate 1 — Phối hợp)
- Mấu chốt dọn dẹp nội bộ trước khi chia sẻ ra các bộ môn khác.
- Đảm bảo **Purge** từ 2-3 lần (để quét sạch cấu kiện thừa) và **Audit** trên Central file.
- Chuẩn hóa tên Worksets để vô danh hóa, xóa sổ các view nháp mang tên Kỹ thuật viên (Modeler).

### Scenario 2: Shared → Published (Cổng Gate 2 — Pháp lý)
- Mấu chốt là thiết lập mô hình chốt phục vụ giao nộp.
- Xóa sổ các phương án **Design Options** bị loại để ra main model cuối.
- Dọn dẹp Sheet Set đảm bảo khớp đúng phân phối MIDP. Áp quy tắc Naming Convention của QĐ 348.

### Scenario 3: Export (Gửi ra ngoài tổ chức)
- Xuất file tách biệt hoàn toàn để bảo vệ Server gốc bằng lệnh **Detach from Central**, giải phóng hoàn toàn các mắt xích Worksets.
- Rút toàn bộ Text/Revision Cloud nháp, quyết định gộp file gốc (remove ALL links) hay gửi kèm bundle nguyên bộ (chuyển Relative path).

## Quan hệ

- **Implements:** [[cde]], hệ quy tắc dung sai trong [[summary_qd-347]].
- **Actors:** Kỹ thuật viên (Modeler) thao tác quy trình ↔ Quản lý BIM / Điều phối BIM (Leader/Coordinator) là người check soát lỗi ở Gate 1 & 2. (Xem [[bim-delivery-roles]]).

## Nguồn

- [[raw/guidance/Revit-File-Handover-Guide]] — Checklist và Hướng dẫn thao tác quy chuẩn cho phần mềm Revit theo tư duy CDE.
