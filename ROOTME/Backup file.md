# Mô tả 
- Chall này liên quan đến việc backup file
# Giải pháp 
- ban đầu tôi xem source và nhập đại một tên và pass nào đấy và tôi đã nhập sai .Khi tôi sử dụng burp suite thì cũng không tìm được gì .Tôi nhớ lại tên Chall và backup file vì vậy tôi sử dụng tool dirseacrh để tìm file của trang web

   <img width="973" alt="Ảnh màn hình 2024-12-25 lúc 22 38 31" src="https://github.com/user-attachments/assets/b5899d44-724a-4fbd-b11b-a2b5b9e5cd0e" />

- Sau một hồi quằn quại với cái terminal về việc cài dirsearch thì cuối cùng tôi tìm được file index.php~ .Bây giờ tôi sẽ xem file dó có gì :

<img width="869" alt="Ảnh màn hình 2024-12-25 lúc 22 40 00" src="https://github.com/user-attachments/assets/662f532d-6181-4712-a78e-6719f928f3b7" />

- Quao tôi đã thấy được password của chall là `OCCY9AcNm1tj`.
