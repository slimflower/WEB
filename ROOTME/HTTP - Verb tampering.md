# Mô tả 
- Chall này liên quan đến sự xác thực của HTTP ,tôi sẽ dùng burp suite để giải quyết bài này
# Giải pháp 
- `HTTP Verb Tampering` là một lỗ hổng bảo mật xảy ra khi ứng dụng web xử lý không đúng cách các HTTP methods (hoặc HTTP verbs, như GET, POST, PUT, DELETE, PATCH, v.v.). Kẻ tấn công có thể tận dụng lỗ hổng này để truy cập trái phép, thay đổi dữ liệu, hoặc thực hiện các hành vi không mong muốn.
- Khi tôi xác thực được và vào trang đăng nhập thì tôi không thể đăng nhập vào vì không biết pass nên sử dụng burp suite để xem request của nó và tôi để ý đến tiêu đề là Verb tampering và tôi thử sửa các methods xem sao và khi tôi sửa thành POST thì không được gì nhưng tôi sửa thành PATCH thì tôi đã được pass

<img width="1064" alt="Ảnh màn hình 2024-12-24 lúc 15 14 04" src="https://github.com/user-attachments/assets/573d208e-b427-4c5b-8220-6cb604aae24a" />

