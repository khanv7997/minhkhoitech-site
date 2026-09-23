MINH KHÔI LANDING V3 — CÓ TRANG QUẢN TRỊ /admin/
====================================================

Cấu trúc:
- index.html                 Website chính
- content/site.json          Toàn bộ nội dung có thể chỉnh trên giao diện
- admin/index.html           Trang quản trị Decap CMS
- assets/                    Logo và hình upload từ trang quản trị
- netlify.toml               Cấu hình Netlify

QUAN TRỌNG
V3 dùng GitHub làm nơi lưu source/content. Mỗi lần bấm Publish trong /admin,
Decap CMS commit thay đổi vào GitHub và Netlify tự deploy lại website.

THIẾT LẬP 1 LẦN
1) Deploy thư mục V3 này lên đúng project Netlify hiện tại.
2) Liên kết project Netlify với GitHub repository (khuyến nghị tên: minhkhoitech-site).
3) Tạo GitHub OAuth App:
   - Homepage URL: https://minhkhoitech.vn
   - Authorization callback URL: https://api.netlify.com/auth/done
4) Trên Netlify: Project configuration > Security > OAuth > Install Provider > GitHub.
   Nhập Client ID và Client Secret của OAuth App.
5) Mở https://minhkhoitech.vn/admin/
   Nhập repository dạng: username/minhkhoitech-site
6) Đăng nhập GitHub > sửa nội dung > Publish.

ĐỔI REPOSITORY
Mở: https://minhkhoitech.vn/admin/?reset=1

LƯU Ý
- DNS và HTTPS hiện tại không cần đổi.
- Chỉ người có quyền push vào GitHub repository mới có thể đăng nhập/sửa nội dung.
- Form endpoint có thể điền ngay trong trang quản trị sau khi nối Google Sheets/Apps Script.
