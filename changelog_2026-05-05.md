# Changelog

## [2026-05-05] — 15:15 (GMT+7)

### Quản lý tích hợp — Thêm trường Authentication Methods cho Webhook

**Các giao diện được cập nhật:**

---

#### Node ID: `l9Z5z` — Integration management · General (màn hình chính)

Trong phần **Webhook URLs** trên trang Quản lý tích hợp, mỗi webhook entry nay hiển thị thêm trường **Authentication Methods** ngay bên dưới URL. Trường này phản ánh phương thức xác thực đang được áp dụng và hiển thị các thông tin con tương ứng:

| Webhook | Authentication Methods | Thông tin bổ sung |
|---------|------------------------|-------------------|
| Webhook 1 | Không có | — |
| Webhook 2 | Bearer Token | Hiển thị trường Token |
| Webhook 3 | API Key | Hiển thị Key Name + Key Value |
| Webhook 4 | Basic Auth | Hiển thị Username + Password |

---

#### Node ID: `oTvtN` — Integration management · UI Component (modal Cập nhật tài khoản)

Trong modal **Cập nhật tài khoản**, mỗi card Webhook (Webhook 1–4) được bổ sung trường **Authentication Methods** dạng dropdown, cho phép người dùng chọn phương thức xác thực khi chỉnh sửa. Tuỳ theo lựa chọn, các trường nhập liệu bổ sung sẽ hiện ra:

- **Không có** — Không có trường phụ
- **Bearer Token** — Hiển thị thêm input Token
- **API Key** — Hiển thị thêm Key Name và Key Value
- **Basic Auth** — Hiển thị thêm Username và Password

---

**Người thực hiện:** Linn  
**Ảnh hưởng:** 2 màn hình (`l9Z5z`, `oTvtN`) thuộc luồng Quản lý tích hợp
