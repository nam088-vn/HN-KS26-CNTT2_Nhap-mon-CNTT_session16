**Bài 4 : Sự cố xung đột phiên đăng nhập trên trình duyệt**

## **Phần 1\. Phân tích**

* **Chế độ ẩn danh:**

  * **Lưu trữ:** Lưu tạm thời trên bộ nhớ RAM.

  * **Đặc điểm:** Tự động xóa sạch toàn bộ Cookie, lịch sử web và mật khẩu ngay khi tắt cửa sổ.

  * **Hạn chế:** Phải đăng nhập lại từ đầu mỗi lần sử dụng, không giữ được trạng thái làm việc lâu dài.

* **Hồ sơ riêng biệt:**

  * **Lưu trữ:** Lưu cố định trên ổ cứng máy tính

  * **Đặc điểm:** Cách ly hoàn toàn dữ liệu giữa các Profile khác nhau.

  * **Ưu điểm:** Giúp duy trì đăng nhập song song 3 tài khoản mà không bị văng phiên.

## **Phần 2\. Triển khai**

### **1\. Quy trình tạo và đồng bộ 3 Profile** 

* **Tạo 3 Profile độc lập:** Bấm vào biểu tượng ảnh đại diện trên góc phải trình duyệt \-\> Chọn Add  \-\> Đặt tên lần lượt là Personal, Work, và Sandbox.

* **Bật đồng bộ :** Đăng nhập email tương ứng cho từng Profile \-\> Chọn Bật đồng bộ.Toàn bộ Bookmark và Mật khẩu sẽ được sao lưu lên mây.

### **2\. Cấu trúc cây thư mục Bookmark** 

- ### **Công cụ DEV:** GitHub, GitLab, Stack Overflow. 

- **Học tập và Quản lý:** Canvas LMS, Portal GreenLogistics.

- **Vận hành:** Trang quản trị phong-dieu-phoi.greenlog.vn.

## **Phần 3\. Kiểm thử**

* **Bật Guest Mode:** Bấm vào ảnh Profile \-\> Chọn **Open Guest Window**.

* **Thao tác:** Đăng nhập và làm việc tạm thời.

* **Thoát an toàn:** Tắt cửa sổ Guest.