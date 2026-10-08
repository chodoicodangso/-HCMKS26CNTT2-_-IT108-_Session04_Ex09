## Bước 1: Xác định vị trí hiện tại

**Câu lệnh:** `pwd`  
**Giải thích:** Hiển thị đường dẫn thư mục hiện hành trên máy chủ.

## Bước 2: Xác nhận sự cố

**Câu lệnh:** `ls public`  
**Giải thích:** Liệt kê các file trong thư mục `public` để xác nhận file bị lộ `db_password.txt` và file mã độc `hacker_log.bat`.

## Bước 3: Xử lý bẫy & Di chuyển an toàn

**Câu lệnh tạo thư mục:** `mkdir secrets`  
**Câu lệnh di chuyển file:** `mv public/db_password.txt secrets/`  
**Giải thích:** Tạo trước thư mục `secrets` để tránh hệ thống hiểu nhầm lệnh `mv` là đổi tên file. Sau đó di chuyển an toàn file mật khẩu vào thư mục mới.

## Bước 4: Dọn dẹp mã độc

**Câu lệnh:** `rm public/hacker_log.bat`  
**Giải thích:** Xóa vĩnh viễn tệp mã độc ra khỏi hệ thống.