# Mô tả về bài tập MongoDB CRUD

## Mục tiêu
Bài tập này giúp tìm hiểu cách tích hợp MongoDB vào một ứng dụng ASP.NET Core API. Quá trình bao gồm cài đặt MongoDB, tạo cơ sở dữ liệu, định nghĩa models, services, và controllers để thực thi các tác vụ CRUD.

---

## Quy trình thực hiện

1. **Cài đặt MongoDB**
   - Cài đặt MongoDB trên máy tính của bạn.

2. **Tạo database và thêm document**
   - Tạo cơ sở dữ liệu MongoDB.
   - Thêm hai document mẫu vào bộ sưu tập.

3. **Cài đặt MongoDB Driver**
   - Truy cập menu `Tools -> NuGet Package Manager` để cài đặt MongoDB.Driver.
   - Thêm thư mục `Models` vào dự án.
   - Tạo các lớp `Book` và `BookStoreDatabaseSettings`.
   - Cấu hình file `Program.cs` để sử dụng các model này.

4. **Thêm CRUD Service**
   - Tạo thư mục `Services` trong dự án.
   - Thêm lớp `BooksService` để xử lý các tác vụ CRUD: 
     - Lấy danh sách tất cả sách.
     - Lấy chi tiết sách theo ID.
     - Thêm sách mới.
     - Cập nhật sách theo ID.
     - Xóa sách theo ID.

5. **Thêm Controller**
   - Tạo lớp `BooksController.cs` để xử lý các yêu cầu API.
   - Định nghĩa các phương thức:
     - `GET /api/books`: Lấy danh sách sách.
     - `GET /api/books/{id}`: Lấy sách theo ID.
     - `POST /api/books`: Thêm sách mới.
     - `PUT /api/books/{id}`: Cập nhật sách.
     - `DELETE /api/books/{id}`: Xóa sách.

6. **Cấu hình và chạy ứng dụng**
   - Thêm Swagger để kiểm thử API.
   - Cấu hình middleware trong `Program.cs`.
   - Chạy ứng dụng và kiểm tra các API thông qua Swagger.

---

## Kết quả rút ra

- **Tích hợp MongoDB:** Biết cách kết nối MongoDB và ASP.NET Core API.
- **Tạo Models:** Biết tạo các models cơ bản nhồm biểu diễn cơ sở dữ liệu.
- **CRUD Service:** Hiểu rõ cách viết các tác vụ CRUD cho một collection.
- **API Controllers:** Biết viết và quản lý routing cho API controllers.
- **Swagger:** Biết sử dụng Swagger để test API nhanh chóng.

---

## Tài liệu tham khảo
- [MongoDB Documentation](https://www.mongodb.com/docs/)
- [ASP.NET Core Documentation](https://learn.microsoft.com/en-us/aspnet/core/)
