# BÀI LÀM – THI THỬ HACKATHON 02 (GAMEZONE)

- **Họ tên:** 
- **Lớp:** 
- **Link repository:** 
- **Hệ điều hành (Windows/macOS):** 

## 4.2. Thao tác CLI

### Các lệnh đã chạy

```shell
# Ghi lệnh vào đây
Hiển thị đường dẫn tuyệt đối thư mục hiện tại: pwd
Liệt kê nội dung, gồm cả file ẩn: ls -Force
Di chuyển cap_nhat.txt vào docs, file logo vào media:
Dùng đường dẫn tương đối vào logs, liệt kê nội dung rồi quay lại gốc: 
    + cd .\logs
    + ls
    + cd ..\
    
```

### Kết quả liệt kê toàn bộ dự án

```text
    Directory: C:\Users\ADMIN\Downloads\luyen_tap\starter-kit\gamezone-website


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        10/29/2026   8:27 AM                backup
d-----        10/29/2026   8:27 AM                data
d-----        10/29/2026   8:27 AM                docs
d-----        10/29/2026   8:27 AM                logs
d-----        10/29/2026   8:27 AM                media
-a----        10/29/2026   8:27 AM             70 .env
-a----        10/29/2026   8:27 AM            225 auto_report.ps1
-a----        10/29/2026   8:35 AM           1760 bai_lam.md

```

## 4.3. Lọc log thủ công

### Lệnh đã chạy

```shell
# Ghi lệnh vào đây
    + Get-Content .\logs\game.log | Select-String "ERROR" >> .\logs\daily_report.txt
    
```

### 2 dòng lỗi đầu tiên trong daily_report.txt

```text
(Dán kết quả vào đây)
2025-11-05 08:03:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:09:15 [ERROR] Mat ket noi may chu game
```

## 4.4. README.md

> Chấm trực tiếp trên `README.md` ở gốc dự án.

- [x] Heading 1
- [x] Mô tả in đậm + in nghiêng
- [x] Bảng `Thư mục | Nội dung` (≥3 dòng)
- [x] Code block lệnh liệt kê
- [x] Task list (≥2 việc, ≥1 đã xong)
- [x] Blockquote nhắc không upload `.env`

## 4.5. Chạy script auto_report

### Lệnh chạy

```shell
# Ghi lệnh vào đây
.\auto_report.ps1
```

### Nội dung file logs/auto_report.txt

```text
(Dán kết quả vào đây)
=== BAO CAO LOI GAMEZONE ===

2025-11-05 08:03:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:09:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:12:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:39:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:42:15 [ERROR] Mat ket noi may chu game
2025-11-05 08:51:15 [ERROR] Loi luu tien trinh choi

```

## 4.6. Đếm số dòng lỗi

### Lệnh

```shell
# Ghi lệnh vào đây
(Get-Content .\logs\game.log | Select-String "ERROR").Count
```

### Kết quả đếm

```text
(Dán kết quả vào đây)
6
```

## 4.7. Báo cáo tổng hợp

### Các lệnh đã chạy

```shell
# Ghi lệnh vào đây

```

### Nội dung file logs/tong_hop.txt

```text
(Dán kết quả vào đây)

```

## 4.8. Excel

> Chấm trực tiếp trên file `data/giao_dich_thang_11.xlsx`.
