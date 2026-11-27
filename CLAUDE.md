# Trading Lab – Hướng dẫn cho Claude

## Tổng quan
- App Trading Lab chạy trên GitHub Pages, chủ yếu xem trên iPhone (Safari).
- Toàn bộ app nằm trong một file `index.html` (HTML + CSS + JS), không dùng công cụ build.
- App có 5 tab:
  1. **Lab mô phỏng**
  2. **Trợ lý gộp lệnh**
  3. **Lọc sản phẩm** – tải nến lịch sử từ Binance, chạy thử các phương pháp của Lab và xếp hạng sản phẩm hợp với từng phương pháp.
  4. **Giá trực tuyến** – giá từ Binance, chỉ đọc, không giao dịch.
  5. **Robot nhắc lệnh** – theo dõi giá Binance (nến 1 phút, WebSocket) khi app đang mở, nhắc khi giá chạm mắc cần đặt lệnh theo sổ của Trợ lý gộp lệnh, mắc lưới hoặc mức giá; báo bằng âm thanh, khung nhắc và Telegram (tùy chọn). Chỉ nhắc, không đặt lệnh, không sửa sổ.

## Quy ước
- Giao diện và chú thích (comment trong code) viết bằng tiếng Việt.
- Gọi **"sản phẩm"** và **"tiền mặt"** thay cho coin/USDT.
- Không tính phí và thuế trong mô phỏng.
- Không sửa logic các phương pháp cũ nếu người dùng không yêu cầu.

## Quy trình sau mỗi lần sửa
1. Kiểm tra app không lỗi (không lỗi JS, chạy được cả 5 tab).
   Đổi hằng số `APP_VER` ở cuối `index.html` (ví dụ `2026-11-27.4`) để app trên iPhone tự nhận ra bản mới.
2. Commit với lời nhắn tiếng Việt.
3. Gộp (merge) thẳng vào nhánh `main` để GitHub Pages cập nhật.
4. Sau khi push, cập nhật bản copy `index.html` vào artifact **Trading Lab**: https://claude.ai/artifact/5cf3XchL4Vqsf95AQRRnUq (đăng lại vào đúng URL này, không tạo artifact mới).
