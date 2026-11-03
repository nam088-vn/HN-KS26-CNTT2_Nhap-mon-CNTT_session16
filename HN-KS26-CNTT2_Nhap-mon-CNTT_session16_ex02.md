**Bài 2 : Sự cố phiên làm việc trên hệ thống vận tải**

## **Phần 1\. Phân tích**

### 

| Tiêu chí | Cookie (\~4KB) | Browser Cache / Storage (MB/GB) |
| :---- | :---- | :---- |
| **Dung lượng** | Rất nhỏ (\~4KB) | Rất lớn (MB đến GB) |
| **Mục đích** | Lưu Token định danh  | Lưu giao diện, ảnh, CSS/JS, dữ liệu tạm |
| **Tự động gửi** | **Có**  | **Không**  |
| **Đánh đổi** | Ưu điểm: Bảo mật cao, tự định danh. Nhược: Giới hạn kích thước.  | Ưu: Lưu được nhiều dữ liệu giỏ hàng. Nhược: Dễ bị XSS nếu lưu Token.  |

## 

## **Phần 2\. Triển khai**

* **Tên và Giá trị :** Chứa mã định danh phiên làm việc của shipper.  
* **Thời gian sống :** Đặt thời hạn lưu trữ, giúp giữ trạng thái đăng nhập kể cả khi đóng hay load lại trình duyệt.  
* **Cờ bảo vệ dữ liệu:** Cấm các đoạn mã JavaScript phía Client đọc hoặc thao tác với Cookie  
* **Cờ bảo vệ đường truyền:** Yêu cầu trình duyệt chỉ gửi Cookie này qua các kết nối được mã hóa HTTPS, chống bị nghe lén trên đường truyền.


## **Phần 3\. Kiểm thử**

- **macOS:** Bấm Cmd \+ Shift \+ R.  
- **Di động:** Vào *Cài đặt trình duyệt* \-\> *Xóa dữ liệu duyệt web* \-\> Chọn xóa *Tệp và hình ảnh được lưu trong bộ nhớ đệm (Cache)*.

