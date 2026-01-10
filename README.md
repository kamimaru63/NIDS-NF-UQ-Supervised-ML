# Network Intrusion Detection using Supervised Machine Learning

## 1. Giới thiệu
Trong bối cảnh các hệ thống mạng ngày càng phức tạp, các cuộc tấn công mạng
(Intrusion/Anomaly) ngày càng đa dạng và khó phát hiện bằng các phương pháp
dựa trên luật (rule-based).  
Đề tài này tập trung xây dựng và so sánh các mô hình **Machine Learning học có giám sát**
nhằm phát hiện bất thường trong lưu lượng mạng, phục vụ cho hệ thống
**Network Intrusion Detection System (NIDS)**.

## 2. Mục tiêu đề tài
- Phân tích và hiểu bộ dữ liệu **NF-UQ-NIDS-v2**.
- Thực hiện **EDA (Exploratory Data Analysis)** và **Feature Engineering**.
- Huấn luyện các mô hình học có giám sát để phát hiện xâm nhập mạng.
- So sánh hiệu quả các mô hình dựa trên các chỉ số đánh giá.
- Xây dựng demo trực quan (dashboard) phục vụ review và bảo vệ đồ án.

## 3. Dataset
- **Tên dataset**: NF-UQ-NIDS-v2 Network Intrusion Detection Dataset  
- **Nguồn**: Kaggle  
- **Đặc điểm**:
  - Dữ liệu dạng bảng (tabular)
  - Có nhãn (label): Normal / Attack (và các loại tấn công)
  - Dataset mới hơn so với CICIDS2017
- **Mục đích sử dụng**:
  - Huấn luyện mô hình học có giám sát
  - Đánh giá khả năng phát hiện bất thường trong lưu lượng mạng

## 4. Phương pháp & Mô hình
### 4.1 Phương pháp
- Bài toán được tiếp cận như một bài toán **classification**.
- Sử dụng các mô hình **Supervised Learning**.
- So sánh các mô hình trên cùng một tập dữ liệu và cùng pipeline tiền xử lý.

### 4.2 Các mô hình dự kiến
- Random Forest
- Support Vector Machine (SVM)
- (Có thể mở rộng) Logistic Regression / XGBoost

## 5. Phương pháp đánh giá
Các mô hình được đánh giá dựa trên:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC Curve / AUC

## 6. Cấu trúc thư mục dự án

- NIDS-Supervised-ML/
  - data/
    - raw/ : Dataset gốc (NF-UQ-NIDS-v2)
    - processed/ : Dữ liệu đã tiền xử lý
  - notebooks/
    - 01_EDA.ipynb : Khám phá và phân tích dữ liệu
    - 02_Feature_Engineering.ipynb : Xây dựng và chọn đặc trưng
    - 03_Models.ipynb : Huấn luyện và so sánh mô hình
  - src/
    - preprocessing.py : Tiền xử lý dữ liệu
    - train.py : Huấn luyện mô hình
    - evaluate.py : Đánh giá mô hình
  - report/
    - outline.docx : Dàn ý báo cáo
    - literature_review.docx : Tổng quan nghiên cứu liên quan
  - slides/
    - review_slides.pptx : Slide review và bảo vệ
  - requirements.txt : Danh sách thư viện Python
  - README.md : Tài liệu mô tả dự án

## 7. Công nghệ sử dụng
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- Jupyter Notebook
- (Optional) Streamlit cho dashboard

## 8. Phân công nhóm
- **Huy**: Trưởng nhóm – Machine Learning & tổng hợp
- **Thảo**: Data Analyst – EDA, Feature Engineering
- **Hân**: Network & Dataset – Phân tích ATTT
- **Hiệp**: Visualization & Report

## 9. Tiến độ
Dự án được thực hiện trong 15 tuần, bao gồm các mốc:
- Review 1: Tuần 4
- Review 2: Tuần 8 (có demo)
- Review 3: Tuần 12 (demo + báo cáo)
- Bảo vệ: Tuần 15

## 10. Giảng viên hướng dẫn
- **ThS. Hồ Hải**

---
