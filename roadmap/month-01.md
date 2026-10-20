# Tháng 01 — Python nâng cao + Đại số tuyến tính

> **Mục tiêu:** viết Python chuyên nghiệp hơn, hiểu ma trận như phép biến đổi, nắm vững SVD/PCA.
> **Bổ trợ:** Linux, Git nâng cao.
> **Project:** công cụ xử lý ảnh bằng NumPy thuần (lọc, convolution, nén ảnh bằng SVD).
> **Tài liệu:** 3Blue1Brown *Essence of Linear Algebra*, MIT 18.06, *The Missing Semester*, Learn Git Branching.

[⬅ README](../README.md) · [Tháng 02 ➡](month-02.md)

---

## Tuần 1 — Vector, ma trận, môi trường làm việc

- [ ] **Ngày 001 (T2)** — ⭐ Tạo repo này, cài Python (uv), VS Code, Jupyter · 📖 3B1B tập 1–2 (vector, tổ hợp tuyến tính) · 💻 NumPy array cơ bản
- [ ] **Ngày 002 (T3)** — 📖 3B1B tập 3–4 (phép biến đổi tuyến tính, nhân ma trận) · 💻 Tự viết nhân ma trận bằng vòng lặp, so tốc độ với NumPy
- [ ] **Ngày 003 (T4)** — ⭐ Linux: hệ thống file, quyền, pipe (*Missing Semester* bài 1–2) · 💻 Viết shell script tự tạo file ghi chú theo ngày
- [ ] **Ngày 004 (T5)** — 📖 3B1B tập 5–7 (định thức, ma trận nghịch đảo, hạng) · 💻 Giải hệ phương trình bằng `np.linalg.solve`, kiểm tra hạng
- [ ] **Ngày 005 (T6)** — 📖 Python typing, dataclass · 💻 Thêm type hints cho script, chạy `mypy`
- [ ] **Ngày 006 (T7)** — 🛠 Project: đọc ảnh thành mảng NumPy (Pillow), chuyển xám, lật, cắt bằng slicing
- [ ] **Ngày 007 (CN)** — 🔁 Ôn tuần · viết note *"Ma trận là phép biến đổi"* · commit

## Tuần 2 — Tích vô hướng, trị riêng, vector hóa

- [ ] **Ngày 008 (T2)** — 📖 3B1B tập 9 & 13 (tích vô hướng, đổi cơ sở) · 💻 Tính cosine similarity giữa các vector
- [ ] **Ngày 009 (T3)** — 📖 3B1B tập 14 (trị riêng, vector riêng) · 💻 Tự viết power iteration, so với `np.linalg.eig`
- [ ] **Ngày 010 (T4)** — 📖 Python generator, iterator, context manager · 💻 Generator đọc ảnh theo batch
- [ ] **Ngày 011 (T5)** — ⭐ Git: branch, rebase, merge conflict (Learn Git Branching) · 💻 Thực hành ngay trên repo này
- [ ] **Ngày 012 (T6)** — 📖 Broadcasting, vector hóa NumPy · 💻 Viết lại vòng lặp xử lý ảnh bằng broadcasting, đo tốc độ
- [ ] **Ngày 013 (T7)** — 🛠 Project: tự viết convolution 2D (blur, sharpen, phát hiện cạnh Sobel)
- [ ] **Ngày 014 (CN)** — 🔁 Ôn tuần · note *"Convolution hoạt động thế nào"* · commit

## Tuần 3 — SVD, bình phương tối thiểu, hiệu năng

- [ ] **Ngày 015 (T2)** — 📖 SVD trực giác (MIT 18.06 bài 29 hoặc Steve Brunton) · 💻 `np.linalg.svd` trên ma trận nhỏ, tự kiểm tra U·Σ·Vᵀ
- [ ] **Ngày 016 (T3)** — 📖 Phép chiếu và bình phương tối thiểu (18.06 bài 15–16) · 💻 Fit đường thẳng bằng least squares
- [ ] **Ngày 017 (T4)** — ⭐ Linux: process, biến môi trường, SSH, tmux · 💻 Chạy script nền trong tmux
- [ ] **Ngày 018 (T5)** — 📖 asyncio cơ bản · 💻 Tải nhiều ảnh song song bằng httpx
- [ ] **Ngày 019 (T6)** — 📖 Profiling (cProfile, line_profiler) · 💻 Profile hàm convolution và tối ưu
- [ ] **Ngày 020 (T7)** — 🛠 Project: nén ảnh bằng SVD low-rank, vẽ đồ thị chất lượng theo số rank
- [ ] **Ngày 021 (CN)** — 🔁 Ôn tuần · note *"SVD và nén ảnh"* · commit

## Tuần 4 — PCA, kiểm thử, đóng gói

- [ ] **Ngày 022 (T2)** — 📖 PCA = SVD trên dữ liệu đã chuẩn hóa · 💻 Tự viết PCA trên dataset digits, so với sklearn
- [ ] **Ngày 023 (T3)** — 📖 Ma trận hiệp phương sai, ma trận xác định dương · 💻 Tự tính covariance, so với `np.cov`
- [ ] **Ngày 024 (T4)** — 📖 pytest · 💻 Viết test cho các hàm xử lý ảnh
- [ ] **Ngày 025 (T5)** — ⭐ Đóng gói bằng `pyproject.toml`, CLI bằng Typer · 💻 Biến công cụ thành lệnh CLI
- [ ] **Ngày 026 (T6)** — 📖 Làm bài tập tổng hợp đại số tuyến tính (problem set 18.06)
- [ ] **Ngày 027 (T7)** — 🛠 Project: hoàn thiện công cụ, README, ảnh demo trước/sau
- [ ] **Ngày 028 (CN)** — 🔁 Ôn tháng · viết blog tháng 1 · commit

## Dự phòng

- [ ] **Ngày 029** — Bù phần trễ / làm lại phần còn yếu
- [ ] **Ngày 030** — Bù phần trễ / tự kiểm tra mốc tháng

---

## ✅ Mốc cuối tháng

- [ ] Giải thích được nhân ma trận, định thức, trị riêng bằng hình học
- [ ] Tự viết được SVD-based PCA và nén ảnh
- [ ] Dùng thành thạo Linux shell, SSH, tmux, Git branch/rebase
- [ ] Project có test, có CLI, có README
