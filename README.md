# Landing Page - Workshop Bài Dịch Lý 64 Quẻ

Project này là landing page cho chiến dịch đăng ký **Workshop Bài Dịch Lý 64 Quẻ**.

File chính đang dùng:

- `6index.html`

## Thông Tin Chiến Dịch

- Hình thức: Workshop Zoom trực tiếp
- Thời lượng: 03 buổi thực hành
- Giá: 2.000.000đ
- Quà tặng: Bộ bài Dịch Lý 64 quẻ trị giá 860.000đ
- Số suất: 100 suất/lớp
- Host: Dịch học sỹ Trần Thái Bình
- Nhóm Zalo: https://zalo.me/g/metc8pjimofspkcynl0k

Thông điệp chính:

> Đăng ký Workshop 03 buổi, nhận bộ bài Dịch Lý 64 quẻ trị giá 860.000đ, học xong biết dùng và biết cách mở thêm một kênh tăng thu nhập.

## Cấu Trúc File

- `6index.html`: Landing page chính, gồm HTML, CSS và JavaScript inline.
- `Image/`: Thư mục ảnh dùng trong landing page.
- `Image/image.png`: Logo.
- `Image/image (2).png`: Ảnh bộ bài chính trong hero và gallery.
- `Image/image (4).png`, `Image/image (5).png`: Ảnh bộ bài phụ trong hero/gallery.
- `Image/image (3).png`: Ảnh host.
- `Image/image (6).png`: Ảnh social/TikTok preview.
- `Image/image (7).png`: QR/Zalo.

## Cách Mở Nhanh

Mở trực tiếp file:

```text
6index.html
```

Landing page không cần build step hoặc dev server vì toàn bộ CSS/JS đang nằm trong file HTML.

## Các Khu Vực Chính

- Hero: headline, CTA, countdown, value stack và visual bộ bài.
- Countdown: đếm ngược đến `20:00 · 22/05/2026`.
- Nhận được gì: kết quả sau 03 buổi.
- Lộ trình: Buổi 1, Buổi 2, Buổi 3.
- Offer: giá, quà tặng, value stack.
- Gallery: hình ảnh bộ bài.
- Host: thông tin Dịch học sỹ Trần Thái Bình.
- Niềm tin trước khi đăng ký: lý do đăng ký, không dùng review giả.
- FAQ: xử lý phản đối chính.
- Đăng ký: form giữ chỗ và link Zalo.

## Checklist Test Nhanh

Trước khi chạy ads hoặc gửi khách, kiểm tra:

- Mở `6index.html` trên desktop.
- Bật mobile responsive, ưu tiên khoảng rộng 360px-430px.
- Kiểm tra không có overflow ngang.
- Bấm các CTA xem có về đúng `#dang-ky` hoặc mở Zalo.
- Kiểm tra countdown vẫn chạy.
- Kiểm tra ảnh bộ bài, host, QR hiển thị đúng.
- Submit thử form và xác nhận thông báo thành công hiện ra.
- Kiểm tra sticky CTA trên mobile không che form quá nhiều.

## Lưu Ý Khi Chỉnh Sửa

- Không đổi thông tin cốt lõi của chiến dịch nếu chưa được xác nhận.
- Không dùng review giả.
- Không dùng các từ nội bộ như `demo`, `fake`, `Academy`, `có thể chỉnh sau`.
- Giữ tone màu: đỏ rượu, nâu trầm, vàng kim, kem.
- CTA chính nên ưu tiên về `#dang-ky`.
- Link Zalo hiện tại: `https://zalo.me/g/metc8pjimofspkcynl0k`.

## Form Đăng Ký

Form hiện đang lưu lead vào `localStorage` với key:

```text
dichLyWorkshopLeads
```

Nếu cần gửi lead về backend/Google Sheet/API, cập nhật biến sau trong script của `6index.html`:

```js
const CONFIG = {
  zaloGroupUrl: "https://zalo.me/g/metc8pjimofspkcynl0k",
  formEndpoint: ""
};
```

Điền endpoint thật vào `formEndpoint` khi có hệ thống nhận lead.
