# Trading Lab – Hướng dẫn cho Claude

## Tổng quan
- App Trading Lab chạy trên GitHub Pages, chủ yếu xem trên iPhone (Safari).
- Toàn bộ app nằm trong một file `index.html` (HTML + CSS + JS), không dùng công cụ build.
- App có 3 tab:
  1. **Lab mô phỏng**
  2. **Trợ lý gộp lệnh**
  3. **Giá trực tuyến** – giá từ Binance, chỉ đọc, không giao dịch.

## Quy ước
- Giao diện và chú thích (comment trong code) viết bằng tiếng Việt.
- Gọi **"sản phẩm"** và **"tiền mặt"** thay cho coin/USDT.
- Không tính phí và thuế trong mô phỏng.
- Không sửa logic các phương pháp cũ nếu người dùng không yêu cầu.

## Quy trình sau mỗi lần sửa
1. Kiểm tra app không lỗi (không lỗi JS, chạy được cả 3 tab).
2. Commit với lời nhắn tiếng Việt.
3. Gộp (merge) thẳng vào nhánh `main` để GitHub Pages cập nhật.
