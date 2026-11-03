## **Bài 5 : Tối ưu tiện ích mở rộng cho hệ thống điều phối vận tải**

## **Phần 1\. Phân tích**

* **Chuyển đổi dữ liệu thô:** Chuỗi JSON thô từ API máy chủ gửi về thường dính liền nhau, rất khó đọc.

* **Gỡ lỗi:** JSON Viewer tự động định dạng, tô màu cú pháp và thu gọn/mở rộng các cấu trúc dữ liệu. 

## **Phần 2\. Triển khai**

### **1\. Danh sách 5 Extensions theo nhóm**

* **Nhóm Dev Suite :**

  1. **JSON Formatter:** Tự động làm đẹp và phân cấu trúc chuỗi JSON API thô.

  2. **Postman / REST Client Extension:** Gửi request test trực tiếp API dữ liệu GPS trên trình duyệt.

* **Nhóm Productivity:**   
  3\. **ColorZilla:** Nhặt mã màu nhanh trên giao diện bản đồ điều phối.   
  4\. **Wappalyzer:** Nhận diện nhanh các công nghệ/thư viện mà trang web đang sử dụng.

* **Nhóm Security :**   
  5\. **uBlock Origin:** Chặn quảng cáo, mã độc và chặn theo dõi; cực kỳ nhẹ, tối ưu RAM đúng ràng buộc.

### **2\. Ghim Extension lên Toolbar & Bật Site Access** 

* **Ghim lên Toolbar:** Bấm biểu tượng Mảnh ghép trên góc phải trình duyệt \-\> Bấm biểu tượng Ghim bên cạnh tiện ích.

* **Phân quyền Site Access :** Click chuột phải vào biểu tượng Extension trên Toolbar \-\> Chọn **This Can Read and Change Site Data** \-\> Chọn **When You Click the Extension**

## **Phần 3\. Kiểm thử**

### Quy trình kiểm tra tài nguyên khi trình duyệt bị lag

1. Nhấn tổ hợp phím Shift \+ Esc \-\> *Công cụ khác* \-\> *Trình quản lý tác vụ*.

2. Tìm các dòng có tiền tố Extension: \[Tên tiện ích\].

3. Quan sát cột Memory footprint (Dung lượng bộ nhớ).

4. Nếu Extension nào ngốn quá nhiều RAM, chọn tiện ích đó và bấm End Process để tắt ngay lập tức.

