# Tháng 05 — Object Detection, Segmentation, Tracking

> **Mục tiêu:** làm chủ detection, segmentation, tracking trên dữ liệu tự thu thập; dựng demo đếm đối tượng theo thời gian thực.
> **Bổ trợ:** video streaming (RTSP), WebSocket, PostgreSQL + SQLAlchemy.
> **Project:** **demo đếm bao hàng ra vào kho** (webcam/điện thoại + YOLO + ByteTrack + vạch ảo).
> **Tài liệu:** Ultralytics YOLO docs, Roboflow *supervision*, paper ByteTrack, SAM/SAM2, FastAPI WebSocket docs.

[⬅ Tháng 04](month-04.md) · [README](../README.md) · [Tháng 06 ➡](month-06.md)

---

## Tuần 1 — Object detection và dữ liệu riêng

- [ ] **Ngày 121 (T2)** — 📖 Bounding box, IoU, NMS, anchor vs anchor-free · 💻 Tự viết IoU và NMS
- [ ] **Ngày 122 (T3)** — 💻 Chạy YOLO pretrained trên ảnh và video
- [ ] **Ngày 123 (T4)** — 📖 mAP, mAP@50, mAP@50:95 · 💻 Tính mAP trên tập nhỏ bằng công cụ có sẵn và hiểu từng bước
- [ ] **Ngày 124 (T5)** — 💻 Quay video "người vác bao/túi" tại nhà ở nhiều góc, trích frame
- [ ] **Ngày 125 (T6)** — ⭐ Gán nhãn 300–500 ảnh (lớp: người, bao) trên Roboflow/CVAT
- [ ] **Ngày 126 (T7)** — 🛠 Project: fine-tune YOLO trên dữ liệu tự gán, ghi mAP
- [ ] **Ngày 127 (CN)** — 🔁 Ôn tuần · note *"Từ IoU đến mAP"* · commit

## Tuần 2 — Segmentation và tracking

- [ ] **Ngày 128 (T2)** — 📖 Semantic vs instance segmentation, U-Net
- [ ] **Ngày 129 (T3)** — 💻 Dùng SAM/SAM2 hỗ trợ gán nhãn nhanh
- [ ] **Ngày 130 (T4)** — 💻 YOLO segmentation trên dữ liệu riêng
- [ ] **Ngày 131 (T5)** — 📖 Tracking: Kalman filter, thuật toán Hungarian, SORT → ByteTrack
- [ ] **Ngày 132 (T6)** — 💻 Ghép YOLO + ByteTrack trên video, hiển thị ID
- [ ] **Ngày 133 (T7)** — 🛠 Project: tracking người và bao trên video tự quay
- [ ] **Ngày 134 (CN)** — 🔁 Ôn tuần · note *"Tracking hoạt động thế nào"* · commit

## Tuần 3 — Đếm qua vạch và chạy thời gian thực

- [ ] **Ngày 135 (T2)** — 💻 Logic đếm qua vạch ảo, phân biệt hướng ra/vào
- [ ] **Ngày 136 (T3)** — 💻 Xử lý trường hợp khó: quay đầu giữa chừng, che khuất, một người vác nhiều bao
- [ ] **Ngày 137 (T4)** — 💻 Script đánh giá: so số AI đếm với số đếm tay, tính sai số %
- [ ] **Ngày 138 (T5)** — ⭐ RTSP, đọc stream từ IP camera hoặc app camera điện thoại
- [ ] **Ngày 139 (T6)** — ⭐ FastAPI + WebSocket đẩy số đếm thời gian thực
- [ ] **Ngày 140 (T7)** — 🛠 Project: demo đếm bao realtime từ webcam/điện thoại
- [ ] **Ngày 141 (CN)** — 🔁 Ôn tuần · commit

## Tuần 4 — Cải thiện model, lưu dữ liệu, dashboard

- [ ] **Ngày 142 (T2)** — 📖 Pose estimation · 💻 YOLO-pose nhận biết người đang vác
- [ ] **Ngày 143 (T3)** — 💻 Thu thêm hard example (ca model sai), augmentation
- [ ] **Ngày 144 (T4)** — 💻 Train lại, so sánh mAP và sai số đếm trước/sau
- [ ] **Ngày 145 (T5)** — ⭐ PostgreSQL (Docker) + SQLAlchemy: lưu sự kiện đếm
- [ ] **Ngày 146 (T6)** — 💻 Dashboard đơn giản: số bao theo giờ/ca
- [ ] **Ngày 147 (T7)** — 🛠 Project: demo v1 hoàn chỉnh + video quay màn hình
- [ ] **Ngày 148 (CN)** — 🔁 Ôn tháng · blog *"Đếm bao hàng bằng YOLO + ByteTrack"* · commit

## Dự phòng

- [ ] **Ngày 149** — Bù phần trễ / làm lại phần còn yếu
- [ ] **Ngày 150** — Bù phần trễ / tự kiểm tra mốc tháng

---

## ✅ Mốc cuối tháng

- [ ] Tự viết IoU, NMS; giải thích được mAP
- [ ] Fine-tune YOLO trên dữ liệu tự thu thập và tự gán nhãn
- [ ] Ghép được detection + tracking + đếm qua vạch
- [ ] Đo được sai số đếm so với thực tế
- [ ] Demo chạy realtime, có lưu dữ liệu và dashboard
