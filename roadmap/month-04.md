# Tháng 04 — Computer Vision cổ điển + CNN + Transfer learning

> **Mục tiêu:** thành thạo OpenCV, transfer learning, và bài toán phát hiện lỗi sản phẩm trong công nghiệp.
> **Bổ trợ:** gán nhãn dữ liệu (CVAT/Roboflow), quản lý phiên bản dữ liệu (DVC), serve model bằng FastAPI.
> **Project:** hệ thống phát hiện lỗi sản phẩm trên **MVTec AD**, có API và giao diện demo.
> **Tài liệu:** OpenCV docs, timm, albumentations, anomalib, DVC docs, FastAPI docs.

[⬅ Tháng 03](month-03.md) · [README](../README.md) · [Tháng 05 ➡](month-05.md)

---

## Tuần 1 — OpenCV cổ điển

- [ ] **Ngày 091 (T2)** — 📖 Ảnh số, kênh màu, không gian màu · 💻 Đọc, hiển thị, chuyển sang HSV, tách màu
- [ ] **Ngày 092 (T3)** — 📖 Lọc ảnh, threshold, morphology · 💻 Làm sạch ảnh nhiễu
- [ ] **Ngày 093 (T4)** — 📖 Canny, contour · 💻 Đếm vật thể đơn giản bằng `findContours`
- [ ] **Ngày 094 (T5)** — 📖 Biến đổi hình học, perspective warp · 💻 Tự viết app "scan tài liệu"
- [ ] **Ngày 095 (T6)** — 💻 Đọc video/webcam, xử lý từng frame, đo FPS
- [ ] **Ngày 096 (T7)** — 🛠 Mini project: đếm đồng xu / ốc vít bằng OpenCV cổ điển
- [ ] **Ngày 097 (CN)** — 🔁 Ôn tuần · note *"Khi nào CV cổ điển là đủ"* · commit

## Tuần 2 — Transfer learning, dữ liệu, gán nhãn

- [ ] **Ngày 098 (T2)** — 📖 Kiến trúc CNN: VGG → ResNet → EfficientNet → ConvNeXt (đọc tóm tắt)
- [ ] **Ngày 099 (T3)** — 💻 Transfer learning bằng timm trên một dataset nhỏ
- [ ] **Ngày 100 (T4)** — 💻 Data augmentation bằng albumentations, so kết quả trước/sau
- [ ] **Ngày 101 (T5)** — ⭐ Cài CVAT (Docker) hoặc dùng Roboflow · 💻 Tự chụp và gán nhãn 100 ảnh
- [ ] **Ngày 102 (T6)** — ⭐ DVC: version dữ liệu, kết nối remote storage · 💻 Đưa dataset vào DVC
- [ ] **Ngày 103 (T7)** — 🛠 Project: tải MVTec AD, khám phá dữ liệu, chọn 2–3 loại sản phẩm
- [ ] **Ngày 104 (CN)** — 🔁 Ôn tuần · commit

## Tuần 3 — Phát hiện lỗi: có giám sát và không giám sát

- [ ] **Ngày 105 (T2)** — 📖 Đặc thù bài toán lỗi: ít ảnh lỗi, mất cân bằng, chi phí bỏ sót
- [ ] **Ngày 106 (T3)** — 💻 Fine-tune EfficientNet/ResNet phân loại OK/NG
- [ ] **Ngày 107 (T4)** — 📖 Grad-CAM · 💻 Hiển thị vùng model "nhìn vào"
- [ ] **Ngày 108 (T5)** — 📖 Đọc paper PatchCore (anomaly detection không giám sát)
- [ ] **Ngày 109 (T6)** — 💻 Chạy PatchCore bằng anomalib trên MVTec, xem heatmap lỗi
- [ ] **Ngày 110 (T7)** — 🛠 Project: so sánh supervised vs anomaly detection bằng số liệu
- [ ] **Ngày 111 (CN)** — 🔁 Ôn tuần · note *"Phát hiện lỗi khi gần như không có ảnh lỗi"* · commit

## Tuần 4 — Đánh giá theo chi phí, API, demo

- [ ] **Ngày 112 (T2)** — 📖 Confusion matrix, chọn ngưỡng theo chi phí sai · 💻 Vẽ đường precision–recall, chọn ngưỡng
- [ ] **Ngày 113 (T3)** — ⭐ FastAPI: endpoint upload ảnh → trả kết quả + heatmap
- [ ] **Ngày 114 (T4)** — ⭐ Docker hóa API
- [ ] **Ngày 115 (T5)** — 💻 Giao diện demo bằng Gradio/Streamlit
- [ ] **Ngày 116 (T6)** — 💻 Viết test cho API (pytest + httpx)
- [ ] **Ngày 117 (T7)** — 🛠 Project: hoàn thiện repo MVTec, README có bảng số liệu và ảnh demo
- [ ] **Ngày 118 (CN)** — 🔁 Ôn tháng · blog tháng 4 · commit

## Dự phòng

- [ ] **Ngày 119** — Bù phần trễ / làm lại phần còn yếu
- [ ] **Ngày 120** — Bù phần trễ / tự kiểm tra mốc tháng

---

## ✅ Mốc cuối tháng

- [ ] Xử lý ảnh/video bằng OpenCV không cần tra cứu nhiều
- [ ] Fine-tune được model phân loại ảnh trên dữ liệu riêng
- [ ] Hiểu và chạy được anomaly detection (PatchCore)
- [ ] Có API + Docker + giao diện demo cho model CV
- [ ] Quản lý dữ liệu bằng DVC
