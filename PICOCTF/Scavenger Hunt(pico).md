# Mô tả 

<img width="1440" alt="Ảnh màn hình 2024-12-05 lúc 09 45 22" src="https://github.com/user-attachments/assets/303e0a77-e0b8-4d11-b813-6622b0a7f9e8">

Thử thách này liên quan đến HTML ,vậy tôi sẽ đi tìm kiếm flag ở view soucre 
# Giải pháp 
- Khi tôi truy cập vào trang web và tôi nhận được 2 câu hỏi How và What

<img width="1440" alt="Ảnh màn hình 2024-12-05 lúc 09 52 42" src="https://github.com/user-attachments/assets/3cfda239-acf0-411e-b26f-f49922a74d57">

- Bây giờ tôi vào view soucre và tôi đã tìm được phần đầu của flag

<img width="1440" alt="Ảnh màn hình 2024-12-05 lúc 09 53 56" src="https://github.com/user-attachments/assets/bda8e298-161a-459d-9112-596c0160176b">

- Bây giờ tôi sẽ tìm phần tiếp theo,tôi vào xem file mycss.css và tôi tìm được phần flag thứ 2 và hints ` CSS makes the page look nice, and yes, it also has part of the flag.`

<img width="1440" alt="Ảnh màn hình 2024-12-05 lúc 09 55 36" src="https://github.com/user-attachments/assets/8d7e8a74-635b-4c37-a98f-a5a43c83a2da">

- Tôi vào file myjs.js tôi không tìm được flag nhưng tôi nhận được 1 gợi ý `How can I keep Google from indexing my website?`. Chúng ta phải nghĩ về cách Google có thể theo dõi tất cả các trang web này? Nó sử dụng công cụ thu thập dữ liệu/nhện của Google. Nhưng vì các nhà phát triển không muốn những con nhện này tiếp cận và `index` mọi phần của trang web, chúng tôi sử dụng một tệp đặc biệt có tên là `robots.txt`! Tệp này cho các trình thu thập dữ liệu biết những phần nào của trang web không được phép và những Tác nhân người dùng nào được phép truy cập (cùng với những thứ khác). Các trình thu thập dữ liệu lắng nghe các tệp này được gọi là `polite`, khi trình thu thập dữ liệu không được phép, `polite` nó có thể rơi vào thứ gọi là spider trap. Sau phần lan man nhỏ của tôi, đây là nội dung của robots.txt:

<img width="618" alt="Ảnh màn hình 2024-12-05 lúc 09 59 30" src="https://github.com/user-attachments/assets/253fb507-9595-403d-b958-7179050c4f28">

- Và tôi đã tìm phần flag thứ 3 . Gợi ý được cung cấp ở tệp robots là `I think this is an apache server... can you Access the next flag?` .Phần flag tiếp theo sẽ liên quan về apache server vậy tôi sẽ truy cập `.htaccess` để tìm flag :

  <img width="702" alt="Ảnh màn hình 2024-12-05 lúc 10 01 58" src="https://github.com/user-attachments/assets/294510bd-bafe-4ece-a287-5565563a1586">

- Tôi đã tìm được phần 4  của flag . Theo những gì tôi đọc được, .DS_Stoređây là một tệp MacOS đặc biệt lưu trữ thông tin về thư mục hiện tại. Giống như vị trí biểu tượng, v.v. Bạn cũng có thể thấy nó nếu bạn giải nén tệp từ người dùng Mac trên máy tính không phải Mac. Một loại mã thông báo nhận dạng máy tính Mac:

  <img width="497" alt="Ảnh màn hình 2024-12-05 lúc 10 04 00" src="https://github.com/user-attachments/assets/938511e4-f570-4fa9-8543-74a6ec209dc3">

Flag : ***picoCTF{th4ts_4_l0t_0f_pl4c3s_2_lO0k_f7ce8828}***

  
