# Network Intrusion Detection using Supervised Machine Learning

## 1. Giới thiệu
Trong bối cảnh các hệ thống mạng ngày càng phức tạp, các cuộc tấn công mạng
(Intrusion/Anomaly) ngày càng đa dạng và khó phát hiện bằng các phương pháp
dựa trên luật (rule-based).  
Đề tài này tập trung xây dựng và so sánh các mô hình **Machine Learning học có giám sát**
nhằm phát hiện xâm nhập trong lưu lượng mạng dựa trên **NetFlow temporal features**, phục vụ cho hệ thống  
**Network Intrusion Detection System (NIDS)**.

---

## 2. Mục tiêu đề tài
- Phân tích và hiểu bộ dữ liệu **NF-UNSW-NB15-v3 (NetFlow V3)**.
- Thực hiện **EDA và phân tích hành vi lưu lượng mạng theo thời gian**.
- Xây dựng mô hình **phân loại lưu lượng bình thường và tấn công**.
- So sánh các mô hình học có giám sát.
- Xây dựng dashboard demo hỗ trợ đánh giá hệ thống NIDS.

---

## 3. Dataset

- **Tên dataset**: **NF-UNSW-NB15-v3 – NetFlow V3 Dataset**  
- **Nguồn**: University of Queensland (RA5 Benchmark)  
  https://staff.itee.uq.edu.au/marius/NIDS_datasets/  
- **Paper tham chiếu**:  
  *Luay et al., “Temporal Analysis of NetFlow Datasets for Network Intrusion Detection Systems”, arXiv 2025*

### Đặc điểm
- Dữ liệu dạng **NetFlow**
- **53 features** (43 NetFlow + 10 temporal features)
- **2.36 triệu flows**
- **9 loại tấn công + Benign**
- Phân bố lưu lượng **theo thời gian thực tế**

### Mục đích sử dụng
- Phát hiện xâm nhập & bất thường trong lưu lượng mạng
- Mô phỏng hệ thống **Network Intrusion Detection System (NIDS)** trong môi trường thật

---

## 4. Phương pháp & Mô hình

### 4.1 Phương pháp
- Bài toán được tiếp cận như một bài toán **classification** (binary và multi-class).
- Dữ liệu được xử lý theo **flow-based learning**.
- Các **temporal features** được giữ lại để mô hình học được hành vi mạng theo thời gian.

### 4.2 Các mô hình
- Random Forest  
- XGBoost  
- Support Vector Machine (SVM)  
- Logistic Regression  

---

## 5. Phương pháp đánh giá
Các mô hình được đánh giá dựa trên:
- Accuracy  
- Precision  
- Recall  
- F1-score  
- Confusion Matrix  
- ROC Curve / AUC  
- Detection rate theo từng loại tấn công  

---

## 6. Cấu trúc thư mục dự án
NIDS-Supervised-ML/
│
├── data/
│ ├── raw/ # Dataset gốc (NF-UNSW-NB15-v3)
│ └── processed/ # Dữ liệu đã tiền xử lý
│
├── notebooks/
│ ├── 01_EDA.ipynb
│ ├── 02_Feature_Engineering.ipynb
│ └── 03_Models.ipynb
│
├── src/
│ ├── preprocessing.py
│ ├── train.py
│ └── evaluate.py
│
├── report/
│ ├── outline.docx
│ └── literature_review.docx
│
├── slides/
│ └── review_slides.pptx
│
├── requirements.txt
└── README.md


---

## 7. Công nghệ sử dụng
- Python  
- Pandas, NumPy  
- Scikit-learn  
- Matplotlib, Seaborn  
- Jupyter Notebook  
- Streamlit (dashboard)  

---

## 8. Phân công nhóm
- **Huy**: Trưởng nhóm – Machine Learning & tổng hợp  
- **Thảo**: Data Analyst – EDA, Feature Engineering  
- **Hân**: Network & Dataset – Phân tích ATTT  
- **Hiệp**: Visualization & Report  

---

## 9. Tiến độ
- Review 1: Tuần 4  
- Review 2: Tuần 8 (demo)  
- Review 3: Tuần 12 (demo + báo cáo)  
- Bảo vệ: Tuần 15  

---

## 10. Giảng viên hướng dẫn
- **ThS. Hồ Hải**

