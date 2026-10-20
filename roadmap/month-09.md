# Tháng 09 — Multimodal (VLM) + Agents + Fine-tuning

> **Mục tiêu:** kết hợp Computer Vision với LLM, xây agent có kiểm soát, biết khi nào nên fine-tune.
> **Bổ trợ:** MCP, LangGraph, PEFT/Unsloth.
> **Project:** **Trợ lý kỹ thuật nhà máy**: chụp ảnh lỗi → VLM mô tả → RAG tra hướng dẫn xử lý → agent tạo phiếu bảo trì → app iOS.
> **Tài liệu:** paper CLIP, LLaVA, Qwen-VL; tài liệu MCP; LangGraph docs; Hugging Face PEFT; Unsloth.

[⬅ Tháng 08](month-08.md) · [README](../README.md) · [Tháng 10 ➡](month-10.md)

---

## Tuần 1 — Vision-Language Model

- [ ] **Ngày 241 (T2)** — 📖 Tổng quan VLM: CLIP, LLaVA, Qwen-VL (cách ghép vision encoder với LLM)
- [ ] **Ngày 242 (T3)** — 💻 CLIP: zero-shot classification, tìm ảnh bằng câu mô tả
- [ ] **Ngày 243 (T4)** — 💻 Dùng VLM (API hoặc local) mô tả ảnh lỗi sản phẩm từ MVTec
- [ ] **Ngày 244 (T5)** — 💻 VLM đọc tài liệu/nhãn sản phẩm → JSON có cấu trúc
- [ ] **Ngày 245 (T6)** — 📖 So sánh VLM với YOLO/PatchCore: khi nào dùng cái nào (tốc độ, chi phí, độ chính xác)
- [ ] **Ngày 246 (T7)** — 🛠 Project: module "ảnh lỗi → mô tả có cấu trúc"
- [ ] **Ngày 247 (CN)** — 🔁 Ôn tuần · note *"VLM vs model CV chuyên biệt"* · commit

## Tuần 2 — Agents

- [ ] **Ngày 248 (T2)** — 💻 Tự viết agent loop không dùng framework
- [ ] **Ngày 249 (T3)** — 📖 Thiết kế tool tốt: tên, mô tả, input/output, xử lý lỗi
- [ ] **Ngày 250 (T4)** — ⭐ MCP: viết MCP server đơn giản (ví dụ tra tồn kho linh kiện)
- [ ] **Ngày 251 (T5)** — ⭐ LangGraph: state, node, edge
- [ ] **Ngày 252 (T6)** — 💻 Human-in-the-loop: agent phải xin xác nhận trước hành động quan trọng
- [ ] **Ngày 253 (T7)** — 🛠 Project: agent tạo phiếu bảo trì từ mô tả lỗi + RAG tháng 8
- [ ] **Ngày 254 (CN)** — 🔁 Ôn tuần · commit

## Tuần 3 — Fine-tuning

- [ ] **Ngày 255 (T2)** — 📖 Khi nào fine-tune, khi nào RAG là đủ · LoRA/QLoRA
- [ ] **Ngày 256 (T3)** — 💻 Chuẩn bị dataset instruction (ví dụ chuẩn hóa phiếu bảo trì)
- [ ] **Ngày 257 (T4)** — 💻 Fine-tune model nhỏ bằng Unsloth/PEFT trên Colab
- [ ] **Ngày 258 (T5)** — 💻 So sánh base vs fine-tuned vs base + RAG trên bộ eval
- [ ] **Ngày 259 (T6)** — 📖 Distillation: dùng model lớn sinh dữ liệu dạy model nhỏ
- [ ] **Ngày 260 (T7)** — 🛠 Project: kết luận fine-tune có đáng không, kèm số liệu và chi phí
- [ ] **Ngày 261 (CN)** — 🔁 Ôn tuần · note *"Fine-tune hay RAG?"* · commit

## Tuần 4 — Ghép hệ thống

- [ ] **Ngày 262 (T2)** — 💻 Ghép: ảnh → VLM → RAG → agent → phiếu bảo trì
- [ ] **Ngày 263 (T3)** — 💻 Eval end-to-end trên 30 ca thử
- [ ] **Ngày 264 (T4)** — 📖 Bảo mật: prompt injection ẩn trong tài liệu/ảnh · 💻 Thêm lớp kiểm tra
- [ ] **Ngày 265 (T5)** — ⭐ App iOS: chụp ảnh gửi lên hệ thống, nhận phiếu đề xuất
- [ ] **Ngày 266 (T6)** — ⭐ docker compose toàn hệ thống
- [ ] **Ngày 267 (T7)** — 🛠 Project: **Trợ lý kỹ thuật nhà máy v1** + video demo
- [ ] **Ngày 268 (CN)** — 🔁 Ôn tháng · blog · **tự kiểm tra mốc Quý 3** · commit

## Dự phòng

- [ ] **Ngày 269** — Bù phần trễ / làm lại phần còn yếu
- [ ] **Ngày 270** — Bù phần trễ / tự kiểm tra mốc tháng

---

## ✅ Mốc cuối tháng (và Quý 3)

- [ ] Dùng VLM trích xuất thông tin có cấu trúc từ ảnh
- [ ] Tự viết agent loop và một MCP server
- [ ] Fine-tune được model nhỏ bằng LoRA, so sánh bằng số liệu
- [ ] Một sản phẩm kết hợp CV + LLM chạy end-to-end, có eval
