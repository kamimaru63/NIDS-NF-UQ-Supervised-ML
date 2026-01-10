# Network Intrusion Detection using Supervised Machine Learning
## NF-UQ-NIDS-v2 Dataset

## 📌 Giới thiệu
Đề tài tập trung vào việc xây dựng và so sánh các mô hình Machine Learning **học có giám sát**
nhằm phát hiện bất thường và tấn công trong lưu lượng mạng.

Dataset sử dụng là **NF-UQ-NIDS-v2 Network Intrusion Detection Dataset**, một bộ dữ liệu mới,
phù hợp với các bài toán IDS hiện đại.

## 🎯 Mục tiêu
- Phân tích và tiền xử lý dữ liệu mạng
- Xây dựng các mô hình học có giám sát để phát hiện xâm nhập
- So sánh hiệu quả giữa các mô hình Machine Learning
- Đánh giá mô hình dưới góc độ An toàn Thông tin

## 🧠 Các mô hình dự kiến
- Random Forest
- Support Vector Machine (SVM)
- (Có thể mở rộng: XGBoost / Logistic Regression)

## 📊 Phương pháp đánh giá
- Accuracy
- Precision, Recall, F1-score
- ROC-AUC
- Confusion Matrix

## 🗂️ Cấu trúc thư mục
NIDS-Supervised-ML/
│
├── data/
│   ├── raw/                # Dataset gốc (NF-UQ-NIDS-v2)
│   └── processed/          # Dữ liệu đã tiền xử lý
│
├── notebooks/
│   ├── 01_EDA.ipynb
│   ├── 02_Feature_Engineering.ipynb
│   └── 03_Models.ipynb
│
├── src/
│   ├── preprocessing.py
│   ├── train.py
│   └── evaluate.py
│
├── report/
│   ├── outline.docx
│   └── literature_review.docx
│
├── slides/
│   └── review_slides.pptx
│
├── requirements.txt
└── README.md

## 👥 Thành viên nhóm
- **Huy** – Trưởng nhóm, Machine Learning
- **Thảo** – Data Analyst
- **Hân** – Network & Dataset
- **Hiệp** – Visualization & Report

## 👨‍🏫 Giảng viên hướng dẫn
- Thầy **Hồ Hải**

## 📅 Tiến độ
- Review 1: Tuần 4
- Review 2: Tuần 8
- Review 3: Tuần 12
- Bảo vệ: Tuần 15
