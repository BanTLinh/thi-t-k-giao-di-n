# Báo Cáo Tái Cấu Trúc Bố Cục (Layout Refactoring Report)

Sử dụng `position: absolute` cho mục đích chia bố cục chính là sai lầm nguy hiểm trong Responsive Design. Thuộc tính này tách phần tử hoàn toàn khỏi dòng chảy tự nhiên của DOM (Normal Document Flow), khiến phần tử cha mất chiều cao thực tế (Collapse height = 0px). Khi màn hình thu nhỏ, các phần tử nằm dưới không thể tự động đẩy xuống, dẫn đến hiện tượng chèn ép và đè nát văn bản bài viết.

CSS Grid giải quyết triệt để vấn đề này nhờ cơ chế điều khiển không gian 2D tự động. Các khung ảnh Mosaic giữ nguyên dòng chảy DOM, co giãn linh hoạt theo tỷ lệ `fr`, tự điều chỉnh hàng/cột qua Breakpoints mà không làm vỡ các thành phần xung quanh.