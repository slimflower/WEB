# Mô tả 
Trong thử thách này tôi sẽ làm quen với 1 tool mới là burp suite Tôi sẽ phải tìm flag trong yêu cầu được gửi tới sever thông qua burp suite 
<img width="998" alt="Ảnh màn hình 2024-12-04 lúc 20 56 35" src="https://github.com/user-attachments/assets/0b215940-f700-47d0-ab12-7b4356170b17">

# Giải pháp 
Mở burp suite và tạo proxy mới .Khi truy cập vào trang web tôi được giao diện.

<img width="1005" alt="Ảnh màn hình 2024-12-04 lúc 20 57 59" src="https://github.com/user-attachments/assets/cb9d1432-a48e-4055-96be-02b928f53c10">

Tôi thử nhập và tạo đăng ký,sau đó trang web yêu cầu nhập mã otp thì tôi mở Intercept của proxy lên và gửi 1 otp bất kì .Tôi sẽ nhận được 1 Post sau đó tôi repeater Post đó và xoá otp đi và send thì tôi được flag .

<img width="1068" alt="Ảnh màn hình 2024-12-04 lúc 21 24 15" src="https://github.com/user-attachments/assets/212e516f-1cfe-4d33-9304-50cf844ea99b">

 Flag : ***picoCTF{#0TP_Bypvss_SuCc3$S_c94b61ac}***
