# Mô tả 
- khi tôi truy cập vào trang web thoi user đề bài cho thì tôi nhận được giao diện như sau :

<img width="1440" alt="Ảnh màn hình 2025-01-03 lúc 22 09 54" src="https://github.com/user-attachments/assets/427cc646-a652-45ab-a3cc-8c75e2b8e49b" />

- Tôi để ý lúc tôi truy cập vào trên đường url của trang web hiện 2 id nào đó . Với cách bình thường tôi không thể nào chặn được chúng để xem vì vậy tôi sử dung burp suite để chặn và xem thì tôi nhận ra đó là 2 mã base64 tôi giải mã và tìm được flag :

<img width="1074" alt="Ảnh màn hình 2025-01-03 lúc 22 11 49" src="https://github.com/user-attachments/assets/346711f7-29b9-4ac7-8d18-d28a6163f2b5" />

<img width="1094" alt="Ảnh màn hình 2025-01-03 lúc 22 12 16" src="https://github.com/user-attachments/assets/320664f6-d50d-4136-b6da-79c08cef1f85" />

- flag : `picoCTF{proxies_all_the_way_3d9e3697}`
