# Tháng 08 — RAG + Evals

> **Mục tiêu:** xây RAG đúng chuẩn production và đo chất lượng bằng số liệu, không đoán.
> **Bổ trợ:** PostgreSQL + pgvector, full-text search / OpenSearch, OCR, xử lý PDF.
> **Project:** RAG trên **tài liệu kỹ thuật** (hướng dẫn vận hành máy, quy trình bảo trì) kèm eval suite tự động.
> **Tài liệu:** pgvector docs, sentence-transformers, Langfuse docs, PaddleOCR, các bài viết về RAG evaluation.

[⬅ Tháng 07](month-07.md) · [README](../README.md) · [Tháng 09 ➡](month-09.md)

---

## Tuần 1 — RAG cơ bản

- [ ] **Ngày 211 (T2)** — 📖 Embedding, độ tương đồng vector, vector database
- [ ] **Ngày 212 (T3)** — ⭐ PostgreSQL + pgvector bằng Docker, tạo index HNSW
- [ ] **Ngày 213 (T4)** — 📖 Chiến lược chunking (kích thước, overlap, theo cấu trúc tài liệu)
- [ ] **Ngày 214 (T5)** — 💻 Pipeline ingest: PDF → text → chunk → embed → lưu DB
- [ ] **Ngày 215 (T6)** — 💻 Retrieval + sinh câu trả lời có trích dẫn nguồn
- [ ] **Ngày 216 (T7)** — 🛠 Project: RAG v0 trên bộ tài liệu kỹ thuật
- [ ] **Ngày 217 (CN)** — 🔁 Ôn tuần · commit

## Tuần 2 — Tìm kiếm tốt hơn

- [ ] **Ngày 218 (T2)** — 📖 BM25 · ⭐ full-text search trong Postgres hoặc OpenSearch
- [ ] **Ngày 219 (T3)** — 💻 Hybrid search (BM25 + vector), gộp kết quả bằng RRF
- [ ] **Ngày 220 (T4)** — 💻 Reranking bằng cross-encoder
- [ ] **Ngày 221 (T5)** — 💻 Lọc theo metadata (loại máy, phiên bản tài liệu)
- [ ] **Ngày 222 (T6)** — 📖 Xử lý tiếng Việt: tách từ, embedding đa ngôn ngữ · 💻 So sánh 2–3 model embedding
- [ ] **Ngày 223 (T7)** — 🛠 Project: RAG v1 có hybrid search + rerank
- [ ] **Ngày 224 (CN)** — 🔁 Ôn tuần · note *"Vì sao chỉ vector search là chưa đủ"* · commit

## Tuần 3 — Evals

- [ ] **Ngày 225 (T2)** — 💻 Tự tạo bộ test 50–100 câu hỏi kèm đáp án và đoạn nguồn đúng
- [ ] **Ngày 226 (T3)** — 💻 Đo retrieval: recall@k, MRR
- [ ] **Ngày 227 (T4)** — 💻 Đo câu trả lời: độ bám nguồn (faithfulness), LLM-as-judge
- [ ] **Ngày 228 (T5)** — 💻 Script eval tự động, lưu kết quả theo phiên bản cấu hình
- [ ] **Ngày 229 (T6)** — ⭐ Tracing bằng Langfuse
- [ ] **Ngày 230 (T7)** — 🛠 Project: báo cáo so sánh các cấu hình (chunk, embedding, rerank) bằng số liệu
- [ ] **Ngày 231 (CN)** — 🔁 Ôn tuần · note *"Eval là gì và vì sao bắt buộc"* · commit

## Tuần 4 — Tài liệu thực tế và hoàn thiện

- [ ] **Ngày 232 (T2)** — ⭐ OCR cho tài liệu scan (PaddleOCR / Tesseract)
- [ ] **Ngày 233 (T3)** — 💻 Trích xuất bảng biểu trong PDF
- [ ] **Ngày 234 (T4)** — 💻 Cập nhật dữ liệu tăng dần (chỉ ingest tài liệu mới/đã sửa)
- [ ] **Ngày 235 (T5)** — 💻 Phân quyền tài liệu cơ bản theo người dùng
- [ ] **Ngày 236 (T6)** — 💻 Giao diện hỏi đáp, hiển thị đoạn nguồn
- [ ] **Ngày 237 (T7)** — 🛠 Project: RAG v2 hoàn chỉnh + eval suite + README có bảng số liệu
- [ ] **Ngày 238 (CN)** — 🔁 Ôn tháng · blog *"Làm RAG cho tài liệu kỹ thuật tiếng Việt"* · commit

## Dự phòng

- [ ] **Ngày 239** — Bù phần trễ / làm lại phần còn yếu
- [ ] **Ngày 240** — Bù phần trễ / tự kiểm tra mốc tháng

---

## ✅ Mốc cuối tháng

- [ ] Xây RAG có hybrid search, rerank, lọc metadata
- [ ] Có bộ eval tự động đo cả retrieval và câu trả lời
- [ ] Chứng minh mỗi cải tiến bằng số liệu
- [ ] Xử lý được tài liệu scan và bảng biểu
