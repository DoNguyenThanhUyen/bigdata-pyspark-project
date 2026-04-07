# 🛒 Hệ Thống Phân Tích Hành Vi Khách Hàng & Khuyến Nghị Thông Minh

Hệ thống phân tích dữ liệu lớn (**End-to-End**) sử dụng **Apache Spark MLlib** để xử lý, phân loại, phân cụm khách hàng và đưa ra các khuyến nghị sản phẩm dựa trên tập dữ liệu Olist (~100.000 đơn hàng).

---

## 👥 Thành viên thực hiện (Nhóm 05)

| MSSV | Họ và Tên | Vai trò chính |
| :--- | :--- | :--- |
| **23126046** | **Nguyễn Ngọc Phương Trinh** | **Nhóm trưởng - Data Engineer** |
| 23126014 | Lê Nguyễn Thanh Huyền | Recommendation & Evaluation |
| 23126024 | Nguyễn Thị Yến Linh | Machine Learning Engineer |
| 23126041 | Nguyễn Ngọc Minh Trang | Frontend & Visualization |
| 23126053 | Đỗ Nguyễn Thanh Uyên | Documentation & Integration |

**Giảng viên hướng dẫn:** Thầy Hồ Nhựt Minh

---

## 🚀 Tổng quan đồ án
Đồ án tập trung vào việc giải quyết bài toán Big Data trong thương mại điện tử tại thị trường Brazil, bao gồm:
* **Tiền xử lý & Feature Engineering:** Xây dựng Spark ML Pipeline, phân tích RFM, TF-IDF.
* **Mô hình hóa:** Triển khai 13 thuật toán thuộc 5 nhóm bài toán Machine Learning.
* **Ứng dụng:** Dashboard trực quan hóa và dự đoán trực tuyến trên nền tảng Streamlit.

---

## 📂 Cấu trúc mã nguồn
Dự án được tổ chức thành các phân phần tương ứng với các giai đoạn phân tích:
* `(1) Classification/`: Dự đoán khả năng khách hàng rời bỏ (Churn) hoặc phân loại đơn hàng.
* `(2) Regression/`: Dự báo giá trị thanh toán và thời gian giao hàng.
* `(3) Clustering/`: Phân khúc khách hàng dựa trên chỉ số RFM (K-Means, GMM).
* `(4) Recommendation/`: Hệ thống gợi ý sản phẩm sử dụng thuật toán ALS.
* `(5) FP-Growth/`: Khai phá luật kết hợp từ giỏ hàng.
* `Streamlit/`: Mã nguồn giao diện người dùng Web Dashboard.

---

## 📁 Lưu trữ Mô hình (Model Storage)
Do hạn chế về dung lượng của GitHub, các mô hình đã huấn luyện hoàn chỉnh được lưu trữ tại Google Drive.

* 🔗 **Link tải Model tổng hợp:** [Click để tải về từ Google Drive](https://drive.google.com/drive/folders/1nBK4xVgsCsQteYD4_pbG0Enaiz9r65Kz)

---

## 🛠 Công nghệ sử dụng
* **Ngôn ngữ:** Python 3.12.13
* **Xử lý dữ liệu lớn:** PySpark 3.5.1 (MLlib)
* **Giao diện:** Streamlit
* **Trực quan hóa:** Plotly, Seaborn, Matplotlib

---

## 📊 Kết quả đạt được
* **Pipeline:** Tự động hóa quy trình từ dữ liệu thô (9 file CSV) đến đặc trưng vector.
* **Hiệu năng:** GBTClassifier đạt độ chính xác cao nhất trong nhóm phân loại; K-Means tối ưu hóa phân cụm với K=4.
