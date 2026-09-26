## **PHẦN A — Activity Diagram**

&nbsp;

| Loại Node | Tên Node / Tác vụ | Swimlane phụ trách |
| ----- | ----- | ----- |
| Initial Node | Bắt đầu | — |
| Action | Đặt đơn hàng | Khách hàng |
| Decision | Kiểm tra tồn kho (Còn hàng / Hết hàng) | Bộ phận Kho |
| Fork | Tách luồng xử lý song song (khi Còn hàng)&nbsp; | Bộ phận Kho |
| Action | Đóng gói đơn hàng | Bộ phận kho |
| Action | Gửi thông báo xuất kho | Bộ phận kho |
| Join | Báo hoàn tiền khi hết hàng | Bộ phận Kho |
| Final Node | Kết thúc | — |

&nbsp;

[Activity Diagram](https://drive.google.com/file/d/1BaYuk5z7r77zKY6SYZAe1MY2EnseuvrI/view?usp=sharing)

## **PHẦN B — Use Case Diagram**&nbsp;

&nbsp;

| Use Case A | Use Case B | Quan hệ | Giải thích logic |
| ----- | ----- | ----- | ----- |
| Đặt đơn hàng | Đăng nhập | \[include\] | Phải đăng nhập trước khi đặt đơn hàng (Bắt buộc) |
| Đặt đơn hàng | Giao hàng hoả tốc | \[extend\] | Tính năng mở rộng, chỉ kích hoạt khi khách sử dụng tính năng |
| Đặt đơn hàng | Đặt đơn hàng lẻ | \[generalization\] | Là một dạng chuyên biệt của Đặt đơn hàng (Kế thừa) |
| Đặt đơn hàng | Đặt đơn hàng sỉ | \[generalization\] | Là 1 dạng đơn chuyên biệt dành cho đơn số lượng lớn&nbsp; |

&nbsp;

[Use Case](https://drive.google.com/file/d/1o-Q7w1oHhB8Ulie25DAm8edx7pbaA6KR/view?usp=sharing)