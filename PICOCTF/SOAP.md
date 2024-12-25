# Mô tả 
- Chall liên quan đến lỗ hổng `XML External Entity (XXE) Injection` và sử dụng burp suite để giải quyết
## XML External Entity (XXE) Injection là gì ?
- XML external entity injection (còn được gọi là XXE) là một lỗ hổng bảo mật web cho phép kẻ tấn công can thiệp vào quá trình xử lý dữ liệu XML của ứng dụng. Nó thường cho phép kẻ tấn công xem các tệp trên hệ thống tệp máy chủ ứng dụng và tương tác với bất kỳ hệ thống phụ trợ hoặc hệ thống bên ngoài nào mà chính ứng dụng có thể truy cập.
## Lỗ hổng được phát sinh như thế nào 
- Một số ứng dụng sử dụng định dạng XML để truyền dữ liệu giữa trình duyệt và máy chủ. Các ứng dụng thực hiện việc này hầu như luôn sử dụng thư viện chuẩn hoặc API nền tảng để xử lý dữ liệu XML trên máy chủ. Các lỗ hổng XXE phát sinh do đặc tả XML chứa nhiều tính năng có khả năng gây nguy hiểm và trình phân tích cú pháp chuẩn hỗ trợ các tính năng này ngay cả khi chúng không được ứng dụng sử dụng bình thường.
## Những loại tấn công XXE 
- Khai thác XXE để truy xuất các tệp , trong đó một thực thể bên ngoài được định nghĩa có chứa nội dung của tệp và được trả về trong phản hồi của ứng dụng.
- Khai thác XXE để thực hiện các cuộc tấn công SSRF , trong đó một thực thể bên ngoài được xác định dựa trên URL tới hệ thống phụ trợ.
- Khai thác XXE mù để đánh cắp dữ liệu ngoài băng tần , trong đó dữ liệu nhạy cảm được truyền từ máy chủ ứng dụng đến hệ thống do kẻ tấn công kiểm soát.
- Khai thác XXE mù để truy xuất dữ liệu thông qua thông báo lỗi , trong đó kẻ tấn công có thể kích hoạt thông báo lỗi phân tích cú pháp có chứa dữ liệu nhạy cảm.
# Giải pháp 
- Chall này liênn quan đến việc tấn công XXE để truy xuất tệp `etc/passwd`
- Để thực hiện cuộc tấn công tiêm XXE nhằm truy xuất một tệp tùy ý từ hệ thống tệp của máy chủ, bạn cần sửa đổi XML đã gửi theo hai cách:
  - Giới thiệu (hoặc chỉnh sửa) một DOCTYPEphần tử xác định một thực thể bên ngoài có chứa đường dẫn đến tệp.
  - Chỉnh sửa giá trị dữ liệu trong XML được trả về trong phản hồi của ứng dụng để sử dụng thực thể bên ngoài đã xác định.
- Sử dụng burp suite và xem POST thì tôi thấy phần XML của tôi :
  
             <?xml version="1.0" encoding="UTF-8"?><data><ID>3</ID></data>

- Và để truy xxuaats được tệp etc/passwd thì tôi cần repeater cái POST này thành :

             
