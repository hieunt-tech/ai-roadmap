# Tháng 11 — Hạ tầng & Vận hành

> **Mục tiêu:** chạy hệ thống AI trên Kubernetes và cloud, có monitoring, bảo mật, và chịu được tải.
> **Bổ trợ:** Kubernetes, Helm, AWS hoặc GCP, Terraform, Prometheus/Grafana/Loki, vLLM, load testing.
> **Project:** hệ thống **production-ready** trên cloud kèm báo cáo load test.
> **Tài liệu:** kubernetes.io tutorials, Helm docs, Terraform tutorials, Prometheus & Grafana docs, vLLM docs, OWASP Top 10 for LLM Applications, k6/Locust docs.

[⬅ Tháng 10](month-10.md) · [README](../README.md) · [Tháng 12 ➡](month-12.md)

---

## Tuần 1 — Kubernetes

- [ ] **Ngày 301 (T2)** — 📖 Khái niệm Kubernetes: pod, deployment, service, ingress
- [ ] **Ngày 302 (T3)** — ⭐ Dựng cluster local bằng kind hoặc minikube
- [ ] **Ngày 303 (T4)** — 💻 Deploy API lên k8s, dùng ConfigMap và Secret
- [ ] **Ngày 304 (T5)** — 💻 Autoscaling bằng HPA
- [ ] **Ngày 305 (T6)** — ⭐ Helm: viết chart cho ứng dụng
- [ ] **Ngày 306 (T7)** — 🛠 Project: backend đếm bao chạy trên k8s local
- [ ] **Ngày 307 (CN)** — 🔁 Ôn tuần · note *"Kubernetes cho người làm AI"* · commit

## Tuần 2 — Cloud và Infrastructure as Code

- [ ] **Ngày 308 (T2)** — ⭐ Chọn AWS hoặc GCP: IAM, **bật cảnh báo chi phí ngay từ đầu**
- [ ] **Ngày 309 (T3)** — ⭐ Compute (EC2/GCE), storage (S3/GCS)
- [ ] **Ngày 310 (T4)** — ⭐ Dịch vụ container (ECS / Cloud Run) hoặc managed k8s (EKS/GKE)
- [ ] **Ngày 311 (T5)** — ⭐ Terraform cơ bản: provider, resource, state
- [ ] **Ngày 312 (T6)** — 💻 Viết Terraform tạo hạ tầng cho project
- [ ] **Ngày 313 (T7)** — 🛠 Project: deploy lên cloud bằng Terraform (**nhớ `terraform destroy` khi xong**)
- [ ] **Ngày 314 (CN)** — 🔁 Ôn tuần · commit

## Tuần 3 — Observability và serving LLM

- [ ] **Ngày 315 (T2)** — ⭐ Prometheus: expose metric từ FastAPI (latency, số request, lỗi)
- [ ] **Ngày 316 (T3)** — ⭐ Grafana dashboard + cảnh báo
- [ ] **Ngày 317 (T4)** — ⭐ Log tập trung bằng Loki
- [ ] **Ngày 318 (T5)** — 📖 Serving LLM: batching, throughput, vLLM
- [ ] **Ngày 319 (T6)** — 💻 Benchmark vLLM vs Ollama trên cùng model
- [ ] **Ngày 320 (T7)** — 🛠 Project: monitoring đầy đủ cho trợ lý kỹ thuật
- [ ] **Ngày 321 (CN)** — 🔁 Ôn tuần · note *"Cần giám sát gì cho một hệ thống AI"* · commit

## Tuần 4 — Bảo mật, chi phí, chịu tải

- [ ] **Ngày 322 (T2)** — ⭐ Quản lý secret, HTTPS, xác thực (JWT/OAuth)
- [ ] **Ngày 323 (T3)** — 📖 OWASP Top 10 cho ứng dụng LLM · 💻 Rà soát hệ thống theo danh sách
- [ ] **Ngày 324 (T4)** — 📖 Tối ưu chi phí GPU: scale về 0, spot instance, chọn model nhỏ hơn
- [ ] **Ngày 325 (T5)** — 💻 Load test bằng k6 hoặc Locust
- [ ] **Ngày 326 (T6)** — 💻 Tối ưu dựa trên kết quả load test, đo lại
- [ ] **Ngày 327 (T7)** — 🛠 Project: hệ thống production-ready + báo cáo load test
- [ ] **Ngày 328 (CN)** — 🔁 Ôn tháng · blog tháng 11 · commit

## Dự phòng

- [ ] **Ngày 329** — Bù phần trễ / làm lại phần còn yếu
- [ ] **Ngày 330** — Bù phần trễ / tự kiểm tra mốc tháng

---

## ✅ Mốc cuối tháng

- [ ] Deploy được ứng dụng lên Kubernetes bằng Helm
- [ ] Tạo hạ tầng cloud bằng Terraform, kiểm soát được chi phí
- [ ] Có dashboard, cảnh báo, log tập trung
- [ ] Rà soát bảo mật theo OWASP LLM Top 10
- [ ] Có số liệu load test và biết hệ thống chịu được bao nhiêu
