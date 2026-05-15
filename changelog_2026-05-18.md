# Changelog

## [2026-05-18] — (GMT+7)

### Quản lý tích hợp & Quản lý nhân viên — Modal xác nhận xoá Webhook & Icon Button

**Các giao diện được cập nhật:**

---

#### Node ID: `WcTDt` — Integration Management · Modal xác nhận xoá Webhook

Bổ sung **modal xác nhận** khi người dùng thực hiện xoá một webhook đã thêm:

- Hiển thị popup xác nhận trước khi xoá để tránh thao tác nhầm
- Nội dung modal nêu rõ hành động không thể hoàn tác
- Gồm 2 nút hành động: **Huỷ** và **Xác nhận xoá**

---

#### Node ID: `VOT6X` — User Management · Quản lý nhân viên · Icon Button

Thay thế **text button** bằng **icon button** trên trang Quản lý nhân viên:

- Trước: các nút hành động hiển thị dạng text label
- Sau: các nút hành động chuyển sang dạng icon — gọn hơn, tiết kiệm không gian

---

#### Node ID: `fcNAl`, `CIvXS`, `EC7tK`, `GNoxY`, `L4wm7e` — Integration Management · Chi tiết xác thực Webhook & Preview Payload

Bổ sung giao diện **detail cho từng loại xác thực** và tính năng **Preview Payload**:

- Giao diện hiển thị chi tiết tương ứng với từng phương thức xác thực mà user đã config (Bearer Token, API Key, Basic Auth, v.v.)
- Tính năng **Preview** cho phép user quan sát trực tiếp cấu trúc request sẽ được gửi đến webhook dựa trên thông tin đã cấu hình — giúp kiểm tra và debug dễ dàng hơn trước khi lưu

| Node | Nội dung |
|------|----------|
| `fcNAl` | Giao diện detail xác thực NONE |
| `CIvXS` | Giao diện detail xác thực API_KEY |
| `EC7tK` | Giao diện detail xác thực BEARER + không check Dynamic token |
| `GNoxY` | Giao diện detail xác thực BEARER + check Dynamic token |
| `L4wm7e` | Giao diện detail xác thực BASIC-AUTH |

---

**Người thực hiện:** Linn  
**Ảnh hưởng:** 7 node (`WcTDt`, `VOT6X`, `fcNAl`, `CIvXS`, `EC7tK`, `GNoxY`, `L4wm7e`) thuộc luồng Quản lý tích hợp & Quản lý nhân viên
