# Nhật Ký Tương Tác AI (AI Prompt Log)

### Prompt 1: Tra cứu CSS Grid Span & Aspect Ratio
* **User Prompt:** "Khi tôi muốn tạo bố cục 1 ảnh to chiếm 2 hàng bên trái và 2 ảnh nhỏ xếp chồng bên phải bằng CSS Grid, cú pháp grid-row và grid-column chuẩn là gì để không phải fix cứng chiều cao pixel?"
* **Ứng dụng:** Thiết lập `.photo-main { grid-column: 1 / 2; grid-row: 1 / span 2; }` kết hợp `object-fit: cover`.

### Prompt 2: Tối ưu Bootstrap Utility Classes cho Flexbox
* **User Prompt:** "Trong Bootstrap 5, làm thế nào để căn giữa theo chiều dọc Avatar, Tên tác giả và Nút Share trên cùng 1 hàng, tự động rớt dòng khi quá hẹp mà không dùng CSS thuần?"
* **Ứng dụng:** Áp dụng chuỗi class `d-flex justify-content-between align-items-center flex-wrap gap-3` vào `.author-section`.

### Prompt 3: Cấu trúc Grid Responsive cho Bài viết liên quan
* **User Prompt:** "Cú pháp lớp Grid của Bootstrap 5 để hiển thị 4 cột trên Desktop (>=992px), 2 cột trên Tablet (>=768px) và 1 cột trên Mobile là gì?"
* **Ứng dụng:** Sử dụng `col-12 col-md-6 col-lg-3` cho danh sách thẻ bài viết đề xuất.