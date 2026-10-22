# Kho Tàng Tri Thức — Knowledge Hub & K Token

Phiên bản khởi tạo giao diện responsive, ưu tiên điện thoại Android. Dự án dùng HTML/CSS/JavaScript thuần, không cần cài đặt thư viện để xem bản demo.

## Chạy trên điện thoại Android
1. Tải file ZIP và giải nén bằng ứng dụng quản lý tệp.
2. Mở thư mục `kho_tang_tri_thuc`.
3. Mở `index.html` bằng trình duyệt. Nếu một số trình duyệt hạn chế chức năng khi mở file trực tiếp, hãy đưa thư mục lên dịch vụ hosting HTTPS.
4. Không cần cài ứng dụng hay chạy lệnh terminal cho bản xem trước.

## Những gì đã có
- Giao diện tiếng Việt, responsive, chế độ sáng/tối.
- Logo SVG và favicon.
- Trang chủ, 15 danh mục, tìm kiếm, lọc, sắp xếp.
- 15 bài viết mẫu, trang đọc bài, tăng/giảm cỡ chữ, chia sẻ.
- Lưu bài và lịch sử đọc trên thiết bị bằng `localStorage`.
- Bảng xếp hạng có ghi chú dữ liệu lượt xem minh họa.
- Hồ sơ khách và thống kê cục bộ.
- Ví K Token, phương thức nạp và hộp thoại bảo trì.
- Admin Dashboard ở chế độ minh họa.

## Chưa kết nối — cần cấu hình trước khi dùng thật
- Đăng nhập Google thật: cấu hình Firebase Authentication, bật Google provider, thêm domain hợp lệ và tích hợp SDK.
- Backend/cơ sở dữ liệu, đồng bộ hồ sơ và dữ liệu đa thiết bị.
- Tác vụ cập nhật tri thức hằng ngày, API nguồn, kiểm duyệt, lịch sử đồng bộ.
- Phân quyền admin phía máy chủ.
- Hệ thống K Token và cổng thanh toán: hiện hoàn toàn bảo trì; không nhận tiền, không tạo số dư thật, không có quy đổi.
- Nội dung bài viết hiện là bản mẫu giáo dục, có ghi chú nguồn cần kiểm chứng; cần biên tập và xác minh nguồn trước khi xuất bản công khai.

## Cấu trúc
- `index.html` — cấu trúc trang.
- `styles.css` — giao diện responsive và dark mode.
- `app.js` — dữ liệu mẫu, điều hướng, tìm kiếm, lưu bài, lịch sử và modal.
- `assets/logo.svg` — logo chính.
- `assets/favicon.svg` — favicon.

## Lưu ý an toàn
Không đưa khóa bí mật, thông tin thanh toán hoặc quyền admin vào frontend công khai. Không coi `localStorage` là cơ sở dữ liệu bảo mật. Mọi số dư token thật và mọi giao dịch tương lai phải được kiểm tra ở backend.
