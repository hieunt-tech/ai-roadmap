# Tháng 03 — Deep Learning từ gốc + PyTorch

> **Mục tiêu:** hiểu backprop đến tận gốc, tự viết autograd, thành thạo PyTorch và biết debug model.
> **Bổ trợ:** Docker.
> **Project:** CNN trên CIFAR-10 kèm báo cáo ablation, đóng gói bằng Docker.
> **Tài liệu:** Karpathy *Neural Networks: Zero to Hero*, 3Blue1Brown *Calculus* & *Neural Networks*, CS231n notes, PyTorch tutorials, Docker docs, Karpathy *A Recipe for Training Neural Networks*.

[⬅ Tháng 02](month-02.md) · [README](../README.md) · [Tháng 04 ➡](month-04.md)

---

## Tuần 1 — Giải tích, backprop, micrograd

- [ ] **Ngày 061 (T2)** — 📖 Đạo hàm riêng, gradient (3B1B / Khan Academy) · 💻 Tính gradient số bằng sai phân hữu hạn
- [ ] **Ngày 062 (T3)** — 📖 Chain rule, đồ thị tính toán · 💻 Karpathy micrograd phần 1
- [ ] **Ngày 063 (T4)** — 💻 micrograd phần 2: tự code lớp `Value` có backward
- [ ] **Ngày 064 (T5)** — 💻 Hoàn thiện micrograd: neuron, layer, MLP
- [ ] **Ngày 065 (T6)** — 📖 SGD, momentum, Adam (Distill *Why Momentum Really Works*) · 💻 Tự viết Adam
- [ ] **Ngày 066 (T7)** — 🛠 Project: train MLP micrograd trên dataset moons, vẽ decision boundary
- [ ] **Ngày 067 (CN)** — 🔁 Ôn tuần · tự suy ra backprop của một lớp linear trên giấy · commit

## Tuần 2 — PyTorch và makemore

- [ ] **Ngày 068 (T2)** — 📖 PyTorch tensor, autograd · 💻 Làm lại ví dụ micrograd bằng PyTorch
- [ ] **Ngày 069 (T3)** — 📖 `nn.Module`, `Dataset`, `DataLoader` · 💻 Viết Dataset tùy chỉnh
- [ ] **Ngày 070 (T4)** — 💻 Training loop tự viết: train/val, lưu checkpoint, early stopping
- [ ] **Ngày 071 (T5)** — 💻 Karpathy makemore phần 1–2 (bigram, MLP)
- [ ] **Ngày 072 (T6)** — 📖 Khởi tạo trọng số, BatchNorm (makemore phần 3) · 💻 Vẽ phân phối activation
- [ ] **Ngày 073 (T7)** — 🛠 Project: MLP trên MNIST bằng PyTorch, đạt trên 97%
- [ ] **Ngày 074 (CN)** — 🔁 Ôn tuần · note *"Vì sao cần BatchNorm"* · commit

## Tuần 3 — Docker, CNN, debug model

- [ ] **Ngày 075 (T2)** — ⭐ Docker: image, container, Dockerfile · 💻 Đóng gói script MNIST
- [ ] **Ngày 076 (T3)** — ⭐ Docker volume, network, docker compose · 💻 Compose app + Jupyter
- [ ] **Ngày 077 (T4)** — 📖 CNN: convolution, padding, stride, pooling (CS231n) · 💻 Tính kích thước output bằng tay rồi kiểm tra bằng code
- [ ] **Ngày 078 (T5)** — 💻 Viết CNN cho CIFAR-10 trong PyTorch
- [ ] **Ngày 079 (T6)** — 📖 *A Recipe for Training NN* · 💻 Overfit 1 batch, tìm learning rate, kiểm tra gradient
- [ ] **Ngày 080 (T7)** — 🛠 Project: train CNN CIFAR-10, theo dõi thí nghiệm bằng Weights & Biases
- [ ] **Ngày 081 (CN)** — 🔁 Ôn tuần · note *"Checklist debug model"* · commit

## Tuần 4 — Regularization, ResNet, ablation

- [ ] **Ngày 082 (T2)** — 📖 Dropout, weight decay, data augmentation · 💻 Thêm vào CNN, so kết quả
- [ ] **Ngày 083 (T3)** — 📖 Đọc lướt paper ResNet · 💻 Tự viết ResNet nhỏ
- [ ] **Ngày 084 (T4)** — 📖 Mixed precision, dùng GPU trên Colab/Kaggle · 💻 Train lại với AMP, so tốc độ
- [ ] **Ngày 085 (T5)** — ⭐ Chạy Docker với GPU (NVIDIA Container Toolkit) · 💻 Docker hóa script train
- [ ] **Ngày 086 (T6)** — 💻 Ablation: bỏ BatchNorm, đổi LR schedule, bỏ augmentation; ghi bảng kết quả
- [ ] **Ngày 087 (T7)** — 🛠 Project: báo cáo ablation + Docker image + README
- [ ] **Ngày 088 (CN)** — 🔁 Ôn tháng · blog tháng 3 · **tự kiểm tra mốc Quý 1** · commit

## Dự phòng

- [ ] **Ngày 089** — Bù phần trễ / làm lại phần còn yếu
- [ ] **Ngày 090** — Bù phần trễ / tự kiểm tra mốc tháng

---

## ✅ Mốc cuối tháng (và Quý 1)

- [ ] Tự suy ra backprop cho linear layer và softmax cross-entropy trên giấy
- [ ] Tự viết được autograd engine (micrograd)
- [ ] Viết training loop PyTorch không cần xem mẫu
- [ ] Debug được model không hội tụ (đọc loss curve, kiểm tra gradient)
- [ ] Đóng gói và chạy training bằng Docker
