# House Price Prediction using Machine Learning

Dự án sử dụng các kỹ thuật **khai phá dữ liệu (Data Mining)** và **học
máy (Machine Learning)** để dự đoán giá nhà dựa trên các đặc trưng thực
tế như diện tích, số phòng, tiện nghi và vị trí.

Dữ liệu sử dụng: *Housing Prices Dataset -- Kaggle (M. Yasser H.)*
Mô hình triển khai: **Linear Regression, ANN, Random Forest, XGBoost**
Ngoài ra, dự án cũng ứng dụng **PCA** để giảm chiều dữ liệu và cải thiện
hiệu suất mô hình.

## Nội dung chính

### 1. Giới thiệu

-   Mục tiêu: xây dựng mô hình dự đoán giá nhà chính xác và có tính ứng
    dụng thực tế.
-   Phạm vi: xử lý dữ liệu, làm sạch, phân tích đặc trưng, mô hình hóa
    và đánh giá.
-   Ý nghĩa: hỗ trợ định giá bất động sản, phân tích đầu tư và tối ưu
    quyết định mua/bán.

### 2. Thu thập & Khám phá dữ liệu

**Tập dữ liệu gồm các thuộc tính chính:** - area -- diện tích
- bedrooms, bathrooms -- số phòng
- stories -- số tầng
- mainroad, guestroom, basement, airconditioning, prefarea -- tiện ích
- parking -- số chỗ đậu xe
- price -- biến mục tiêu

**Các bước xử lý dữ liệu:** - Kiểm tra & xử lý dữ liệu rỗng
- Phát hiện & loại bỏ dữ liệu không hợp lệ
- Kiểm tra trùng lặp
- Xử lý ngoại lai bằng IQR + Capping
- Chuẩn hóa dữ liệu
- Áp dụng PCA (92% variance -- còn 8 thành phần chính)

### 3. Mô hình học máy

#### 🔹 Linear Regression

-   Đơn giản, dễ diễn giải
-   So sánh kết quả trước & sau PCA
-   Có phân tích Ridge, Lasso và Feature Importance

#### 🔹 Artificial Neural Network (ANN)

-   Cấu trúc nhiều lớp
-   Học quan hệ phi tuyến
-   Trình bày forward/backpropagation, độ phức tạp thuật toán

#### 🔹 Random Forest

-   Ensemble mạnh mẽ, giảm overfitting
-   Dựa trên bootstrap + random feature selection
-   Hỗ trợ đánh giá Feature Importance

#### 🔹 XGBoost

-   Boosting mạnh mẽ
-   Regularization giảm overfitting
-   Tốc độ nhanh, hiệu quả cao

### 4. Đánh giá mô hình

Dự án sử dụng chỉ số: - RMSE
- R² Score

Kèm theo: - So sánh dữ liệu gốc & PCA
- Chọn mô hình tối ưu

### 5. Ứng dụng thực tế

Ứng dụng cho phép: - Nhập đặc trưng căn nhà
- Dự đoán giá
- Giao diện trực quan

### 6. Hạn chế & Hướng phát triển

**Hạn chế:** - Tập dữ liệu nhỏ
- Thiếu yếu tố địa lý thực
- Một số mô hình nhạy cảm phân phối lệch

**Hướng phát triển:** - Bổ sung dữ liệu vị trí
- Áp dụng LightGBM, CatBoost
- Deep Learning nâng cao
- Phát triển web (Flask/Django)

## Thành viên

-   Lý Tiểu Long -- 52200168
-   Lê Hồng Quang -- 52200156
-   Huỳnh Hoài Nam -- 52200151
-   Nguyễn Nhật Trường -- 52200192
-   Giản Hoàng Huy -- 52200147

## Giảng viên hướng dẫn: TS. Hoàng Anh
