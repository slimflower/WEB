# Mô tả 

<img width="1440" alt="Ảnh màn hình 2024-12-07 lúc 19 18 22" src="https://github.com/user-attachments/assets/9525057b-efc3-4939-91b3-f903d69d2e4f">

- Thử thách này liên quan đến đăng nhập qua cookies .Khi truy cập vaò trang web tôi nhận được 1 trang đăng nhập .
<img width="1439" alt="Ảnh màn hình 2024-12-07 lúc 19 19 46" src="https://github.com/user-attachments/assets/e81cb698-3509-4dcc-9448-cb6fa0dce01d">

# Giải pháp 
- Tôi đăng nhập bằng 1 tài khoản bất kì thì trang web thông báo

<img width="1439" alt="Ảnh màn hình 2024-12-07 lúc 19 20 51" src="https://github.com/user-attachments/assets/00b4f51a-1b55-40f3-8e30-c84b1bdf1868">

- Trang web cho biết tôi đăng nhập thành công nhưng không có flag nào được giấu ở đây cả vì vậy tôi mang nó vào burp suite

<img width="1075" alt="Ảnh màn hình 2024-12-07 lúc 19 28 37" src="https://github.com/user-attachments/assets/39b11356-027d-4957-be1c-fa94f49cdf5d">

- Khi tôi đăng nhập thì thấy cookie của mình là False vì vậy tôi không thể tìm flag được.Tôi repeater sửa thành True và tìm được flag
<img width="1067" alt="Ảnh màn hình 2024-12-07 lúc 19 29 57" src="https://github.com/user-attachments/assets/1e9908d8-d3f6-49a7-be43-3ffc9c3c29a2">

Flag : `picoCTF{th3_c0nsp1r4cy_l1v3s_6edb3f5f}`
