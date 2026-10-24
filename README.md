# QuanLyTaiKhoanNganHang (Quản Lý Tài Khoản Ngân Hàng)

Ứng dụng Quản lý tài khoản ngân hàng được phát triển bằng ngôn ngữ **C# (Windows Forms / .NET Framework 4.7.2)** kết hợp cơ sở dữ liệu **Microsoft SQL Server**.

---

## 📌 Tính Năng Chính

- **Hệ thống xác thực:**
  - Đăng ký tài khoản người dùng mới (kèm ảnh đại diện, thông tin CCCD, email, số điện thoại...).
  - Đăng nhập bảo mật vào hệ thống.
  - Quên mật khẩu / khôi phục mật khẩu.
  - Cập nhật thông tin tài khoản & xóa tài khoản.
- **Nghiệp vụ tài chính ngân hàng:**
  - Tra cứu / kiểm tra số dư hiện tại.
  - Nạp tiền / gửi tiền vào tài khoản.
  - Rút tiền từ tài khoản.
  - Chuyển tiền liên tài khoản với thông báo xác nhận và kiểm tra số dư.
  - Lịch sử & thông tin giao dịch chi tiết (ngày giờ, loại giao dịch, số tiền).
- **Tiện ích:**
  - Tích hợp máy tính (Calculator) hỗ trợ tính toán nhanh chóng.
  - Giao diện thân thiện, trực quan với bộ icon ngân hàng hoàn chỉnh.

---

## 🛠 Công Nghệ Sử Dụng

- **Ngôn ngữ:** C# (.NET Framework 4.7.2)
- **Giao diện:** Windows Forms (WinForms)
- **Cơ sở dữ liệu:** Microsoft SQL Server
- **Công cụ phát triển:** Visual Studio 2019 / 2022, SQL Server Management Studio (SSMS)

---

## 🚀 Hướng Dẫn Cài Đặt & Chạy Ứng Dụng

### 1. Chuẩn bị Cơ sở dữ liệu (SQL Server)
1. Mở **SQL Server Management Studio (SSMS)**.
2. Mở tệp SQL tại thư mục: `SqlServerDataBase/Database.sql`.
3. Nhấn **Execute** (`F5`) để tạo cơ sở dữ liệu `QuanLyTaiKhoanNganHang` cùng các bảng cần thiết.

### 2. Cấu hình Chuỗi Kết Nối
Mở tệp `QuanLyTaiKhoanNganHang/Connection.cs` và cập nhật chuỗi kết nối phù hợp với máy của bạn:
```csharp
private static string stringConnection = @"Data Source=YOUR_SERVER_NAME\SQLEXPRESS;Initial Catalog=QuanLyTaiKhoanNganHang;Integrated Security=True";
```

### 3. Chạy Ứng Dụng
1. Mở file giải pháp `QuanLyTaiKhoanNganHang.sln` bằng Visual Studio.
2. Nhấn `Build Solution` (Ctrl + Shift + B).
3. Nhấn **Start** (`F5`) để chạy chương trình.
