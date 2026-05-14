# Changelog

## [2026-05-14] — (GMT+7)

### Quản lý đơn hàng — Cập nhật Design System màu Orange & Action Buttons dạng Icon

**Các giao diện được cập nhật:**

---

#### Node ID: `R8xXq` — Design System · Orange (beta)

Cập nhật bộ **Color brand** sang tone màu **Orange (Ahamove)** thay thế cho bộ màu Primary Blue trước đó:

- Bảng màu chính gồm 8 bậc từ `s00` (#FFF7F2) đến `s70` (#E35600)
- Màu mặc định / active (★): `s50` — **#FF7F32**
- Màu hover: `s60` — **#F55F00**
- Màu pressed: `s70` — **#E35600**
- Bổ sung trạng thái button: Default, Hover, Active, Disabled, Outline, Ghost
- Bổ sung trạng thái Icon Button (Popup): Outline (có viền), Ghost (không viền)
- Bổ sung trạng thái Outline Button & Cancel Button
- Bổ sung trạng thái Input / Dropdown: Default, Focus, Disabled, Error

---

#### Node ID: `UKUWB` — Order Management · New features · Order listing

Apply mẫu **Design System màu Orange** mới cho màn hình quản lý đơn hàng:

- Toàn bộ màu brand trong màn hình được chuẩn hoá theo bộ màu Orange (R8xXq)
- Các thành phần UI (tab active, nút tạo đơn, trạng thái đơn hàng, v.v.) phản ánh đúng tone màu cam chủ đạo

---

#### Node ID: `KMe3Y` — Order Management · Action Buttons (r1Actions)

Chuyển đổi các **action button** trong bảng danh sách đơn hàng từ dạng **Text sang Icon**:

- Trước: nút action hiển thị dạng text label
- Sau: nút action hiển thị dạng icon (lucide icon set) — gọn hơn, tiết kiệm không gian cột
- Áp dụng cho toàn bộ các rows trong bảng

---

**Người thực hiện:** Linn  
**Ảnh hưởng:** 3 màn hình / node (`R8xXq`, `UKUWB`, `KMe3Y`) thuộc luồng Design System & Quản lý đơn hàng
