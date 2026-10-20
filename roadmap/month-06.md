# Tháng 06 — Edge AI + IoT

> **Mục tiêu:** đưa model CV chạy nhanh trên thiết bị edge và kết nối thành hệ thống IoT hoàn chỉnh.
> **Bổ trợ:** mạng cơ bản, MQTT, systemd, app iOS (SwiftUI).
> **Project:** **hệ thống đếm bao hoàn chỉnh**: camera → edge → MQTT → backend → dashboard → cảnh báo trên iOS.
> **Tài liệu:** ONNX Runtime docs, TensorRT / OpenVINO docs, Eclipse Mosquitto docs, NVIDIA DeepStream docs.

[⬅ Tháng 05](month-05.md) · [README](../README.md) · [Tháng 07 ➡](month-07.md)

---

## Tuần 1 — Tối ưu model cho edge

- [ ] **Ngày 151 (T2)** — 📖 ONNX · 💻 Export YOLO sang ONNX, chạy bằng onnxruntime, đo latency
- [ ] **Ngày 152 (T3)** — 📖 Quantization: FP16, INT8, post-training quantization
- [ ] **Ngày 153 (T4)** — 💻 TensorRT (nếu có GPU NVIDIA/Jetson) hoặc OpenVINO trên CPU
- [ ] **Ngày 154 (T5)** — 💻 Benchmark: FPS và mAP ở từng mức tối ưu, lập bảng đánh đổi
- [ ] **Ngày 155 (T6)** — ⭐ Mạng cơ bản: IP, port, TCP/UDP, RTSP, NAT
- [ ] **Ngày 156 (T7)** — 🛠 Project: chạy model đã tối ưu trên thiết bị edge (Jetson / Raspberry Pi / laptop CPU)
- [ ] **Ngày 157 (CN)** — 🔁 Ôn tuần · note *"Đánh đổi tốc độ và độ chính xác"* · commit

## Tuần 2 — MQTT và luồng dữ liệu

- [ ] **Ngày 158 (T2)** — ⭐ MQTT: broker Mosquitto chạy bằng Docker, publish/subscribe
- [ ] **Ngày 159 (T3)** — 📖 Thiết kế message sự kiện (JSON schema), QoS, retain
- [ ] **Ngày 160 (T4)** — 💻 Edge app publish sự kiện đếm qua MQTT
- [ ] **Ngày 161 (T5)** — 💻 Backend subscribe MQTT → lưu PostgreSQL
- [ ] **Ngày 162 (T6)** — ⭐ systemd: chạy edge app thành service, tự khởi động lại khi lỗi
- [ ] **Ngày 163 (T7)** — 🛠 Project: luồng edge → MQTT → backend → DB chạy ổn định
- [ ] **Ngày 164 (CN)** — 🔁 Ôn tuần · commit

## Tuần 3 — Độ bền hệ thống, quyền riêng tư, iOS

- [ ] **Ngày 165 (T2)** — 📖 GStreamer cơ bản, đọc giới thiệu DeepStream
- [ ] **Ngày 166 (T3)** — 💻 Xử lý nhiều camera bằng multiprocessing
- [ ] **Ngày 167 (T4)** — 💻 Lưu ảnh/clip ngắn khi có sự kiện bất thường, làm mờ khuôn mặt
- [ ] **Ngày 168 (T5)** — 💻 Logging, xử lý mất kết nối camera, retry
- [ ] **Ngày 169 (T6)** — ⭐ iOS: app SwiftUI nhận số đếm realtime và push cảnh báo
- [ ] **Ngày 170 (T7)** — 🛠 Project: tích hợp app iOS vào hệ thống
- [ ] **Ngày 171 (CN)** — 🔁 Ôn tuần · note *"Thiết kế camera AI tôn trọng quyền riêng tư"* · commit

## Tuần 4 — Hoàn thiện và phát hành

- [ ] **Ngày 172 (T2)** — 💻 Giả lập phiếu xuất kho, logic cảnh báo khi số đếm lệch
- [ ] **Ngày 173 (T3)** — ⭐ docker compose cho toàn bộ hệ thống
- [ ] **Ngày 174 (T4)** — 💻 Chạy liên tục 24h, ghi lỗi và sửa
- [ ] **Ngày 175 (T5)** — 💻 Tài liệu kiến trúc + sơ đồ hệ thống
- [ ] **Ngày 176 (T6)** — 💻 Quay video demo
- [ ] **Ngày 177 (T7)** — 🛠 Project: phát hành **v1 hệ thống đếm bao** (repo riêng)
- [ ] **Ngày 178 (CN)** — 🔁 Ôn tháng · blog · **tự kiểm tra mốc Quý 2** · commit

## Dự phòng

- [ ] **Ngày 179** — Bù phần trễ / làm lại phần còn yếu
- [ ] **Ngày 180** — Bù phần trễ / tự kiểm tra mốc tháng

---

## ✅ Mốc cuối tháng (và Quý 2)

- [ ] Export và tối ưu model (ONNX, FP16/INT8), có bảng benchmark
- [ ] Hệ thống IoT chạy ổn định: edge → MQTT → backend → DB
- [ ] App iOS nhận dữ liệu và cảnh báo
- [ ] Chạy liên tục 24h không sập
- [ ] Repo có tài liệu kiến trúc, số liệu, video demo
