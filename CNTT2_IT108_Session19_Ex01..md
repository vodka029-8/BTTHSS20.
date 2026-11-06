
#1. Ký tự lạ và Cơ chế đánh lừa

• Ký tự lạ: Chữ ú có dấu sắc (U+00FA) thay vì chữ u thường trong chữ github.
• Cơ chế đánh lừa (Homograph Attack):
	• Kẻ gian tạo tên miền giả chứa ký tự Unicode nhìn giống hệt chữ gốc để lừa mắt thường.
	• Hệ thống dịch tên miền này thành chuỗi Punycode: xn--githb-bva.com.
	• Khi lập trình viên gõ tài khoản, thông tin sẽ gửi về máy chủ của kẻ gian thay vì GitHub thật.

##2. Quy trình kiểm tra URL nhanh


Bằng mắt thường (3 giây)

• Nhìn kỹ dấu thanh: Kiểm tra xem tên miền có bị thừa dấu (ú, í, à) hoặc nét lạ không.
• Copy ra nơi khác: Copy URL dán vào thanh tìm kiếm hoặc file Notepad. Nếu nó hiện ra chữ bắt đầu bằng xn--, đó là trang giả mạo.

Bằng công cụ (Tự động)

• Trình quản lý mật khẩu: Dùng Bitwarden, 1Password... Nếu là trang giả, công cụ sẽ không tự động điền (Auto-fill) mật khẩu.
• Tiện ích mở rộng (Extension): Cài các tiện ích chống Phishing/Homograph trên trình duyệt để tự động chặn tên miền độc hại.
