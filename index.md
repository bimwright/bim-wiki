---
title: "BIM Wiki — Master Index"
type: index
updated: 2026-04-18
---

# BIM Wiki — Index

> Catalog of all wiki pages. Updated by the agent on every ingest. Humans read top-down. Format per line: `- [[slug]] — TL;DR first sentence (max 120 chars)`.

## Entities
<!-- pages where frontmatter.type == entity, alphabetical -->
- [[iso-19650]] — Bộ tiêu chuẩn quốc tế 6 phần (ISO/TC 59/SC 13) định nghĩa quản lý thông tin BIM trong toàn vòng đời tài sản xây dựng.

## Concepts
<!-- pages where frontmatter.type == concept, alphabetical -->
- [[aim]] — Mô hình thông tin tài sản trong giai đoạn vận hành; được khởi tạo từ PIM khi bàn giao và cập nhật liên tục.
- [[bep]] — Tài liệu delivery team lập để đáp ứng EIR; có hai phiên bản (pre-appointment và post-appointment).
- [[bim]] — Cách tiếp cận quản lý thông tin toàn vòng đời tài sản xây dựng dựa trên mô hình số phối hợp.
- [[bim-delivery-roles]] — Ba vai trò cốt lõi ISO 19650-2: Appointing Party, Lead Appointed Party, Appointed Party.
- [[cde]] — Môi trường dữ liệu chung với workflow 4 trạng thái: WIP → Shared → Published → Archive.
- [[eir]] — Yêu cầu trao đổi thông tin do Appointing Party phát hành; specify LOIN, format, timeline cho từng giao nộp.
- [[exchange-criteria]] — 6 tiêu chuẩn (6 Cs) áp dụng đánh giá quality assurance mỗi lượt Information Exchange (Decision A/B).
- [[federation]] — Tạo composite information model từ các information containers riêng biệt của nhiều task teams; nền tảng collaborative production.
- [[hs-schema]] — Cấu trúc dữ liệu 4 phân hệ liên kết đánh giá rủi ro An toàn và Sức khỏe H&S tích hợp thẳng vào mô hình thông tin.
- [[information-container]] — Đơn vị lưu trữ thông tin trong BIM — file/model/schedule/doc có tên xác định và managed trong CDE.
- [[information-requirements-hierarchy]] — Hierarchy 4 tầng OIR → AIR/PIR → EIR cascade yêu cầu từ tổ chức xuống dự án.
- [[lod-vn]] — Hệ thống Mức độ phát triển thông tin (LOD) rẽ nhánh của Việt Nam dựa trên BIMForum thay cho LOIN quốc tế.
- [[lod-levels-vn]] — Chi tiết LOD 100-500 (BIMForum), ánh xạ Phase 2-5 QĐ 347 ↔ LOD, Bảng 7.4 %MEP, worked example "MEP LOD 400".
- [[loin]] — Level of Information Need (ISO 19650-1) — mức độ thông tin cần thiết cho một mục đích cụ thể; thay thế khái niệm LOD.
- [[midp-tidp]] — TIDP (per task team) + MIDP (aggregated) — kế hoạch giao nộp: ai produce gì, khi nào, format nào.
- [[pim]] — Mô hình thông tin dự án tích lũy trong giai đoạn thiết kế và thi công; handover thành AIM khi bàn giao vận hành.
- [[sensitivity-assessment]] — Đánh giá tính nhạy cảm (Clause 4, Part 5) để đưa ra quyết định Security Triage cho dự án.
- [[trigger-event]] — Sự kiện kích hoạt loại 1 (lên lịch trước) hoặc 2, 3 (bất thường) khởi chạy chu trình cập nhật lại thông tin AIM.
- [[uk-national-annex]] — Phụ lục Quốc gia Anh quy định mã trạng thái CDE (S0-S7), phân loại Uniclass 2015 và khái niệm Golden Thread.

## Comparisons
<!-- pages where frontmatter.type == comparison, alphabetical -->
- [[bep-template-qd348-variants]] — So sánh BEP Template QĐ 348: base (Markdown + commentary + signature) vs V1_StandardFit (paper-form, bám Phụ lục 03 gốc).
- [[pas-1192-mapping]] — Bảng đối chiếu thuật ngữ và tiêu chuẩn giữa bộ PAS 1192 (ngôn ngữ cũ của UK) sang ISO 19650 (quốc tế).
- [[pre-bep-template-qd348-variants]] — So sánh Pre-BEP QĐ 348: base (Markdown + signature + commentary) vs V1_StandardFit (paper-form, bám Mẫu số 6a).

## Meta
<!-- pages where frontmatter.type == meta, alphabetical -->
- [[iso-19650-revision-watch]] — Tracker meta cho stage ISO/DIS và edition hiện hành của ISO 19650; căn cứ raw revision-watch/Status.md.

## Summaries
<!-- pages where frontmatter.type == summary, alphabetical, one per ingested source -->
- [[summary_bep-template-qd348]] — Tóm tắt mẫu BEP theo QĐ 348: cấu trúc thực thi, biểu mẫu 01-08, CDE, MIDP/TIDP, LOD và naming convention.
- [[summary_iso-19650-1]] — Tóm tắt ISO 19650-1 (13 clauses): information requirements hierarchy, delivery cycle, CDE workflow, federation, LOIN, MIDP/TIDP.
- [[summary_iso-19650-2]] — Tóm tắt ISO 19650-2: quy trình 8 bước delivery phase, CDE mapping, hai bước authorization, EIR cascade.
- [[summary_iso-19650-3]] — Tóm tắt ISO 19650-3: 8 bước dạng vòng lặp duy trì liên tục, trigger events, hệ thống CAFM/CMMS, gộp AIM.
- [[summary_iso-19650-4]] — Tóm tắt ISO 19650-4: 3 bước information exchange, 6 Cs criteria, ưu tiên định dạng open schema.
- [[summary_iso-19650-5]] — Tóm tắt ISO 19650-5: Lớp phủ security, đánh giá risk 4 bước, yêu cầu bảo mật dội xuống supply chain.
- [[summary_iso-19650-6]] — Tóm tắt ISO 19650-6: Lớp phủ H&S (sức khỏe an toàn), database sub-schemas rủi ro, map thông tin IFC.
- [[summary_iso-19650-overview]] — Tổng quan bộ tiêu chuẩn ISO 19650 gồm 6 phần, kiến trúc phụ thuộc, quy trình 8 giai đoạn và các acronym cốt lõi.
- [[summary_pre-bep-template-qd348]] — Tóm tắt mẫu Pre-BEP theo QĐ 348: control table, 7 mục nội dung tối thiểu và khối xác nhận cho tender / pre-appointment.
- [[summary_qd-347]] — Quyết định 347: Tiêu chuẩn cơ sở Việt Nam, quy định rõ quy tắc mã màu, clash detection và bảng LOD dân dụng-hạ tầng.
- [[summary_qd-348]] — Quyết định 348: Văn bản vĩ mô Việt Nam, định dạng CDE 4 phân vùng, ISO quy tắc đặt tên, và cung cấp Template EIR/BEP.
- [[summary_revit-handover]] — Hướng dẫn xử lý nội file mô hình BIM (Revit) qua CDE Gate: Purge, Audit, Detach, Worksets và Design Options.
- [[summary_status]] — Trạng thái soát xét ISO 19650 (DIS 2026, bảng edition/stage, thay đổi đề xuất có thẻ commentary).
- [[summary_luat-60-2024]] — Luật Dữ liệu 60/2024/QH15 (hiệu lực 01/07/2025): khung cấp Luật chi phối mọi dữ liệu số VN; không nhắc BIM trực tiếp.
- [[summary_nd-111-2024]] — NĐ 111/2024 (hiệu lực 01/11/2024): khung CSDL quốc gia hoạt động XD; không nhắc BIM trực tiếp, cha của TT 24/2025.
- [[summary_nd-175-2024]] — NĐ 175/2024 Điều 8 (hiệu lực 30/12/2024): BIM bắt buộc cho nhóm B + cấp II trở lên; IFC 4.0, ≤500MB/tệp.
- [[summary_qd-1004]] — QĐ 1004/QĐ-BXD (2020): kế hoạch chuyển đổi số ngành XD 2020-2025 với mục tiêu 10% dự án áp dụng BIM vào 2025.
- [[summary_qd-1056]] — QĐ 1056/QĐ-BXD (2017): chương trình khung đào tạo BIM (28h QLDA/CĐT + 48h tư vấn/nhà thầu) giai đoạn thí điểm.
- [[summary_qd-1057]] — QĐ 1057/QĐ-BXD (2017): hướng dẫn tạm thời 8 phần áp dụng BIM giai đoạn thí điểm; đã bị QĐ 348 thay thế phần lớn.
- [[summary_qd-2500-ttg]] — QĐ 2500/QĐ-TTg (2016): đề án áp dụng BIM giai đoạn thí điểm 2017-2021; lộ trình đã bị QĐ 258/2023 kế nhiệm.
- [[summary_qd-258-ttg]] — QĐ 258/QĐ-TTg (2023): lộ trình BIM bắt buộc 4 mốc 2023-2026 theo cấp công trình × nguồn vốn.
- [[summary_qd-66-bcdbim]] — QĐ 66/QĐ-BCĐBIM (2021): công bố 4 phần tài liệu đào tạo BIM tại bim.gxd.vn, hiện thực hoá QĐ 1056.
- [[summary_taileu-hdc-2021]] — Tài liệu HDC BIM (Bộ XD, 2021): hướng dẫn body đính kèm QĐ 348, chi tiết CDE, naming ISO 19650-2, 9 use case BIM.
- [[summary_tt-09-2024]] — TT 09/2024/TT-BXD (hiệu lực 15/10/2024): chi phí BIM theo % chi phí thiết kế; ≤50% tổng, ≤20% TKBVTC.
- [[summary_tt-24-2025]] — TT 24/2025/TT-BXD (hiệu lực 15/10/2025): hướng dẫn CSDL quốc gia XD; BIM xuất hiện gián tiếp Phụ lục III "nếu có".
- [[summary_uk-bim-framework]] — UK BIM: Bản phác thảo (stub) khung tài liệu hướng dẫn thực hành ISO 19650 từ Vương quốc Anh (Part A-F).

## Overviews
<!-- pages where frontmatter.type == overview, alphabetical -->
<!-- (empty) -->

## Syntheses
<!-- pages where frontmatter.type == synthesis, alphabetical -->
- [[bim-applicability-matrix-vn]] — Hai bộ tiêu chí song song (QĐ 258 cấp×vốn×năm; NĐ 175 nhóm×cấp) quyết định bắt buộc BIM; chờ TT hướng dẫn giải mâu thuẫn.
- [[vn-bim-landscape]] — Landscape BIM VN: 4 tầng pháp lý + TCVN, không có QCVN BIM, bộ ngành khác chưa có TT dedicated BIM.
