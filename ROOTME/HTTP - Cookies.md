# Mô tả 
- Chall này liên quan đến cookies của trang web
# Giải pháp 
- Khi tôi save email thì web yêu cầu tôi phải là quản trị viên và tôi đi đọc source thì thấy hints `SetCookie("ch7","visiteur")`.Và nó liên quan đến cookies của trang web và tôi đax sài burp suite để xem request .

<img width="1059" alt="Ảnh màn hình 2024-12-24 lúc 19 44 59" src="https://github.com/user-attachments/assets/db70ae8d-65ed-48b5-b7b7-26cab7f927c4" />

- Cookies ở phần GET cho tôi thấy răng tôi chưa được câp quyền admin vì thế tôi không thể save email được ,và tôi sửa cookies `ch7=admin` và send thì tôi được flag

<img width="1060" alt="Ảnh màn hình 2024-12-24 lúc 19 46 20" src="https://github.com/user-attachments/assets/e81a58ab-dc0e-4d3c-ba82-a56892965448" />

