## **PHẦN A — Activity Diagram**

&nbsp;

| Loại Node | Tên Node / Tác vụ | Swimlane phụ trách |
| ----- | ----- | ----- |
| Initial Node | Bắt đầu | — |
| Action | Quét mã QR | Khách hàng |
| Decision | Kiểm tra số dư (Đủ / Không đủ) | Hệ thống |
| Fork | Tách 2 nhánh song song khi Đủ số dư&nbsp; | Hệ thống |
| Action | Nhả tiền | Hệ thống |
| Action | Gửi SMS báo biến động số dư | Hệ thống |
| Join | Gộp 2 nhánh song song sau khi nhả tiền và gửi SMS&nbsp; | Hệ thống |
| Final Node | Kết thúc | — |

&nbsp;

[Activity Diagram](https://drive.google.com/file/d/1CnyS4tstNrfoRqR1oSQCgqq0FIJCPYUh/view?usp=drive_link)

&nbsp;

## **PHẦN B — Use Case Diagram**&nbsp;

&nbsp;

| Use Case A | Use Case B | Quan hệ | Giải thích logic |
| ----- | ----- | ----- | ----- |
| Rút tiền | Đăng nhập | \[include\] | Phải đăng nhập trước khi rút tiền (Bắt buộc) |
| Rút tiền | In hóa đơn giao dịch | \[extend\] | Khách hàng có thể tùy chọn in hoặc không in hóa đơn sau khi hoàn tất rút tiền (Không bắt buộc)&nbsp; |
| Rút tiền | Rút tiền tiêu chuẩn | \[generalization\] | Là một dạng chuyên biệt của Rút tiền (Kế thừa) |
| Rút tiền | Rút tiền nhanh | \[generalization\] | Là một dạng chuyên biệt của Rút tiền, cho phép rút nhanh mà không cần chọn mệnh giá (Kế thừa)&nbsp; |

&nbsp;

&nbsp;

[Use Case Diagram](https://drive.google.com/file/d/1cySaUeNbmJPeqCiVcRMxyt_ZBqP7YPly/view?usp=sharing)