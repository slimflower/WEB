# Mô tả 
- `HTTP Improper Redirect` là một lỗ hổng bảo mật xảy ra khi một ứng dụng web thực hiện việc chuyển hướng (redirect) không đúng cách. Điều này có thể gây ra các vấn đề như tấn công Open Redirect, xâm phạm dữ liệu người dùng, hoặc các hành vi không mong muốn khác. Dưới đây là các đặc điểm chính:
- Hints của chall cho rằng chúng ta cần truy cập vào index của nó
# Giải pháp 
- Khi tôi sử burp suite của web để xem requets của web khi gửi đi thì tôi thấy phần GET có thành phần `redirect`
- Theo hints thì tôi thử dẫn đến thư mục index.php thử xem sao và tôi nhận được flag : `ExecutionAfterRedirectIsBad`

![Uploading Ảnh màn hình 2024-12-24 lúc 09.24.54.png…]()
