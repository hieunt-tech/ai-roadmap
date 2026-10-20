# Tháng 02 — Xác suất, Thống kê + Machine Learning cổ điển

> **Mục tiêu:** hiểu xác suất và thống kê đủ để đọc paper và đánh giá model đúng cách; tự viết lại các thuật toán ML cơ bản.
> **Bổ trợ:** SQL, pandas, trực quan hóa.
> **Project:** phân tích bộ dữ liệu sản xuất bán dẫn **SECOM** (UCI) và dự đoán sản phẩm lỗi.
> **Tài liệu:** Harvard Stat 110, *An Introduction to Statistical Learning* (ISLR), CS229 lecture notes, SQLBolt, Mode SQL Tutorial.

[⬅ Tháng 01](month-01.md) · [README](../README.md) · [Tháng 03 ➡](month-03.md)

---

## Tuần 1 — Xác suất cơ bản, SQL, pandas

- [ ] **Ngày 031 (T2)** — 📖 Xác suất cơ bản, biến cố, xác suất có điều kiện (Stat 110 bài 1–3) · 💻 Mô phỏng Monte Carlo tung xúc xắc
- [ ] **Ngày 032 (T3)** — 📖 Phân phối Bernoulli, Binomial, Normal · 💻 Sinh mẫu và vẽ histogram bằng matplotlib
- [ ] **Ngày 033 (T4)** — 📖 Kỳ vọng, phương sai, định lý giới hạn trung tâm · 💻 Mô phỏng CLT
- [ ] **Ngày 034 (T5)** — ⭐ SQL cơ bản: SELECT, WHERE, GROUP BY (SQLBolt) · 💻 Bài tập trên SQLite
- [ ] **Ngày 035 (T6)** — ⭐ pandas: đọc CSV, lọc, groupby, merge · 💻 Bài tập trên một bộ CSV mẫu
- [ ] **Ngày 036 (T7)** — 🛠 Project: tải SECOM, khám phá dữ liệu (EDA), mô tả tỉ lệ lỗi
- [ ] **Ngày 037 (CN)** — 🔁 Ôn tuần · note *"Xác suất cho kỹ sư"* · commit

## Tuần 2 — MLE, lý thuyết thông tin, regression

- [ ] **Ngày 038 (T2)** — 📖 MLE và MAP · 💻 Tự ước lượng MLE cho phân phối Normal
- [ ] **Ngày 039 (T3)** — 📖 Entropy, cross-entropy, KL divergence · 💻 Tự tính và kiểm tra trên ví dụ
- [ ] **Ngày 040 (T4)** — ⭐ SQL: JOIN, subquery, CTE · 💻 Bài tập Mode SQL
- [ ] **Ngày 041 (T5)** — 📖 Linear regression (ISLR ch.3 / CS229) · 💻 Tự viết bằng normal equation và gradient descent
- [ ] **Ngày 042 (T6)** — 📖 Logistic regression · 💻 Tự viết bằng NumPy, so với sklearn
- [ ] **Ngày 043 (T7)** — 🛠 Project: làm sạch SECOM, xử lý missing value, chọn đặc trưng
- [ ] **Ngày 044 (CN)** — 🔁 Ôn tuần · note *"Vì sao cross-entropy = MLE"* · commit

## Tuần 3 — Regularization, metrics, cây quyết định

- [ ] **Ngày 045 (T2)** — 📖 Regularization L1/L2, bias–variance · 💻 Tự viết Ridge, vẽ learning curve
- [ ] **Ngày 046 (T3)** — 📖 Precision, recall, F1, ROC-AUC, dữ liệu mất cân bằng · 💻 Tự tính metric, so với sklearn
- [ ] **Ngày 047 (T4)** — 📖 Cross-validation, data leakage · 💻 Dựng sklearn Pipeline đúng cách
- [ ] **Ngày 048 (T5)** — 📖 Cây quyết định, Random Forest · 💻 Train và xem feature importance
- [ ] **Ngày 049 (T6)** — 📖 Gradient Boosting (XGBoost / LightGBM) · 💻 Train và tune cơ bản
- [ ] **Ngày 050 (T7)** — 🛠 Project: so sánh 3 model trên SECOM bằng cross-validation
- [ ] **Ngày 051 (CN)** — 🔁 Ôn tuần · note *"Chọn metric cho dữ liệu mất cân bằng"* · commit

## Tuần 4 — Thống kê thực nghiệm, unsupervised, báo cáo

- [ ] **Ngày 052 (T2)** — ⭐ SQL: window function, index, EXPLAIN · 💻 Bài tập tối ưu truy vấn
- [ ] **Ngày 053 (T3)** — 📖 Khoảng tin cậy, kiểm định giả thuyết, bootstrap · 💻 Bootstrap khoảng tin cậy cho F1
- [ ] **Ngày 054 (T4)** — 📖 k-means, PCA trong ứng dụng · 💻 Phân cụm dữ liệu SECOM sau PCA
- [ ] **Ngày 055 (T5)** — 📖 Phát hiện bất thường cơ bản (Isolation Forest) · 💻 Áp dụng lên SECOM
- [ ] **Ngày 056 (T6)** — ⭐ Trực quan hóa tốt với matplotlib/seaborn · 💻 Làm lại biểu đồ cho báo cáo
- [ ] **Ngày 057 (T7)** — 🛠 Project: báo cáo hoàn chỉnh (notebook + README), metric kèm khoảng tin cậy
- [ ] **Ngày 058 (CN)** — 🔁 Ôn tháng · viết blog tháng 2 · commit

## Dự phòng

- [ ] **Ngày 059** — Bù phần trễ / làm lại phần còn yếu
- [ ] **Ngày 060** — Bù phần trễ / tự kiểm tra mốc tháng

---

## ✅ Mốc cuối tháng

- [ ] Giải thích được MLE, entropy, KL divergence
- [ ] Tự viết được linear và logistic regression bằng NumPy
- [ ] Chọn đúng metric và tránh được data leakage
- [ ] Viết SQL có JOIN, CTE, window function
- [ ] Project SECOM có báo cáo, số liệu kèm khoảng tin cậy
