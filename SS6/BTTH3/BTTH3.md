## **PHẦN A — Activity Diagram**

&nbsp;

| Loại Node | Tên Node / Tác vụ | Swimlane phụ trách |
| ----- | ----- | ----- |
| Initial Node | Bắt đầu | — |
| Action | Đặt lịch khám | Bệnh nhân |
| Decision | Kiểm tra khung giờ (Còn trống / Hết chỗ) | Lễ tân |
| Fork | Tách luồng xử lý song song (khi Còn trống)&nbsp; | Lễ tân |
| Action | Xác nhận lịch khám | Lễ tân |
| Action | Gửi SMS nhắc lịch | Lễ tân |
| Join | Báo chọn khung giờ khác (khi Hết chỗ)&nbsp; | Lễ tân |
| Final Node | Kết thúc | — |

&nbsp;

[Activity Diagram](https://drive.google.com/file/d/1g-xm_PpXCaFN0QNNsfjqimmi6Cwmo-Hq/view?usp=sharing)

## **PHẦN B — Use Case Diagram**&nbsp;

&nbsp;

| Use Case A | Use Case B | Quan hệ | Giải thích logic |
| ----- | ----- | ----- | ----- |
| Đặt lịch khám | Đăng nhập | \[include\] | Phải đăng nhập trước khi đặt lịch khám (Bắt buộc) |
| Đặt lịch khám | Chọn bác sĩ chỉ định | \[extend\] | Tính năng mở rộng tùy chọn, chỉ kích hoạt khi bệnh nhân có nhu cầu&nbsp; |
| Đặt lịch khám | Đặt lịch khám thường | \[generalization\] | Là một dạng chuyên biệt của Đặt lịch khám (Kế thừa) |
| Đặt lịch khám | Đặt lịch khám ưu tiên&nbsp; | \[generalization\] | Là dạng chuyên biệt có thu thêm phụ phí&nbsp; |

&nbsp;

[Use Case](https://drive.google.com/file/d/1VUDErVW4xXap1FBJxdz2rXCeKnsko4wx/view?usp=sharing)