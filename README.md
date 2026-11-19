# Mật ong Thủy Sỹ — Landing page

Hộ kinh doanh mật ong tại Sơn Tây, Hương Sơn, Hà Tĩnh.

Mở `index.html` bằng trình duyệt để xem. Để đưa lên mạng, chỉ cần tải cả thư mục này
(gồm `index.html` và thư mục `media`) lên hosting bất kỳ.

## 1. Số điện thoại và Facebook

Mở `index.html`, kéo xuống gần cuối trang, tìm khối:

```js
const SHOP = {
  phoneText: "0901 234 567",              // số hiện trên trang
  phoneHref: "tel:+84901234567",           // số dùng để gọi, dạng +84
  messenger: "https://m.me/matongthuysy",  // link Messenger của bạn
  zalo: ""                                 // ví dụ "https://zalo.me/0901234567"; để trống sẽ ẩn
};
```

- `messenger`: vào trang Facebook của bạn → **Nhắn tin** → sao chép link dạng
  `https://m.me/ten-trang`.
- Số điện thoại hiển thị và nút gọi dùng chung cấu hình này, không cần sửa chỗ khác.
- Nút **Sao chép số** hoạt động sẵn.

## 2. Video và ảnh

Đặt tệp vào thư mục `media` (đã tạo sẵn) đúng tên:

| Tệp | Dùng ở đâu |
|---|---|
| `media/hero.mp4` | Video lớn ở đầu trang (tự phát, không tiếng) |
| `media/hero.jpg` | Ảnh nền cho video đầu trang |
| `media/story.jpg` | Ảnh lớn mục “Một hũ mật đi qua nhiều đôi tay” |
| `media/product-1.jpg` | Sản phẩm 1 — Mật ong vườn nhà |
| `media/product-2.jpg` | Sản phẩm 2 — Mật ong hoa sim |
| `media/product-3.jpg` | Sản phẩm 3 — Mật ong hoa keo |
| `media/video-1.mp4` + `media/video-1.jpg` | Thước phim 01 |
| `media/video-2.mp4` + `media/video-2.jpg` | Thước phim 02 |
| `media/video-3.mp4` + `media/video-3.jpg` | Thước phim 03 |
| `media/gallery-1.jpg` … `media/gallery-6.jpg` | Sáu khung ảnh cuối trang |

Ghi chú:

- Ảnh nên là JPG/WebP, cạnh dài khoảng 1600 px, dung lượng dưới 500 KB để tải nhanh.
- Video nên là MP4 (H.264), dưới 15 MB mỗi tệp.
- Chưa có tệp nào thì trang vẫn hiển thị khung chờ có sẵn tên tệp — không bị vỡ ảnh.
- Muốn dùng định dạng/tên khác: tìm `media/` trong `index.html` và đổi đường dẫn.

## 3. Nội dung khác

- Tên hộ kinh doanh: “Mật ong Thủy Sỹ” (tìm chữ `MẬT ONG THỦY SỸ` để đổi).
- Địa chỉ: Sơn Tây, Hương Sơn, Hà Tĩnh — sửa trong phần footer nếu cần.
- Giá: trang đang dùng “Nhắn hỏi giá”. Nếu muốn ghi giá, thêm vào phần `.card__meta`.
- Mùa hoa, độ ẩm, quy trình: sửa trong mục “Chuyện của mật” và dải thông số ở đầu trang.
