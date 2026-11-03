**Bài 1 : Sự cố không truy cập được hệ thống quản trị**

**Phần 1: phân tích**

- **Input: [phong-dieu-phoi.grenlog.vn](http://phong-dieu-phoi.greenlog.vn/)**  
- **Output: Ip không tồn tại**  
- **Sơ đồ luồng dữ liệu: gõ sai URL → tra cứu tên miền → báo lỗi NXDOMAIN**

## **Phần 2\. Triển khai**

- Lỗi DNS: Lỗi nằm ở phía Client.   
- Lỗi `500 Internal Server Error`: Lỗi nằm ở phía Server 

  ### **Quy trình kiểm tra HTTP Status Code**

1. Bấm F12 để mở Developer Tools, chọn tab Network.  
2. Nhập địa chỉ trang web và bấm Enter.  
3. Quan sát cột Status:

## **Phần 3\. Kiểm thử**

- **Trạng thái:** Yêu cầu đã chạm tới máy chủ thành công   
- **Vấn đề:** Đường dẫn hoặc tài nguyên không tồn tại trên Web Server 