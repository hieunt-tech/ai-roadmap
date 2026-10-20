# Tháng 10 — MLOps + CI/CD

> **Mục tiêu:** biến các project thành hệ thống có thể tái hiện, tự kiểm thử, tự deploy và tự train lại.
> **Bổ trợ:** GitHub Actions, container registry, Prefect/Airflow, Evidently.
> **Project:** pipeline MLOps hoàn chỉnh cho **hệ thống đếm bao** (CV) và **trợ lý kỹ thuật** (LLM).
> **Tài liệu:** Google *MLOps: Continuous delivery and automation pipelines*, MLflow docs, DVC pipelines, GitHub Actions docs, Evidently docs, Made With ML.

[⬅ Tháng 09](month-09.md) · [README](../README.md) · [Tháng 11 ➡](month-11.md)

---

## Tuần 1 — Theo dõi thí nghiệm và quản lý model

- [ ] **Ngày 271 (T2)** — 📖 Tổng quan MLOps, các mức độ trưởng thành (Google MLOps levels)
- [ ] **Ngày 272 (T3)** — 💻 MLflow tracking: log tham số, metric, artifact
- [ ] **Ngày 273 (T4)** — 💻 MLflow model registry: version, staging, production
- [ ] **Ngày 274 (T5)** — 💻 DVC pipeline (`dvc.yaml`): chuẩn bị dữ liệu → train → đánh giá
- [ ] **Ngày 275 (T6)** — 💻 Kiểm tra `dvc repro` tái hiện đúng kết quả
- [ ] **Ngày 276 (T7)** — 🛠 Project: đưa YOLO đếm bao vào MLflow + DVC
- [ ] **Ngày 277 (CN)** — 🔁 Ôn tuần · commit

## Tuần 2 — CI/CD

- [ ] **Ngày 278 (T2)** — ⭐ GitHub Actions: workflow, job, runner, secret
- [ ] **Ngày 279 (T3)** — ⭐ CI: lint (ruff), type-check (mypy), test (pytest) tự động
- [ ] **Ngày 280 (T4)** — ⭐ Build và push Docker image lên registry (GHCR)
- [ ] **Ngày 281 (T5)** — ⭐ CD: deploy tự động lên VPS khi merge vào main
- [ ] **Ngày 282 (T6)** — 💻 Kiểm tra model trong CI: chặn merge nếu mAP hoặc sai số đếm xấu đi
- [ ] **Ngày 283 (T7)** — 🛠 Project: CI/CD hoàn chỉnh cho repo đếm bao
- [ ] **Ngày 284 (CN)** — 🔁 Ôn tuần · note *"CI/CD cho model khác gì cho code"* · commit

## Tuần 3 — Giám sát và train lại

- [ ] **Ngày 285 (T2)** — 📖 Data drift, concept drift · 💻 Thử Evidently
- [ ] **Ngày 286 (T3)** — 💻 Giám sát dữ liệu ảnh đầu vào (độ sáng, phân phối lớp, độ tin cậy dự đoán)
- [ ] **Ngày 287 (T4)** — ⭐ Orchestration bằng Prefect (hoặc Airflow)
- [ ] **Ngày 288 (T5)** — 💻 Pipeline train lại tự động khi phát hiện drift
- [ ] **Ngày 289 (T6)** — 💻 Quản lý phiên bản prompt + chạy eval trong CI cho app LLM
- [ ] **Ngày 290 (T7)** — 🛠 Project: pipeline train lại + cổng eval trước khi lên production
- [ ] **Ngày 291 (CN)** — 🔁 Ôn tuần · commit

## Tuần 4 — Triển khai an toàn

- [ ] **Ngày 292 (T2)** — 📖 Feature store, khi nào cần
- [ ] **Ngày 293 (T3)** — 📖 A/B test, shadow deployment, canary release
- [ ] **Ngày 294 (T4)** — 💻 Rollback model về phiên bản trước
- [ ] **Ngày 295 (T5)** — 💻 Viết runbook vận hành (sự cố thường gặp và cách xử lý)
- [ ] **Ngày 296 (T6)** — 💻 Áp dụng MLOps cho trợ lý kỹ thuật (Langfuse + eval trong CI)
- [ ] **Ngày 297 (T7)** — 🛠 Project: MLOps hoàn chỉnh cho cả 2 hệ thống
- [ ] **Ngày 298 (CN)** — 🔁 Ôn tháng · blog tháng 10 · commit

## Dự phòng

- [ ] **Ngày 299** — Bù phần trễ / làm lại phần còn yếu
- [ ] **Ngày 300** — Bù phần trễ / tự kiểm tra mốc tháng

---

## ✅ Mốc cuối tháng

- [ ] Mọi thí nghiệm đều được log và tái hiện được
- [ ] CI/CD tự kiểm thử code lẫn chất lượng model
- [ ] Có giám sát drift và pipeline train lại
- [ ] Biết triển khai an toàn (shadow, canary, rollback)
