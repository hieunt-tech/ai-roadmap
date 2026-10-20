# 🚀 AI Engineer Roadmap — Computer Vision + LLM (365 ngày)

> Repo cá nhân để học và nghiên cứu mỗi ngày **2 tiếng**, mục tiêu sau **1 năm** đạt trình độ **Middle AI Engineer** theo hướng **Computer Vision + LLM**, gắn chặt với **ứng dụng thực tế** (AIoT, nhà máy thông minh, kho vận).

![Progress](https://img.shields.io/badge/Tiến_độ-0%2F360_ngày-blue)
![Focus](https://img.shields.io/badge/Hướng-CV_%2B_LLM-orange)
![Time](https://img.shields.io/badge/Thời_gian-2h%2Fngày-green)

---

## 🎯 Mục tiêu sau 12 tháng

- [ ] Nền toán và ML/DL vững: tự suy ra backprop, hiểu vì sao model chạy hoặc không chạy
- [ ] Xây được hệ thống **Computer Vision end-to-end** chạy trên thiết bị edge
- [ ] Xây được ứng dụng **LLM / RAG / Agent** có bộ eval tự động
- [ ] Kết hợp **CV + LLM** trong cùng một sản phẩm (multimodal)
- [ ] Vận hành được trên production: **MLOps, CI/CD, Docker, Kubernetes, Cloud, Monitoring**
- [ ] Portfolio gồm **3 project lớn** có số liệu đo thực tế, 12+ bài blog, ít nhất 1 PR open-source
- [ ] Trình bày được các lựa chọn kỹ thuật theo kiểu *"chọn X vì Y, đánh đổi Z"*

---

## 🗓️ Nhịp học mỗi tuần

| Ngày | Thời lượng | Nội dung |
| --- | --- | --- |
| Thứ 2 – Thứ 6 | 2h | 📖 45' lý thuyết + 💻 75' code |
| Thứ 7 | 2h | 🛠 Làm project của tháng |
| Chủ nhật | 2h | 🔁 Ôn tập, viết ghi chú/blog, commit (có thể nghỉ 1h) |

Mỗi tháng gồm **28 ngày học + 2 ngày dự phòng** để bù phần bị trễ.

**Ký hiệu:** 📖 Lý thuyết · 💻 Code · 🛠 Project · 🔁 Ôn tập · ⭐ Bổ trợ (DevOps, hạ tầng...)

---

## 📊 Tiến độ theo tháng

| # | Tháng | Chủ đề chính | Bổ trợ | Project | Xong |
| --- | --- | --- | --- | --- | --- |
| 1 | [Tháng 01](roadmap/month-01.md) | Python nâng cao + Đại số tuyến tính | Linux, Git | Công cụ xử lý ảnh bằng NumPy | ⬜ |
| 2 | [Tháng 02](roadmap/month-02.md) | Xác suất – Thống kê + ML cổ điển | SQL, pandas | Phân tích dữ liệu sản xuất (SECOM) | ⬜ |
| 3 | [Tháng 03](roadmap/month-03.md) | Deep Learning từ gốc + PyTorch | Docker | CNN CIFAR-10 + ablation | ⬜ |
| 4 | [Tháng 04](roadmap/month-04.md) | CV cổ điển + CNN + Transfer learning | Gán nhãn, DVC, FastAPI | Phát hiện lỗi sản phẩm (MVTec AD) | ⬜ |
| 5 | [Tháng 05](roadmap/month-05.md) | Detection, Segmentation, Tracking | Video stream, WebSocket, PostgreSQL | Demo đếm bao hàng ra vào kho | ⬜ |
| 6 | [Tháng 06](roadmap/month-06.md) | Edge AI + IoT | Mạng, MQTT, systemd, iOS | **Hệ thống đếm bao hoàn chỉnh** | ⬜ |
| 7 | [Tháng 07](roadmap/month-07.md) | Transformer + LLM nền tảng | Redis, async, deploy | Chatbot có tool calling | ⬜ |
| 8 | [Tháng 08](roadmap/month-08.md) | RAG + Evals | PostgreSQL/pgvector, search, OCR | RAG tài liệu kỹ thuật + eval suite | ⬜ |
| 9 | [Tháng 09](roadmap/month-09.md) | Multimodal (VLM) + Agents + Fine-tune | MCP, LangGraph | **Trợ lý kỹ thuật nhà máy (CV + LLM)** | ⬜ |
| 10 | [Tháng 10](roadmap/month-10.md) | MLOps | CI/CD, GitHub Actions, Prefect | Pipeline MLOps cho 2 hệ thống | ⬜ |
| 11 | [Tháng 11](roadmap/month-11.md) | Hạ tầng & vận hành | Kubernetes, Cloud, Terraform, Monitoring, Security | Hệ thống production-ready | ⬜ |
| 12 | [Tháng 12](roadmap/month-12.md) | ML System Design + Portfolio | Open-source, phỏng vấn | Design doc + portfolio hoàn chỉnh | ⬜ |

### 🏁 Mốc theo quý

- [ ] **Quý 1 – Nền tảng:** tự suy ra backprop trên giấy, train và debug được model bằng PyTorch
- [ ] **Quý 2 – Computer Vision:** một hệ thống CV chạy thật end-to-end (camera → edge → backend → app)
- [ ] **Quý 3 – LLM:** ứng dụng LLM có eval, kết hợp CV + LLM trong một sản phẩm
- [ ] **Quý 4 – Production:** hệ thống có CI/CD, monitoring, chạy trên cloud; portfolio sẵn sàng đi phỏng vấn

---

## 📁 Cấu trúc repo

```
ai-roadmap/
├── README.md              # File này — tổng quan & tiến độ
├── roadmap/               # Kế hoạch từng ngày, mỗi tháng một file
│   ├── month-01.md
│   └── ... month-12.md
├── notes/                 # Ghi chú lý thuyết (mỗi chủ đề một file)
├── projects/              # Code project từng tháng
├── templates/
│   └── weekly-review.md   # Mẫu tổng kết tuần
└── .gitignore
```

---

## ✅ Cách dùng repo này

1. **Mỗi ngày** mở file tháng hiện tại, làm xong thì đổi `- [ ]` thành `- [x]`.
2. **Commit mỗi ngày**, ví dụ:
   ```
   git commit -m "day 012: SVD + nén ảnh low-rank"
   ```
   Lịch sử commit chính là nhật ký học tập.
3. **Chủ nhật** copy `templates/weekly-review.md` vào `notes/` để tổng kết tuần.
4. **Cuối tháng** tick mốc tháng, đánh dấu ✅ trong bảng tiến độ ở trên, cập nhật badge tiến độ.
5. **Nếu bị trễ:** dùng 2 ngày dự phòng. Trễ nhiều thì **cắt bớt phần bổ trợ, không bỏ project**.

---

## 📌 Nguyên tắc

- **Build > xem khóa học.** Kiến thức chỉ "chắc" khi đã tự code lại.
- **Viết lại từ đầu trước, dùng thư viện sau.**
- **Mỗi tháng một project chạy được**, không bỏ dở.
- **Đo bằng số liệu:** độ chính xác, độ trễ, chi phí, sai số đếm.
- **Viết công khai:** mỗi tháng ít nhất 1 bài blog hoặc ghi chú chất lượng.
- **Áp dụng vào công việc thật** bất cứ khi nào có thể.

---

## 📚 Tài liệu chính

| Mảng | Tài liệu |
| --- | --- |
| Toán | 3Blue1Brown *Essence of Linear Algebra* & *Calculus*, MIT 18.06 (Gilbert Strang), Harvard Stat 110, *Mathematics for Machine Learning* |
| ML | Stanford CS229, *An Introduction to Statistical Learning* (ISLR) |
| Deep Learning | Karpathy *Neural Networks: Zero to Hero*, Stanford CS231n, d2l.ai |
| Computer Vision | OpenCV docs, Ultralytics YOLO docs, Roboflow *supervision*, anomalib |
| LLM | Karpathy *Let's build GPT*, Stanford CS224n, tài liệu API của các nhà cung cấp LLM |
| MLOps | Chip Huyen *Designing Machine Learning Systems*, MLflow docs, DVC docs, Made With ML |
| DevOps | *The Missing Semester* (MIT), Docker docs, kubernetes.io, Terraform tutorials |

---

## 📝 Nhật ký

| Tuần | Đã học | Khó khăn | Ghi chú |
| --- | --- | --- | --- |
| 1 | | | |
