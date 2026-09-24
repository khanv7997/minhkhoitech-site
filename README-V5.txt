MINH KHÔI TECH — V5 CMS + BÀI VIẾT + HÌNH ẢNH

MỚI TRONG V5
- Giữ nguyên landing page V4, domain, phone/Zalo, bảng giá, Form endpoint, GTM.
- /admin/ có thêm mục “Bài viết & hình ảnh”.
- Có thể tạo/sửa/xóa bài, bật/tắt công khai, chọn danh mục, ảnh đại diện và album ảnh.
- Trang danh sách: https://minhkhoitech.vn/bai-viet/
- URL bài viết: https://minhkhoitech.vn/bai-viet/<slug>
- Trang chủ tự lấy 3 bài công khai mới nhất.
- Ảnh upload từ CMS lưu tại assets/uploads/.

CÁCH UPDATE
1. Nếu Netlify đang nối GitHub (khuyến nghị):
   - Chép toàn bộ file V5 vào repo minhkhoitech-site, thay file cũ.
   - Commit + Push.
   - Netlify tự deploy.
2. Nếu còn deploy thủ công:
   - Có thể kéo thư mục V5 vào Netlify để xem website.
   - Tuy nhiên để nút Publish trong /admin/ hoạt động, project phải liên kết đúng repository GitHub.

SAU KHI DEPLOY
- Kiểm tra /
- Kiểm tra /bai-viet/
- Kiểm tra /bai-viet/5-dau-hieu-camera-can-kiem-tra
- Kiểm tra /admin/

CÁCH ĐĂNG BÀI
/admin/ > Bài viết & hình ảnh > Quản lý bài viết > Danh sách bài viết > Add item
Điền:
- Tiêu đề
- Slug URL (chữ thường, không dấu, dấu gạch ngang)
- Danh mục
- Ngày đăng
- Mô tả ngắn
- Ảnh đại diện
- Nội dung bài
- Album ảnh (nếu có)
- Đăng công khai = ON
Sau đó bấm Publish. Netlify sẽ tự deploy commit mới.

LƯU Ý
- posts.json có sẵn 2 bài kiến thức công khai và 1 bài mẫu công trình đang ẩn. Có thể sửa/xóa tùy ý.
- V5 là CMS tĩnh không dùng database; toàn bộ nội dung được lưu trong GitHub.
- Nếu đổi repo: mở /admin/?reset=1.
- Không cần sửa DNS, P.A Việt Nam hoặc SSL khi chỉ update source.


V5.1 - IT HELPDESK TỪ XA
- Bổ sung section Helpdesk từ xa theo tháng trên trang chủ.
- Gói tham khảo: 2.000.000đ/tháng cho quy mô khoảng 10 máy.
- Phản hồi/bắt đầu xử lý trong vòng 2 giờ, giờ hành chính.
- Onsite, vật tư, thiết bị, phần mềm bản quyền và sửa phần cứng báo phí riêng.
- Toàn bộ nội dung Helpdesk chỉnh được trong /admin/.
