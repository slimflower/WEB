# Mô tả 
- Bài này liên quan đến Headers của HTTP vì vậy chúng ta càn sử dụng burp suite để xem request và respones của nó để tìm flag
# Giải pháp 
- Ta hãy so sánh phần request và respones của web và thấy có sự khác biệt ở `Header-RootMe-Admin: none` .Vì dòng này ở respones có nhưng ở resquets không có .Dòng này cho ta biết headers admin của web không có vì vậy chúng ta cần sửa cho nó thành có để tìm flag

  <img width="1059" alt="Ảnh màn hình 2024-12-24 lúc 08 57 00" src="https://github.com/user-attachments/assets/1a4f3369-c8b1-4949-8c38-813fd3a882ae" />

- Chúng ta đã tìm ra Flag : `HeadersMayBeUseful`
