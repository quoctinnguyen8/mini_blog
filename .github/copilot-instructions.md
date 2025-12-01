Dưới đây là **danh sách đầy đủ và có cấu trúc** cho đề tài **“Website Blog Mini có Trang Quản Trị”** dưới dạng **Markdown**, chia theo **Frontend, Backend, User, Admin**, và cả **chức năng nâng cao**.

---

# 📝 Website Blog Mini có Trang Quản Trị

## 1. Chức năng người dùng (Frontend)

### **1.1. Trang chủ**

* Hiển thị danh sách bài viết theo thứ tự mới nhất
* Phân trang (pagination)
* Sidebar: danh mục, bài viết nổi bật

### **1.2. Trang xem bài viết**

* Xem chi tiết bài viết
* Hiển thị:

  * Tiêu đề
  * Ảnh thumbnail
  * Nội dung
  * Ngày đăng
  * Tác giả
  * Danh mục
* Gợi ý bài viết liên quan theo danh mục

### **1.3. Tìm kiếm**

* Tìm kiếm theo tiêu đề bài viết

### **1.4. Xem bài theo danh mục**

* Danh sách bài viết thuộc một danh mục
* Phân trang

---

## 2. Chức năng quản trị (Admin Panel)

### **2.1. Authentication**

* Đăng nhập admin
* Đăng xuất
* Quên mật khẩu

### **2.2. Dashboard**

* Thống kê số bài viết
* Số danh mục
* Số tài khoản admin
* Biểu đồ thống kê

---

## 3. Quản lý bài viết (Post Management)

### **3.1. CRUD bài viết**

* Tạo bài viết
* Sửa bài viết
* Xóa bài viết
* Xem danh sách bài viết

### **3.2. Trường dữ liệu bài viết**

* Tiêu đề
* Slug tự động
* Danh mục
* Ảnh thumbnail (upload file – Laravel Storage)
* Nội dung (dùng rich text editor: TinyMCE)
* Trạng thái:

  * Draft
  * Published
* Ngày đăng
* Tác giả

### **3.3. Tính năng nâng cao**

* Lọc bài viết theo:

  * Danh mục
  * Trạng thái
  * Tác giả
* Tìm kiếm bài theo tiêu đề
* Khôi phục bài viết (soft delete)

---

## 4. Quản lý danh mục (Category Management)

### **4.1. CRUD danh mục**

* Tạo danh mục
* Sửa danh mục
* Xóa danh mục
* Danh sách danh mục

### **4.2. Trường dữ liệu danh mục**

* Tên danh mục
* Slug tự động
* Mô tả

### **4.3. Tính năng nâng cao**

* Danh mục cha – con (nested category)
* Đếm số bài viết thuộc mỗi danh mục

---

## 5. Quản lý người dùng (User/Admin Management)

* Tạo tài khoản admin
* Phân quyền cơ bản:

  * Admin toàn quyền
  * Editor chỉ được tạo/sửa bài
* Cập nhật thông tin cá nhân
* Đổi mật khẩu

---

## 6. Các chức năng hệ thống

### **6.1. Upload & Storage**

* Upload ảnh bài viết
* Tự động resize/tối ưu ảnh
* Laravel storage: local, public

### **6.2. Bảo mật**

* Middleware kiểm tra admin
* CSRF token
* Validation toàn bộ form

### **6.3. SEO cơ bản**

* Slug cho bài viết & danh mục
* Meta title, meta description

### **6.4. Validation**
* Validate tất cả các form đầu vào (bài viết, danh mục, user)
* Thông báo lỗi được hiển thị bằng tiếng Việt

---

## 7. Tính năng nâng cao

### **7.1. Bình luận bài viết**

* Bình luận theo user
* Duyệt bình luận (moderation)

### **7.2. Like / View Count**

* Đếm lượt xem
* Like bài viết

### **7.3. API mini**

* API cho:

  * Danh sách bài viết
  * Xem bài
* Sử dụng Laravel API Resource

### **7.4. Dark mode**

* Giao diện dark/light

### **7.5. Trang giới thiệu & liên hệ**

* Form liên hệ gửi email bằng Laravel Mail


# Quy tắc

- Luôn phản hồi bằng tiếng Việt.
- Luôn tuần theo danh sách chức năng đã liệt kê ở trên.
- Sử dụng tiếng Việt có dấu trong toàn bộ giao diện và thông báo lỗi.
- Không dùng NodeJS.
- Không cần unit test.
- Dự án sử dụng hướng tiếp cận Code-First.
- Sử dụng bootstrap5 cho giao diện admin.
- Tất cả các file hướng dẫn .md được đặt ở thư mục `.docs` trong dự án.
- Luôn kiểm tra lại tên model, tên bảng, tên cột, tên biến, tên route đã có trong dự án hay chưa sau khi hoàn thành chức năng.

# Technical Stack

- Backend: Laravel 12.x, PHP 8.2
- Frontend: Blade Template + Bootstrap 5.3
- Database: MySQL

# Tài liệu

- https://laravel.com/docs/12.x
- https://getbootstrap.com/docs/5.3/getting-started/introduction/