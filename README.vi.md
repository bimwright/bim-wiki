---
title: "bim-wiki"
updated: 2026-04-20
---

<p align="center">
  <img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" width="360" />
</p>

<p align="center">
  📖 <a href="README.md">English</a> · Tiếng Việt · <a href="README.zh-CN.md">简体中文</a>
</p>

---

# bim-wiki

Mình bắt đầu viết mấy cái note này cho chính mình. Mỗi lần viết BEP là một lần phải tra chéo ISO 19650 với 4 quyết định (QĐ 347, QĐ 348, QĐ 1057, QĐ 2500) để hiểu thuật ngữ nào đang thực sự áp dụng cho dự án — và lần nào đóng máy xong là lần đó quên sạch mapping.

Cái repo này là cái mapping đó, được viết ra.

**bim-wiki** là knowledge base BIM có curate. Tổng hợp tiếng Việt ISO 19650 Parts 1–6, đặt song song với khung pháp lý BIM Việt Nam (4 QĐ trên + Luật 60/2024, Nghị định 111/2024 và 175/2024, Thông tư 09/2024 và 24/2025). Kèm các trang khái niệm — CDE, LOIN, PIM/AIM, EIR cascade, BEP templates — cross-link giữa chuẩn quốc tế và thực hành trong nước.

52 trang markdown, CC-BY-SA 4.0, paraphrase từ nguồn (không copy nguyên văn). Nếu anh/chị cần normative text của ISO, mua trực tiếp từ iso.org — wiki này không thay thế được.

## Dành cho ai

- BIM practitioner ở VN đang phải juggle ISO 19650 với quy định trong nước trong cùng một tài liệu.
- BIM Coordinator đang viết BEP / pre-BEP theo template QĐ 348.
- Sinh viên + kỹ sư hay quên term nào nghĩa là gì (LOIN vs LOD, PIM vs AIM, federation vs aggregation, CDE states vs revision states).
- AI agent cần domain grounding cho BIM — các trang viết sao cho cả người đọc lẫn LLM đều parse được.

## Có gì bên trong

- **`summary_*.md`** — summary cấp chương của từng source document (mỗi ISO 19650 part, mỗi QĐ/Luật/NĐ/TT của VN).
- **Trang khái niệm** — `cde.md`, `eir.md`, `pim.md`, `loin.md`, `bep.md`, `lod-vn.md`, và ~30 trang nữa. Mỗi trang 1 topic, cross-link lẫn nhau.
- **Delta VN** — `lod-vn.md`, `bim-applicability-matrix-vn.md`, `bep-template-qd348-variants.md`: chỗ thực hành VN lệch với ISO, và lệch vì lý do gì.
- **`iso-19650.md`** — trang cha của series.
- **`index.md`** — catalog tổng.

## Đọc sao

Bắt đầu từ [`index.md`](index.md) cho catalog đầy đủ, hoặc nhảy thẳng vào 1 concept page nếu anh/chị đã biết mình cần gì.

### Tag nguồn

Mỗi trang đều có tag để anh/chị biết mệnh đề nào dựa trên bằng chứng gì:

- `[ISO-CORE:verified]` — đối chiếu với bản ISO gốc (mình giữ bản tham chiếu local; chỉ *nội dung factual* được diễn đạt lại, không phải wording).
- `[ISO-CORE:structure]` — theo cấu trúc clause của ISO nhưng chưa verbatim-verify.
- `[VN-BXD:verified]` — đối chiếu với PDF nguồn VN.
- `[COMMENTARY]` — tổng hợp / so sánh của bimwright.
- `[INFERRED]` — suy luận logic, không có source trực tiếp.

Nếu 1 statement quan trọng cho dự án, trace về tag nguồn trước khi dựa vào.

## License & attribution

Giấy phép **CC-BY-SA 4.0** — xem [`LICENSE`](LICENSE).

License phủ **đóng góp gốc** của bimwright: summary, paraphrase, chọn lọc, sắp xếp, commentary. License **không** cấp quyền lên standard gốc. Xem [`NOTICE.md`](NOTICE.md) cho policy per-source — source nào paraphrase theo fair-use / fair-dealing, source nào là văn bản nhà nước VN (công khai), source nào vẫn thuộc rights-holder gốc.

Nếu anh/chị cần normative text của ISO, mua từ iso.org. Wiki này không thay thế được.

## Contributing

Mở issue để đề xuất trang mới hoặc báo lỗi. Với pull request — xem [`NOTICE.md`](NOTICE.md). Quy tắc chính: **paraphrase, đừng paste.** Trích nguyên văn từ standard có bản quyền sẽ bị reject dù edit có thiện chí và nội dung đúng. Mô hình dual-tier chỉ work khi tier public giữ sạch.

---

Thuộc family [bimwright](https://github.com/bimwright) —
[rvt-mcp](https://github.com/bimwright/rvt-mcp) (cầu nối Revit ↔ LLM) · bim-wiki (repo này) · còn nữa trên forge.

---

<p align="center">
  Một dự án của <a href="https://github.com/bimwright">bimwright</a> —
  <a href="https://github.com/bimwright"><img src="https://raw.githubusercontent.com/bimwright/.github/master/assets/logos/bimwright-logo.png" alt="bimwright" height="24" align="middle" /></a>
</p>
