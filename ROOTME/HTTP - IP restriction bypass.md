# Mô tả 
- Thử thách này liến quan đến việc bạn bypass cái địa chỉ IP của trang web từ đó bỏ việc đăng nhập
# Giải pháp 
## Lý thuyết 
- Lỗ hổng HTTP - IP Restriction Bypass là một loại lỗ hổng bảo mật xảy ra khi cơ chế kiểm soát truy cập dựa trên địa chỉ IP được cấu hình để bảo vệ tài nguyên không hoạt động như mong đợi, cho phép kẻ tấn công bỏ qua các hạn chế này và truy cập trái phép vào hệ thống.
- Khi một ứng dụng web hoặc API giới hạn quyền truy cập dựa trên IP (ví dụ, chỉ cho phép truy cập từ các IP đáng tin cậy hoặc IP nội bộ), kẻ tấn công có thể khai thác lỗ hổng để vượt qua kiểm tra IP bằng cách:
    - Sử dụng Proxy hoặc VPN: Ẩn IP thực hoặc giả mạo IP để phù hợp với danh sách được phép.
    - Khai thác Header HTTP: Gửi các giá trị giả mạo trong các header như `X-Forwarded-For`, `X-Real-IP`, hoặc `Forwarded`.
    - Lợi dụng lỗ hổng máy chủ/ngược dòng: Khi máy chủ ngược dòng (reverse proxy) hoặc cân bằng tải xử lý kiểm tra IP không đúng cách.
    - Bỏ qua bằng IP nội bộ: Nếu ứng dụng không kiểm tra đúng cách IP nội bộ, kẻ tấn công có thể giả mạo một IP trong dải nội bộ (127.0.0.1, 10.x.x.x, 192.168.x.x...).
## Giải web
- sử dụng burp suite và tôi chỉnh sửa POST gửi đi bằng cách thêm IP giả mạo vào phần header `X-Forwarded-For:192.168.0.1` và send và ở phần respone tôi đã nhận được cờ `Ip_$po0Fing`.

<img width="1067" alt="Ảnh màn hình 2024-12-21 lúc 12 53 59" src="https://github.com/user-attachments/assets/fb5f7593-a5a9-424b-b97c-1dc9d5b8b541" />
