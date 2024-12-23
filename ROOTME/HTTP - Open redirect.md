# Mô tả 
- Bài này liên quan đến việc chuyển hướng trang web
# Giải pháp 
- Nếu chúng ta chuyển hướng trang web đến cái hướng cho phép thì chúng ta sẽ thấy hiện ở phần POST của burp suite

<img width="1051" alt="Ảnh màn hình 2024-12-21 lúc 13 25 43" src="https://github.com/user-attachments/assets/1517d228-4ecf-42de-a9fe-9fb9a89fc5b1" />

- Chúng ta hãy phân tích của POST .Chúng ta sẽ thấy có 2 phần một là dường dẫn tên miền của trang web và 1 phần sau **h** .Vậy chúng là gì thì chúng ta sẽ biết được đó là hàm băm md5 .
- Vậy để tìm được flag chúng ta cần điều hướng sang một trang web khác với các thành phần giống POST
- Chúng ta sex điều hướng trang web đến `https://www.google.com.vn/?hl=vi` với hàm băm md5 của link này là `47069fe028cb71841bc1ecdbea73849f` và send thì chúng ta sẽ nhận được flag .

![Uploading Ảnh màn hình 2024-12-23 lúc 21.36.06.png…]()

