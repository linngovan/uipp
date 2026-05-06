# Changelog

## [2026-05-06] — 17:08 (GMT+7)

### Quản lý tích hợp — Empty state, popup không có webhook & Required fields / Error message

**Các giao diện được cập nhật:**

---

#### Node ID: `ciBXE` — Integration management · Empty state (Webhook section)

Bổ sung trạng thái **empty state** cho phần Webhook URLs trên màn hình chính khi người dùng chưa thêm webhook nào:

- Header vẫn hiển thị label **"Webhook URLs"** và counter **"0 webhook(s)"** ở góc phải
- Vùng nội dung hiển thị icon webhook (lucide) trên nền tròn xám nhạt
- Tiêu đề: **"Chưa có webhook nào"**
- Mô tả: *"Thêm webhook URL để nhận thông báo real-time khi trạng thái đơn hàng thay đổi."*
- Đường phân cách (divider) ngăn giữa header và vùng empty body

---

#### Node ID: `xYGEY` — Integration management · Modal Cập nhật tài khoản (chưa có webhook)

Biến thể modal **"Cập nhật tài khoản"** khi người dùng chưa thêm bất kỳ webhook nào:

- Hiển thị đầy đủ các required fields có đánh dấu `*` đỏ: Tên Hợp Pháp Công Ty, ID, Số Điện Thoại, Tên Nhân Hiệu, Email
- Phần **Webhooks** chỉ gồm tiêu đề section và link **"+ Thêm webhook"** — không có webhook card nào
- Footer: nút **Huỷ** và **Lưu** như thường

---

#### Node ID: `EjJnD` — Integration management · Modal Cập nhật tài khoản (Required fields & Error message)

Bổ sung trạng thái **validation / error** cho modal "Cập nhật tài khoản":

- Tất cả labels của các trường bắt buộc đều có dấu `*` màu đỏ (`#EF4444`) đứng trước tên trường
- Các trường bắt buộc bao gồm: Tên Hợp Pháp Công Ty, ID, Số Điện Thoại, Tên Nhân Hiệu, Email
- Trường **URL** trong mỗi webhook card (Webhook 1–4) chuyển sang trạng thái lỗi khi bỏ trống:
  - Border đổi sang màu đỏ
  - Text placeholder đổi màu đỏ báo lỗi
- Hiển thị đồng thời 4 webhook cards với error state để thể hiện toàn bộ các trường hợp validation

---

**Người thực hiện:** Linn  
**Ảnh hưởng:** 3 màn hình (`ciBXE`, `xYGEY`, `EjJnD`) thuộc luồng Quản lý tích hợp
