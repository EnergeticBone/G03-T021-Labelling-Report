# Problem backlog

Những chỗ gặp trong lúc gán nhãn mà **guideline chưa trả lời được**, cộng các pain point về công cụ.

Ghi ngay khi gặp, kể cả lúc chưa biết xử lý thế nào. Một edge case không được ghi lại thì
mỗi người sẽ tự xử lý theo một kiểu — và đó là nguồn lớn nhất của nhãn không nhất quán.

> Các mục bên dưới là **ví dụ**, tên và link CVAT đều giả. Mẫu trống để copy nằm cuối file.

## Danh sách


| Mã              | Tóm tắt                         | Loại                   | Mục guideline | Trạng thái   | Kết quả |
| --------------- | ------------------------------- | ---------------------- | ------------- | ------------ | ------- |
| [P-001](#p-001) | Các xe nằm gần nhau quá dày đặc | Guideline chưa nói tới | —             | 🗣️ Đang bàn | —       |
| [P-002](#p-002) | Xe bị che khuất bởi hàng rào    | Guideline mơ hồ        | —             | 🗣️ Đang bàn | —       |


**Loại**


| Loại                   | Nghĩa là                                           |
| ---------------------- | -------------------------------------------------- |
| Guideline chưa nói tới | Tình huống không có trong guideline                |
| Guideline mơ hồ        | Đọc guideline ra được hai cách hiểu trở lên        |
| Guideline mâu thuẫn    | Hai mục trong guideline nói ngược nhau             |
| Pain point công cụ     | Guideline rõ, nhưng làm trên CVAT chậm hoặc dễ sai |


**Trạng thái:** 🔴 Mở · 🗣️ Đang bàn · ↗️ Hỏi BTC · ✅ Đã chốt (trỏ sang QĐ) · 🛠️ Làm tool (trỏ sang `source-tool/`) · ⚪ Bỏ (ghi lý do)

---



## P-001

**Các xe nằm gần nhau dày đặc:**

- **Loại:** Guideline chưa nói tới
- **Mục guideline:** §3 — Quy tắc bounding box
- **Người phát hiện:** @EnergeticBone · 15/09/2026
- **Link CVAT:**
  - [Link 1](https://cvat.note.transformerlabs.ai/tasks/141/jobs/1410) — Nhiều xe ở cạnh nhau, bounding box vẽ chèn lên nhau nhiều
  - [Link 2](https://cvat.note.transformerlabs.ai/tasks/141/jobs/1410) — Nhiều xe ở cạnh nhau, có xe bật đèn nên bị loá
- **Mô tả:** §3 — Quy tắc bounding box nói Mỗi object = một annotation riêng. Không dùng một box để bao nhiều object độc lập và Với object bị che/cắt mép, vẫn annotate nếu còn đủ bằng chứng thị giác để xác định class; dùng attribute phù hợp, tuy nhiên chưa đề cập đến việc khi có quá nhiều bounding box ở cùng một chỗ đè lên nhau thì xử lý thế nào.
- **Các cách hiểu:**
  1. Theo câu chữ: Vẫn phải vẽ dù đè lên nhau
  2. Theo cách hiểu cá nhân: Nhiều bounding box cùng đè lên nhau trong một khoảng khung hình nhỏ liệu có phải một dữ liệu tốt?
- **Xử lý tạm trong lúc chờ:** Tạo issue chờ thống nhất xử lý
- **Kết quả:** Đang chờ kết quả



## P-002

**Xe bị che khuất bởi hàng rào**

- **Loại:** Guideline mơ hồ
- **Mục guideline:** §3 — Quy tắc vẽ mask và xử lý biên
- **Người phát hiện:** @Nguyễn Đăng Huân · 16/09/2026
- **Link CVAT:**
  - [Link 1](https://cvat.note.transformerlabs.ai/tasks/194/jobs/1628) — Xe con ở sau hàng rào, tuy nhiên hàng rào trên ảnh mờ, không che được xe phía sau
- **Mô tả:** Quy tắc nói Semantic segmentation chỉ gán các pixel đang nhìn thấy. Không suy đoán và tô phần vật thể bị che bởi vật khác. Không rõ gán nhãn vật thể bị che hay vật thể che.
- **Các cách hiểu:**
  1. Hiểu rằng có hàng rào ở đó nhưng khi một vật thể che nhưng khi lên ảnh không thật sự che thì làm thế nào
  2. Gán vào hàng rào bởi nó là vật che.
  3. Gán vào xe con bởi nó là phần có bằng chứng hình ảnh rõ ràng theo §1 — Rule 02.
- **Xử lý tạm trong lúc chờ:** Tạo issue chờ thống nhất xử lý
- **Kết quả:** Đang chờ kết quả



## Mẫu để copy

```markdown
## P-NNN

**Tóm tắt một dòng**

- **Loại:** Guideline chưa nói tới | Guideline mơ hồ | Guideline mâu thuẫn | Pain point công cụ
- **Mục guideline:** §
- **Người phát hiện:** @ · dd/mm/yyyy
- **Link CVAT:** (bỏ trống nếu không có)
  - https://…/tasks/<id>/jobs/<id>?frame=<n> — frame này có gì
- **Mô tả:**
- **Các cách hiểu:** (với pain point công cụ thì ghi **Hướng đang cân nhắc:**)
  1.
  2.
- **Xử lý tạm trong lúc chờ:**
- **Kết quả:** 🔴 Mở
```

Nhớ thêm một dòng vào bảng **Danh sách** ở đầu file.