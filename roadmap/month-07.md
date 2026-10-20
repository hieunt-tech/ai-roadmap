# Tháng 07 — Transformer + LLM nền tảng

> **Mục tiêu:** hiểu Transformer từ bên trong, dùng LLM API thành thạo (streaming, structured output, tool calling).
> **Bổ trợ:** Redis, async nâng cao, deploy lên cloud.
> **Project:** chatbot web có tool calling, streaming và cache, deploy lên cloud.
> **Tài liệu:** Karpathy *Let's build GPT* & *Let's build the GPT Tokenizer*, 3Blue1Brown chương Transformer, paper *Attention Is All You Need*, tài liệu API của các nhà cung cấp LLM, Ollama, Redis docs.

[⬅ Tháng 06](month-06.md) · [README](../README.md) · [Tháng 08 ➡](month-08.md)

---

## Tuần 1 — Xây GPT từ đầu

- [ ] **Ngày 181 (T2)** — 📖 Tokenization, BPE (Karpathy tokenizer) · 💻 Tự viết BPE đơn giản
- [ ] **Ngày 182 (T3)** — 📖 Cơ chế attention (3Blue1Brown) · 💻 Tự viết scaled dot-product attention
- [ ] **Ngày 183 (T4)** — 💻 Karpathy *Let's build GPT* phần 1
- [ ] **Ngày 184 (T5)** — 💻 *Let's build GPT* phần 2 (multi-head, residual, LayerNorm)
- [ ] **Ngày 185 (T6)** — 💻 Train GPT nhỏ trên văn bản tiếng Việt
- [ ] **Ngày 186 (T7)** — 🛠 Project: GPT nhỏ sinh văn bản tiếng Việt, ghi loss curve
- [ ] **Ngày 187 (CN)** — 🔁 Ôn tuần · note *"Attention giải thích bằng ví dụ"* · commit

## Tuần 2 — LLM hiện đại và API

- [ ] **Ngày 188 (T2)** — 📖 Đọc *Attention Is All You Need*
- [ ] **Ngày 189 (T3)** — 📖 LLM hiện đại: RoPE, KV cache, GQA, pretraining → SFT → RLHF/DPO
- [ ] **Ngày 190 (T4)** — 💻 LLM API: messages, system prompt, streaming
- [ ] **Ngày 191 (T5)** — 💻 Structured output (JSON schema) + kiểm tra bằng Pydantic
- [ ] **Ngày 192 (T6)** — 💻 Tool calling: tự định nghĩa tool, xử lý vòng gọi tool
- [ ] **Ngày 193 (T7)** — 🛠 Project: chatbot CLI có 2–3 tool (tính toán, tra cứu dữ liệu)
- [ ] **Ngày 194 (CN)** — 🔁 Ôn tuần · commit

## Tuần 3 — Prompting, model local, Redis

- [ ] **Ngày 195 (T2)** — 📖 Prompt engineering: few-shot, chia nhỏ tác vụ, xử lý output lỗi
- [ ] **Ngày 196 (T3)** — 💻 Chạy model local bằng Ollama, so chất lượng/tốc độ với API
- [ ] **Ngày 197 (T4)** — ⭐ Redis: cache, pub/sub, queue
- [ ] **Ngày 198 (T5)** — ⭐ FastAPI async + streaming SSE
- [ ] **Ngày 199 (T6)** — 💻 Cache câu trả lời bằng Redis, rate limit theo người dùng
- [ ] **Ngày 200 (T7)** — 🛠 Project: chatbot web (FastAPI + SSE + Redis)
- [ ] **Ngày 201 (CN)** — 🔁 Ôn tuần · note *"Thiết kế tool tốt cho LLM"* · commit

## Tuần 4 — Chi phí, độ bền, deploy

- [ ] **Ngày 202 (T2)** — 📖 Đếm token, tính chi phí, chọn model theo bài toán
- [ ] **Ngày 203 (T3)** — 💻 Retry, timeout, fallback sang model khác khi API lỗi
- [ ] **Ngày 204 (T4)** — 💻 Log hội thoại an toàn (ẩn dữ liệu nhạy cảm)
- [ ] **Ngày 205 (T5)** — ⭐ Deploy bằng Docker lên VPS hoặc dịch vụ cloud
- [ ] **Ngày 206 (T6)** — 💻 Viết test cho các tool và luồng hội thoại
- [ ] **Ngày 207 (T7)** — 🛠 Project: phát hành chatbot v1
- [ ] **Ngày 208 (CN)** — 🔁 Ôn tháng · blog tháng 7 · commit

## Dự phòng

- [ ] **Ngày 209** — Bù phần trễ / làm lại phần còn yếu
- [ ] **Ngày 210** — Bù phần trễ / tự kiểm tra mốc tháng

---

## ✅ Mốc cuối tháng

- [ ] Tự viết attention và một GPT nhỏ
- [ ] Giải thích được các bước huấn luyện LLM (pretrain, SFT, RLHF/DPO)
- [ ] Dùng thành thạo streaming, structured output, tool calling
- [ ] Ứng dụng LLM có cache, rate limit, fallback, đã deploy
