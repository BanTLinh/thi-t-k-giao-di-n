# Nhật Ký Tương Tác AI (AI Prompt Log)

### Prompt 1: Phân tích 1D vs 2D
* **User Prompt:** "Khi tôi cần một bố cục mà một phần tử con (Child) phải chiếm chính xác 2 hàng và 2 cột (span 2 rows, 2 columns) đan xen với các phần tử nhỏ khác, tôi nên chọn CSS Grid hay Flexbox? Tại sao Flexbox lại chật vật với yêu cầu này?"
* **Mục đích:** Thẩm định tư duy kiến trúc giữa Grid và Flexbox.
* **Kết quả ứng dụng:** Xác định Bento Box Dashboard phải dùng `display: grid` kết hợp `grid-column: span 2` và `grid-row: span 2`, loại bỏ toàn bộ cấu trúc chia cột `.column` thừa trong mã cũ.

### Prompt 2: Tra cứu Bootstrap Breakpoints
* **User Prompt:** "Trong Bootstrap 5, sự khác biệt giữa lớp col-sm-4 và col-md-4 là gì? Tại sao tôi nên dùng Bootstrap thay vì tự viết CSS Grid cho một phần tử đơn giản như 3 cột Bảng giá?"
* **Mục đích:** Lựa chọn giải pháp Responsive tối ưu tốc độ triển khai cho phần Pricing.
* **Kết quả ứng dụng:** Sử dụng `col-12 col-md-4` cho Pricing Cards để đảm bảo tự động chuyển thành 1 cột trên Mobile (<768px) và 3 cột trên Desktop/Tablet.

### Prompt 3: Tối ưu khoảng cách bằng gap
* **User Prompt:** "Thuộc tính `gap` hoạt động như thế nào trong cả Flexbox và CSS Grid? Làm thế nào để dùng `gap` thay thế cho margin/padding lộn xộn giữa các phần tử con?"
* **Mục đích:** Làm sạch mã CSS, loại bỏ các kỹ thuật `margin-right` / `float` lỗi thời.
* **Kết quả ứng dụng:** Áp dụng `gap: 15px` cho cả `.navbar-flex` và `.bento-grid`.