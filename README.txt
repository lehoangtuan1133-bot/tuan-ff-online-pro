TUAN FF ONLINE - GIỮ NGUYÊN GAME + BỔ SUNG QUẢN LÝ TÀI KHOẢN

Trong ZIP:
- public/index.html: game gốc được giữ nguyên từ file hiện có.
- public/admin.html: trang admin riêng, bổ sung danh sách toàn bộ tài khoản.
- server.js: server Socket.IO gốc, bổ sung khóa/mở, xóa và đặt lại mật khẩu tài khoản.
- package.json: lệnh chạy Render.

RENDER
Build Command: npm install
Start Command: npm start

Environment:
ADMIN_PASSWORD = mật khẩu admin riêng
DATABASE_URL = Internal Database URL của PostgreSQL Render

Nếu đang có PostgreSQL cũ, server tự thêm cột is_banned vào bảng game_accounts.
Nếu không có DATABASE_URL, tài khoản chỉ lưu RAM và mất khi server khởi động lại.

LINK SAU DEPLOY
Trang game/người chơi: https://TEN-SERVICE.onrender.com/
Trang admin: https://TEN-SERVICE.onrender.com/admin.html

QUẢN TRỊ
Admin dùng ADMIN_PASSWORD. Sau khi đăng nhập có thể xem người chơi online, phòng, và tải danh sách tất cả tài khoản (kể cả offline), khóa/mở khóa, đặt lại mật khẩu, xóa tài khoản.

LƯU Ý
- Game được giữ nguyên, không thay bằng trang đăng nhập mẫu.
- Bản này giữ nguyên giao thức game Socket.IO hiện có.
- Kiểm tra DATABASE_URL để dữ liệu tài khoản tồn tại sau khi restart.
