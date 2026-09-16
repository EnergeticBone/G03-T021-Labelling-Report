# Nhật ký tuần 01 · 15/09 – 21/09/2026

> **File ví dụ** — tên, số liệu và link đều là giả. Tuần mới thì copy
> `[_mau-tuan.md](_mau-tuan.md)` thành `tuan-02.md`.

**Lead tuần này:** Trần Tuấn Linh @EnergeticBone 
**Dữ liệu / task CVAT:** Ảnh giao thông đô thị — [W1-SEG-G3-T1](https://cvat.note.transformerlabs.ai/tasks/194?page=1&pageSize=10)

## Thành viên và phân công


| Thành viên                            | Vị trí               | Phân công tuần này                                                     |
| ------------------------------------- | -------------------- | ---------------------------------------------------------------------- |
| Trần Tuấn Linh (@EnergeticBone)       | Lead, Reviewer       | Job 1410, chốt edge case, review job 1626, review xác suất 10% mọi job |
| Bùi Thanh Minh Hoàng (@MinhHoang-123) | Annotator            | Job 1627, 1412                                                         |
| Trần Đình Cương (@cuongcoki)          | Annotator            | Job 1629, 1416                                                         |
| Nguyễn Đăng Huân                      | Annotator            | Job 1628, 1414                                                         |
| Nguyễn Thế Anh (@thanh-vien-d)        | Reviewer · Annotator | Review job 1410, 1412, 1414, 1416; gán job 1626                        |


Nguyễn Thế Anh vừa review vừa gán, nên job 1626 do Lead review, đồng thời job 1410 sẽ do Nguyễn Thế Anh review

## Công việc


| #   | Nội dung công việc                                          | Annotator         | Reviewer        | Hoàn thành | Ghi chú                           |
| --- | ----------------------------------------------------------- | ----------------- | --------------- | ---------- | --------------------------------- |
| 1   | Job 1410 — 25 ảnh, gán theo bbox_polygon guideline          | @EnergeticBone    | @Nguyễn Thế Anh | 🟡 50%     | Tạm thời bỏ qua và chờ chốt P-001 |
| 2   | Job 1412 — 25 ảnh, gán theo bbox_polygon guideline          | @MinhHoang-123    | @Nguyễn Thế Anh |            |                                   |
| 3   | Job 1414 — 25 ảnh, gán theo bbox_polygon guideline          | @Nguyễn Đăng Huân | @Nguyễn Thế Anh |            |                                   |
| 4   | Job 1416 — 25 ảnh, gán theo bbox_polygon guideline          | @cuongcoki        | @Nguyễn Thế Anh |            |                                   |
| 5   | Job 1626 — 25 ảnh, gán theo semantic segmentation guideline | @Nguyễn Thế Anh   | @EnergeticBone  | ⬜ 0%       |                                   |
| 6   | Job 1627 — 25 ảnh, gán theo semantic segmentation guideline | @MinhHoang-123    | @EnergeticBone  | ⬜ 0%       |                                   |
| 7   | Job 1628 — 25 ảnh, gán theo semantic segmentation guideline | @Nguyễn Đăng Huân | @EnergeticBone  | 🟡 5%      | Tạm thời bỏ qua và chờ chốt P-002 |
| 8   | Job 1629 — 25 ảnh, gán theo semantic segmentation guideline | @Trần Đình Cương  | @EnergeticBone  | ⬜ 0%       |                                   |


Mức hoàn thành: ✅ xong **và đã qua review** · 🟡 đang làm (ghi %) · ⛔ bị chặn (ghi lý do) · ⬜ chưa bắt đầu

## Tổng kết

- Đã gán: 425 / 1.250 ảnh (34%)
- Qua review lần đầu: 
- Edge case mới: P-001, P-002



## Vướng mắc

- P-001 (Các xe nằm gần nhau quá dày đặc): chưa chốt nên job 1410 phải dừng. Chờ họp bàn ra cách giải quyết
- P-002 (Xe bị che khuất bởi hàng rào): chưa chốt nên job 1628 phải dừng. Chờ họp bàn ra cách giải quyết.



## Kế hoạch tuần 02

