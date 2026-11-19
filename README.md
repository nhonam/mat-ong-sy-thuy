# Mật ong Sỹ Thủy — Landing page

Mật ong nhà nuôi tại vườn nhà, Xóm Cây Thị, Sơn Tây, Hà Tĩnh.

Bố là người nuôi ong và thu hoạch. Mật được quay ly tâm ngay trong ngày, sau đó
đưa qua máy lọc công nghệ cao để làm sạch và tách nước, chỉ giữ lại mật nguyên
chất. Mật đóng trong chai thủy tinh (không phải hũ).

Mở `index.html` bằng trình duyệt để xem. Để đưa lên mạng, chỉ cần tải cả thư mục
này (gồm `index.html` và thư mục `media`) lên hosting bất kỳ.

## 1. Số điện thoại và Zalo

Mở `index.html`, kéo xuống gần cuối trang, tìm khối:

```js
const SHOP = {
  phoneText: "0392 679 935",               // số hiện trên trang
  phoneHref: "tel:+84392679935",           // số dùng để gọi, dạng +84
  zalo: "https://zalo.me/0392679935",      // link Zalo; để trống sẽ ẩn nút
  messenger: ""                            // link Facebook Messenger; để trống sẽ ẩn nút
};
```

- `zalo`: link chat Zalo theo số điện thoại. Để trống `""` thì mọi nút Zalo tự ẩn.
- `messenger`: nếu có trang Facebook, dán link dạng `https://m.me/ten-trang`.
  Để trống thì nút Messenger (nếu có) tự ẩn.
- Số điện thoại hiển thị và nút gọi dùng chung cấu hình này, không cần sửa chỗ khác.
- Nút **Sao chép số** hoạt động sẵn.

## 2. Video và ảnh

Đặt tệp vào thư mục `media` (đã tạo sẵn) đúng tên:

| Tệp | Dùng ở đâu |
|---|---|
| `media/hero.mp4` | Video lớn ở đầu trang (tự phát, không tiếng) |
| `media/hero.jpg` | Ảnh nền cho video đầu trang |
| `media/story.jpg` | Ảnh lớn mục “Một chai mật đi qua nhiều đôi tay” |
| `media/process-1.jpg` | Quy trình 01 — Quay ly tâm |
| `media/process-2.jpg` | Quy trình 02 — Lọc máy, tách nước |
| `media/process-3.jpg` | Quy trình 03 — Đóng chai |
| `media/video-1.mp4` + `media/video-1.jpg` | Thước phim 01 — Thu hoạch trong vườn |
| `media/video-2.mp4` + `media/video-2.jpg` | Thước phim 02 — Quay ly tâm lấy mật |
| `media/video-3.mp4` + `media/video-3.jpg` | Thước phim 03 — Rót vào chai thủy tinh |
| `media/gallery-1.jpg` … `media/gallery-6.jpg` | Sáu khung ảnh cuối trang |

Ghi chú:

- Ảnh nên là JPG/WebP, cạnh dài khoảng 1600 px, dung lượng dưới 500 KB để tải nhanh.
- Video nên là MP4 (H.264), dưới 15 MB mỗi tệp.
- Chưa có tệp nào thì trang vẫn hiển thị khung chờ có sẵn tên tệp — không bị vỡ ảnh.
- Muốn dùng định dạng/tên khác: tìm `media/` trong `index.html` và đổi đường dẫn.

## 3. Nội dung khác

- Tên thương hiệu: “Mật ong Sỹ Thủy” (tìm chữ `MẬT ONG SỸ THỦY` để đổi).
- Địa chỉ: Xóm Cây Thị, Sơn Tây, Hà Tĩnh — sửa trong phần footer nếu cần.
- Quy trình hiển thị trên trang: nuôi ong trong vườn → quay ly tâm → lọc máy
  công nghệ cao, tách nước → đóng chai thủy tinh. Sửa ở mục “Quy trình” và
  “Câu chuyện”.
- Giá: trang không ghi giá, khách liên hệ Zalo hoặc gọi điện. Nếu muốn ghi giá,
  thêm vào phần `.card__meta` hoặc nội dung mục “Đặt hàng”.
- Trang nhắc “gọi trước để hẹn nhận mật tại vườn”; đổi câu này ở mục “Đặt hàng”
  nếu gia đình có giao hàng.
