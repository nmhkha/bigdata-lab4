# Tóm tắt Dự án: Nhiệm vụ 3 — Tổng hợp dữ liệu (Aggregation)

Tài liệu này tóm tắt các nhiệm vụ đã thực hiện trong notebook `aggre.ipynb` như một phần của Nhiệm vụ 3 — Tổng hợp dữ liệu.

## Các công việc đã thực hiện

### 1. **Khám phá tập dữ liệu**
- Tải tập dữ liệu đã làm sạch từ tệp `data_cleaned.parquet` bằng thư viện `fastparquet`.
- Kiểm tra các bản ghi đầu tiên bằng lệnh `df.head()` để hiểu cấu trúc dữ liệu.
- Xác định các cột chính để phân tích: `category` (để nhóm) và `price` (để tính toán số liệu thống kê).

### 2. **Nhóm dữ liệu theo danh mục và tính toán số liệu thống kê**
- Thực hiện tổng hợp dữ liệu bằng hàm `groupby` trong thư viện `pandas`.
- Nhóm các bản ghi theo cột `category`.
- Tính toán các số liệu thống kê sau cho cột `price` trong mỗi danh mục:
  - **Trung bình (Mean)**: Giá trung bình của các mặt hàng.
  - **Tổng (Sum)**: Tổng giá trị của tất cả các mặt hàng.
  - **Số lượng (Count)**: Số lượng mặt hàng trong mỗi danh mục.

### 3. **Tạo biểu đồ trực quan hóa**
- Tạo các biểu đồ biểu diễn dữ liệu đã tổng hợp bằng thư viện `matplotlib`:
  - **Biểu đồ cột (Bar Chart)**: Hiển thị giá trung bình theo từng danh mục để so sánh các giá trị trung bình.
  - **Biểu đồ tròn (Pie Chart)**: Trực quan hóa sự phân bổ tổng giá trị giữa các danh mục để xem tỷ lệ đóng góp của mỗi loại.

---
*Ngày thực hiện: 13 tháng 4, 2026*