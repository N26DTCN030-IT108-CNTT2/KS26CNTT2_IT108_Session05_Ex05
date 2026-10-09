\# BÀI 5

\## IN PUT 



Thư mục đầu vào downloads của máy chủ đang bị đầy và chưa được phân loại



\## PROCESS



Di chuyển vào folder Downloads



Tạo hai folder con media/ và scripts/



Quét định dạng tệp theo lệnh đã nhập

&#x20;   - nếu là .png , .jpg thì vào folder media/

&#x20;   - nếu là .py thì vào folder scripts/

&#x20;   - nếu là .tmp tiến hành xóa (rm)





\## OUT PUT



Thư mục Downloads đã sạch sẽ, và được sắp xếp gọn gàng. Ngoài ra các file tạm cũng đã bị xóa sạch hoàn toàn.



\---



\# KỊCH BẢN LỆNH



md media ; md scripts 

mv \*.png, .jpg ./media/ ; mv \*.py ./scripts/

rm \*.tmp 



*Nếu Robot gặp một thư mục trùng tên với file đang di chuyển, hệ thống báo lỗi \*"Is a directory"\* (kiến thức đã học ở Lesson 04). Robot cần xử lý thế nào để không gây crash?*



thêm dấu / vào sau tên thư mục mỗi khi di chuyển vd

mv \*.png, .jpg **./media*/***  

**để đi đến bên trong thư mục cần đến**

