# Giải Trình Kiến Trúc Dàn Trang (Layout Strategy)

CSS Grid được thiết kế cho bố cục hai chiều (2D - điều khiển cả hàng và cột đồng thời), lý tưởng để phân chia cấu trúc Dashboard Bento Box phức tạp mà không cần tạo các thẻ bao bọc (Div Soup) lộn xộn. 

Flexbox là công cụ một chiều (1D), tối ưu cho việc căn chỉnh các phần tử con tự động co giãn linh hoạt theo dung lượng nội dung thực tế (Content-first), thích hợp giải quyết vấn đề tràn chữ ở Thanh điều hướng (Navbar). 

Hệ thống Grid 12 cột của Bootstrap đóng vai trò tạo mẫu nhanh (Rapid Prototyping) cho các thành phần chuẩn hóa như Bảng giá (Pricing), giúp đảm bảo tính đồng bộ trên đa thiết bị nhờ hệ thống Breakpoint tích hợp sẵn mà không tốn công viết CSS thuần.