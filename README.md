# bigdata-pyspark-project

## 1. Giới thiệu

Dự án xây dựng hệ thống phân tích dữ liệu và Machine Learning trên bộ dữ liệu **Olist E-commerce** bằng PySpark.

Hệ thống bao gồm:

* Xử lý dữ liệu lớn (Big Data)
* Xây dựng pipeline bằng Spark ML
* Áp dụng nhiều nhóm thuật toán Machine Learning
* Hướng tới tích hợp Web UI bằng Streamlit

---

## 2. Mục tiêu

* Thực hiện EDA trên 9 bảng dữ liệu Olist
* Xây dựng master DataFrame
* Thiết kế pipeline xử lý dữ liệu (Spark ML)
* Triển khai các nhóm mô hình:

  * Clustering
  * Classification
  * Regression
  * Recommendation (ALS)
  * Association Rules (FP-Growth)
* Đánh giá mô hình bằng nhiều metrics
* Tích hợp hệ thống với Streamlit

---

## 3. Thành viên & phân công

### Nguyễn Ngọc Phương Trinh – Data Engineer

* Khảo sát & EDA dataset Olist
* Join 9 bảng → master DataFrame
* Xử lý missing values & Feature Engineering (RFM)
* Xây dựng Spark ML Pipeline
  (Indexer, OneHotEncoder, VectorAssembler, StandardScaler, ChiSqSelector)
* Clustering:

  * K-Means
  * Bisecting K-Means
  * Gaussian Mixture Model (GMM)

### Nguyễn Thị Yến Linh – Machine Learning Engineer

* Classification:

  * Logistic Regression
  * Random Forest
  * Naive Bayes
  * LinearSVC
  * GBTClassifier
* Regression:

  * Linear Regression
  * Decision Tree
  * Random Forest Regressor
* Hyperparameter tuning (CrossValidator)
* Đánh giá metrics:

  * Accuracy, F1-score
  * RMSE, MAE, R²

### Lê Nguyễn Thanh Huyền – Recommendation & Evaluation

* ALS Recommendation:

  * Xây dựng implicit feedback matrix
  * Train model
  * Evaluate RMSE (~1.9358)
* FP-Growth:

  * Frequent itemsets
  * Association rules
* Tổng hợp metrics & RankingMetrics


### Nguyễn Ngọc Minh Trang – Frontend & Visualization

* Thiết kế giao diện Streamlit
* Xây dựng dashboard với Plotly
* Các module:

  * Dashboard tổng quan
  * Phân khúc khách hàng
  * Gợi ý sản phẩm
  * Xu hướng mua sắm


### Đỗ Nguyễn Thanh Uyên – Documentation & Integration

* Tích hợp Spark model vào Streamlit (save/load pipeline)
* Quản lý GitHub repository & README
* Format báo cáo Word/PDF
* Xây dựng Gantt chart & theo dõi tiến độ
* Viết báo cáo:

  * Executive Summary
  * II, III, VII, VIII, IX, X, XI


## 4. Kiến trúc hệ thống

Pipeline tổng thể:

Data → Preprocessing → Feature Engineering → Model → Evaluation → Streamlit UI

---

## 5. Tiến độ dự án

* Tuần 1: **75%**
* Tuần 2 (tích luỹ): **~62%**

### Nhận xét:

* Phần Data & Pipeline gần hoàn thiện
* Các mô hình ML đang được mở rộng
* UI và Integration vẫn là trọng tâm của giai đoạn tiếp theo

---

## 6. Cấu trúc project

```id="x8k3lm"
data/           # Dữ liệu Olist
notebooks/      # EDA, Pipeline, ML models
app/            # Streamlit (đang phát triển)
report/         # Báo cáo
```

---

## 7. Công nghệ sử dụng

* Python
* PySpark
* Spark MLlib
* Streamlit
* Plotly
* GitHub

---

## 8. Hướng dẫn chạy

Hiện tại project chạy qua Notebook:

```bash id="g2p9wd"
jupyter notebook
```

(Phần Streamlit sẽ được cập nhật sau khi hoàn thiện tích hợp)

---

## 9. Khó khăn

* Tích hợp PySpark với Streamlit
* Đồng bộ pipeline giữa các thành viên
* Tuning model tốn thời gian

---

##  10. Hướng phát triển

* Hoàn thiện Classification & Regression
* Tích hợp end-to-end hệ thống
* Hoàn thiện Web UI
* Tối ưu hiệu năng

---

##  11. Ghi chú

Dự án đang trong quá trình hoàn thiện và sẽ tiếp tục được cập nhật trong Tuần 3.
