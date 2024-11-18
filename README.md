# Dự án Phê Duyệt Vay Tiền bằng Học Máy

## Giới thiệu
Dự án này tập trung vào việc nâng cao quá trình ra quyết định trong việc phê duyệt vay tiền, sử dụng các kỹ thuật học máy có khả năng giải thích. Bằng cách áp dụng các phương pháp học máy như Logistic Regression, Support Vector Machines, Decision Tree, Random Forest, và XGBoost, nghiên cứu này nhằm tạo ra một hệ thống quyết định vay tiền hiệu quả, minh bạch và đáng tin cậy trong bối cảnh kinh tế số.

## Mục tiêu
Mục tiêu của dự án là nâng cao tính minh bạch và hiệu quả trong quá trình phê duyệt vay tiền, đồng thời giảm thiểu các sai sót và thiên vị tiềm ẩn trong các quyết định tài chính.

## Phương pháp nghiên cứu
1. **Thu thập và tổng hợp dữ liệu**: Tập dữ liệu bao gồm các đặc điểm liên quan đến đơn xin vay tiền, với biến mục tiêu là phân loại trạng thái duyệt vay (đã duyệt hoặc bị từ chối).
2. **Phân tích và xử lý dữ liệu**: Dữ liệu được xử lý và mã hóa để phù hợp với mô hình học máy.
3. **Đánh giá kết quả**: Sử dụng các chỉ số Precision, Recall và F1-Score để đánh giá hiệu suất mô hình.
4. **Tinh chỉnh mô hình**: Sử dụng RandomizedSearchCV để tìm các tham số tối ưu cho mô hình học máy.

## Cấu trúc dự án
- **CHƯƠNG 1: TỔNG QUAN**: Giới thiệu về lý do chọn đề tài, mục tiêu nghiên cứu và phương pháp nghiên cứu.
- **CHƯƠNG 2: XỬ LÝ DỮ LIỆU**: Xác định bài toán, thu thập và tổng hợp dữ liệu, tiền xử lý dữ liệu.
- **CHƯƠNG 3: TRIỂN KHAI MÔ HÌNH**: Xây dựng và kiểm định mô hình học máy.
- **CHƯƠNG 4: ĐÁNH GIÁ**: Lựa chọn mô hình phù hợp và thực hiện đánh giá kết quả.
- **CHƯƠNG 5: THẢO LUẬN**: Ưu điểm, hạn chế và hướng phát triển trong tương lai.
- **CHƯƠNG 6: KẾT LUẬN**: Tổng kết kết quả nghiên cứu.

## Cài Đặt và Chạy Mô Hình

### Cài đặt các thư viện cần thiết
```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

## Các Bước Tiền Xử Lý Dữ Liệu
1. **Đọc dữ liệu** từ tập tin CSV.
2. **Chuyển đổi các cột phân loại** (như `default`, `housing`, `loan`) thành giá trị nhị phân (`0` hoặc `1`).
3. **Mã hóa các cột phân loại** khác (như `education`, `marital`, `job`) thành các giá trị số.
4. **Chia dữ liệu thành các tập huấn luyện và kiểm tra**, với tỷ lệ 80/20.
5. **Chuẩn hóa dữ liệu** sử dụng `MinMaxScaler` để đảm bảo tất cả các đặc trưng nằm trong phạm vi từ 0 đến 1.

## Đánh Giá và Tinh Chỉnh Mô Hình
- **Đánh giá mô hình** dựa trên các chỉ số Precision, Recall, và F1-Score.
- **Tinh chỉnh mô hình** sử dụng `RandomizedSearchCV` để tối ưu các tham số đầu vào cho mô hình.

## Thực Hiện Mô Hình
Sau khi huấn luyện mô hình, kết quả sẽ được đánh giá và phân tích để chọn mô hình tối ưu cho việc phê duyệt vay tiền.

## Tài Liệu Tham Khảo
1. [Sergio, 2020] - Nguồn dữ liệu cho bài toán phê duyệt vay tiền.
2. [Các nghiên cứu khác] - Các nghiên cứu về học máy trong lĩnh vực tài chính.
