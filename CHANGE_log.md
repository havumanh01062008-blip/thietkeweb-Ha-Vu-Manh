# CHANGE_log – Nhật ký thay đổi

**Dự án:** Website Câu Lạc Bộ Bóng Chuyền Đại Nam
**Môn học:** Nhập môn Công nghệ thông tin – Trường Đại học Đại Nam
**Sinh viên:** Hà Vũ Mạnh – Lớp 20-02 – K20
**Phiên bản hiện tại:** 1.1

Nhật ký ghi lại những thay đổi của dự án theo từng phiên bản, mới nhất ở trên cùng.

---

## [1.1] – 25/11/2026 – Sửa lỗi cấu trúc HTML và hoàn thiện tài liệu

### Đã sửa
- `index.html`: thêm thẻ `<body>` sau `</head>` (trước đó file có `</body>` ở cuối nhưng không có thẻ mở).
- `index.html`: thêm thẻ `</nav>` còn thiếu trong phần menu.
- `index.html`: xóa thẻ `</section>` bị thừa sau phần banner.
- `index.html`: thêm thẻ `</section>` đóng phần Thư viện hình ảnh.
- `index.html`: đổi thứ tự menu thành Trang chủ → Cá nhân → Giới thiệu → Hoạt động → Hình ảnh, cho khớp với thứ tự các phần trên trang.

### Đã thêm
- `index.html`: dòng bản quyền trong footer (`© 2026 Hà Vũ Mạnh - Lớp 20-02 - K20`), dùng class `.copyright` đã có sẵn trong `style.css`.
- `AI_log.md`: viết lại, ghi chi tiết từng lần sử dụng AI (23/11, 24/11, 25/11), cách kiểm tra kết quả, hạn chế của AI và bài học.
- `CHANGE_log.md`: viết lại theo từng phiên bản.

### Chưa sửa (còn tồn tại)
- Đường dẫn ảnh banner trong `style.css` (lỗi số 5).
- Tên file ảnh có dấu cách trong thư mục `asset` (lỗi số 8).

---

## [1.0] – 23/11/2026 – Bản hoàn chỉnh đầu tiên

### Đã thêm
- `index.html` với 7 phần: menu, trang chủ (banner), thông tin cá nhân, giới thiệu CLB, hoạt động, thư viện hình ảnh, chân trang.
- `style.css` gồm:
  - cài đặt chung và bảng màu (xanh navy, vàng, xám xanh nhạt);
  - menu cố định khi cuộn (`position: sticky`) và cuộn mượt (`scroll-behavior: smooth`);
  - bố cục bằng Flexbox (menu, giới thiệu, hoạt động, thông tin cá nhân) và Grid (thư viện ảnh 3 cột);
  - hiệu ứng đổi màu khi rê chuột vào menu và nút bấm, hiệu ứng nổi lên nhẹ ở thẻ hoạt động và ảnh;
  - giao diện điện thoại bằng `@media` (dưới 768px: gallery 2 cột; dưới 480px: gallery 1 cột).
- Thư mục `asset` chứa 7 hình ảnh (1 ảnh cá nhân, 1 ảnh giới thiệu, 5 ảnh thư viện).
- Ba file tài liệu: `README.md`, `AI_log.md`, `CHANGE_log.md`.

---

## Bảng theo dõi lỗi

> Cập nhật lần cuối: 25/11/2026. Khi sửa xong một lỗi, đổi ⬜ thành ✅ và ghi ngày sửa.

| STT | File | Vấn đề | Cách sửa | Trạng thái |
|---|---|---|---|---|
| 1 | `index.html` | Thiếu thẻ mở `<body>` nhưng cuối file có `</body>` | Thêm `<body>` sau `</head>` | ✅ Đã sửa (24/11/2026) |
| 2 | `index.html` | Thẻ `<nav>` chưa được đóng | Thêm `</nav>` trước `</header>` | ✅ Đã sửa (24/11/2026) |
| 3 | `index.html` | Thừa một thẻ `</section>` sau phần banner | Xóa thẻ thừa | ✅ Đã sửa (24/11/2026) |
| 4 | `index.html` | Phần Thư viện hình ảnh thiếu `</section>` | Thêm `</section>` sau `</div>` của gallery | ✅ Đã sửa (24/11/2026) |
| 5 | `style.css` | Ảnh banner trỏ tới `images/anh2.jpg`, trong khi ảnh nằm ở thư mục `asset/` | Đổi đường dẫn cho đúng thư mục và tên ảnh thật | ⬜ Chưa sửa |
| 6 | `index.html` | Menu để "Cá nhân" trước "Trang chủ", không khớp thứ tự trên trang | Đổi thứ tự menu | ✅ Đã sửa (24/11/2026) |
| 7 | `index.html` | Class `.copyright` có trong CSS nhưng chưa dùng trong HTML | Thêm dòng bản quyền vào footer | ✅ Đã sửa (24/11/2026) |
| 8 | `asset/` | Tên ảnh có dấu cách (ví dụ `trang ca nhan.jpg`) dễ lỗi khi đưa lên mạng | Đổi thành `trang-ca-nhan.jpg` và sửa lại đường dẫn trong HTML | ⬜ Chưa sửa |

---

## Kế hoạch cập nhật sau này

- [ ] Sửa lỗi số 5 và số 8 trong bảng trên.
- [ ] Thêm menu thu gọn (nút ☰) cho điện thoại.
- [ ] Thêm lịch tập luyện và thông tin liên hệ của CLB.
- [ ] Thêm form đăng ký tham gia CLB.
- [ ] Đưa website lên GitHub Pages.

---
*Hà Vũ Mạnh – Lớp 20-02 – K20 – Cập nhật lần cuối: 25/11/2026*
