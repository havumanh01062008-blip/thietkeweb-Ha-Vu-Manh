# AI_log – Nhật ký sử dụng AI

**Đề tài:** Website Câu Lạc Bộ Bóng Chuyền Đại Nam
**Môn học:** Nhập môn Công nghệ thông tin – Trường Đại học Đại Nam
**Sinh viên:** Hà Vũ Mạnh – Lớp 20-02 – K20

---

## 1. Công cụ AI đã sử dụng

| Công cụ | Dùng để làm gì |
|---|---|
| Claude (Anthropic) | Viết tài liệu (`README.md`, `AI_log.md`, `CHANGE_log.md`), rà soát và sửa lỗi cấu trúc HTML |

Em chỉ dùng **một** công cụ AI trong bài này.

## 2. Nguyên tắc em tự đặt ra

- Dùng AI để **hỗ trợ**, không để AI làm thay toàn bộ bài.
- Nội dung AI viết ra phải được em **đọc lại và đối chiếu với code thật** của mình.
- Ghi lại trung thực từng lần dùng AI, kể cả những chỗ AI làm chưa đúng hoặc chưa đủ.

## 3. Bảng tóm tắt các lần sử dụng

| Lần | Ngày | Em nhờ AI việc gì | Kết quả |
|---|---|---|---|
| 1 | 23/11/2026 | Viết 3 file tài liệu từ code HTML và CSS của em | `README.md`, `AI_log.md`, `CHANGE_log.md` bản đầu và danh sách 8 lỗi trong code |
| 2 | 24/11/2026 | Viết lại `index.html` đã sửa các lỗi AI tìm ra | `index.html` đã sửa và `CHANGE_log.md` cập nhật |
| 3 | 24/11/2026 | Gửi toàn bộ nội dung 5 file dạng text để em dán vào VS Code | Nội dung `index.html`, `style.css` và 3 file `.md` |
| 4 | 25/11/2026 | Viết lại `AI_log.md` cho đầy đủ và trung thực hơn | File này |

## 4. Chi tiết từng lần

### Lần 1 – Nhờ AI viết tài liệu cho dự án (23/11/2026)

- **Em đưa cho AI:** file `index.html` và `style.css` do em làm.
- **Yêu cầu của em:** Viết giúp `README.md`, `AI_log.md` và `CHANGE_log.md` cho bài tập lớn, theo văn phong của sinh viên năm nhất.
- **AI trả về:**
  - Ba file tài liệu mô tả website, cấu trúc thư mục, cách chạy, bảng màu, hạn chế và hướng phát triển.
  - Danh sách 8 vấn đề AI tìm thấy khi đọc code (ghi trong `CHANGE_log.md`), ví dụ: thiếu thẻ `<body>`, thiếu `</nav>`, thừa/thiếu `</section>`, đường dẫn ảnh banner `images/anh2.jpg` không khớp thư mục `asset/`.
- **Em làm tiếp:** đọc lại nội dung, đối chiếu với code và cấu trúc thư mục thật của em.

### Lần 2 – Nhờ AI viết lại code HTML đã sửa lỗi (24/11/2026)

- **Yêu cầu của em:** Viết lại code theo các lỗi đã được chỉ ra.
- **AI trả về:** `index.html` mới với các thay đổi:
  - thêm thẻ `<body>` và thẻ `</nav>`;
  - xóa `</section>` thừa sau banner;
  - thêm `</section>` đóng phần Thư viện hình ảnh;
  - đổi thứ tự menu để "Trang chủ" đứng trước "Cá nhân";
  - thêm dòng bản quyền trong footer (dùng class `.copyright` đã có sẵn trong CSS của em).
- **AI cập nhật** `CHANGE_log.md`: đánh dấu ✅ các lỗi 1, 2, 3, 4, 6, 7.
- **Chưa sửa:** lỗi 5 (đường dẫn ảnh banner) và lỗi 8 (tên ảnh có dấu cách), vì AI không biết tên ảnh thật trong thư mục `asset` của em nên em phải tự làm.

### Lần 3 – Nhờ AI gửi nội dung file dạng text (24/11/2026)

- **Yêu cầu của em:** Viết toàn bộ nội dung để em copy và dán vào Visual Studio Code.
- **AI trả về:** Nội dung của `index.html`, `style.css`, `README.md`, `AI_log.md`, `CHANGE_log.md`. Code CSS giữ nguyên như em đã viết, chỉ thêm một dòng ghi chú nhắc đổi đường dẫn ảnh banner.
- **Em làm tiếp:** tạo file trong VS Code, dán nội dung vào và chỉnh lại cho khớp với bài của em.

### Lần 4 – Nhờ AI viết lại AI_log (25/11/2026)

- **Yêu cầu của em:** Viết lại `AI_log.md`.
- **AI trả về:** Bản `AI_log.md` này, ghi theo từng lần dùng AI.

## 5. Cách em kiểm tra kết quả của AI

- Mở `index.html` bằng Live Server trên VS Code để xem trang chạy thật.
- Bấm thử từng mục trên menu để kiểm tra cuộn tới đúng phần.
- Kiểm tra các ảnh trong thư mục `asset` có hiện đầy đủ không, tên file có khớp với code không.
- Dùng Chrome DevTools để xem giao diện ở kích thước điện thoại (dưới 768px và dưới 480px).
- Đối chiếu tên file, tên class, màu sắc trong README với `style.css` thật.

## 6. Phần em tự làm

- Chọn chủ đề CLB Bóng chuyền Đại Nam.
- Viết nội dung HTML (giới thiệu bản thân, giới thiệu CLB, hoạt động, thư viện ảnh).
- Viết toàn bộ CSS: bảng màu, Flexbox, Grid, hiệu ứng rê chuột, giao diện điện thoại.
- Chọn, đặt tên và sắp xếp các hình ảnh trong thư mục `asset`.
- Kiểm tra, chỉnh sửa và quyết định nội dung cuối cùng nộp bài.

## 7. Những hạn chế em nhận thấy ở AI

- AI **không nhìn thấy thư mục ảnh thật** trên máy em, nên không biết ảnh banner đúng tên gì, em phải tự sửa.
- AI tìm lỗi bằng cách **đọc code**, không chạy thử trang web, nên em vẫn phải tự mở trình duyệt để kiểm tra.
- Nội dung AI viết là **mẫu chung**, em phải đối chiếu lại với bài của mình, nhất là những phần nói về việc em đã làm gì.

## 8. Em học được gì

- Mỗi thẻ HTML mở ra đều phải có thẻ đóng tương ứng, thiếu hoặc thừa một thẻ có thể làm giao diện bị lỗi.
- Đường dẫn ảnh phải khớp chính xác tên thư mục và tên file.
- Nên đặt tên file ảnh không có dấu cách và không có dấu tiếng Việt để tránh lỗi khi đưa lên mạng.
- AI hỗ trợ nhanh nhưng không thay được việc tự kiểm tra, và em phải hiểu nội dung mình nộp.

## 9. Cam kết

Em xin cam đoan đã ghi lại đúng những lần em sử dụng AI trong bài này và em hiểu nội dung bài nộp của mình.

*Hà Vũ Mạnh – Lớp 20-02 – K20*
