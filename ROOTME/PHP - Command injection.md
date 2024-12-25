# Mô tả 
- Chall theo tên  đề bài là PHP - Command injection vì vậy chúng ta sẽ sử dụng các hàm của linux và burp suite để tìm flag
# Giải pháp 
- Ban đầu tôi thử nhập 127.0.0.1 và xem POST có gì

<img width="1058" alt="Ảnh màn hình 2024-12-25 lúc 23 00 09" src="https://github.com/user-attachments/assets/1e9ee786-2836-446d-b53f-59be2181cf73" />

- Tôi thấy có file index.php vậy tôi thử xem file đó có gì nên tôi sử dụng lệnh `127.0.0.1 && cat index.php` và tôi nhận được

  <img width="1077" alt="Ảnh màn hình 2024-12-25 lúc 23 02 01" src="https://github.com/user-attachments/assets/4503ec8e-8eed-4816-8162-1e1056c5fa79" />

   - đọc source thì tôi hiểu tôi cần xem file .passwd thì sex có được flag

  <img width="1344" alt="Ảnh màn hình 2024-12-25 lúc 23 03 16" src="https://github.com/user-attachments/assets/566fc69a-3285-4c5d-9a29-c036cabf65bc" />

- Như vậy tôi đã tìm được flag .Chall này chủ yếu sử dụng các lệnh linux để truy cập vào các file pass để lấy flag
  
