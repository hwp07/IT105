# **BƯỚC 1 — BẢNG LỖI PHÁT HIỆN**

| STT | Nội dung lỗi | Phân loại lỗi | Vị trí đúng / Cách khắc phục |
| ----- | ----- | ----- | ----- |
| 1 | Actor và Use Case đặt ở 2.4 Constraints | Sai vị trí IEEE 830 | Đưa Actor vào 2.3 User Classes and Characteristics, Use Case vào 2.2 Product Functions |
| 2 | ERD đặt tại 1.3 Definitions | Sai vị trí IEEE 830 | Đưa ERD vào 3.2 Functional Requirements hoặc phần mô hình dữ liệu liên quan |
| 3 | REQ-21 dùng từ "nhanh chóng" | Verifiable | Quy định thời gian phản hồi cụ thể |
| 4 | REQ-22 chưa quy định trường hợp thanh toán không đủ | Complete | Bổ sung xử lý khi thanh toán chưa đủ 100% |
| 5 | REQ-23 và REQ-24 mâu thuẫn | Consistent | Chỉ quy định một trạng thái chỉnh sửa báo giá |
| 6 | REQ-25 "có thể cân nhắc", "tùy nguồn lực" | Unambiguous | Xác định rõ yêu cầu và mức độ ưu tiên |

# **BƯỚC 2 — BẢN CHỈNH SỬA**

## **1.2 Scope**

Hệ thống hỗ trợ khách hàng doanh nghiệp đặt tour trọn gói cho nhóm từ 10 người trở lên.

## **2.2 Product Functions**

* Tạo yêu cầu đặt tour.  
* Duyệt báo giá.  
* Xác nhận thanh toán.

## **2.3 User Classes and Characteristics**

* Nhân viên đặt tour: tạo yêu cầu, duyệt báo giá và xác nhận thanh toán.  
* Điều phối viên RikkeiTravel: xử lý và cập nhật báo giá.

## **2.4 Constraints**

* Hệ thống phải tuân thủ các quy định và giới hạn kỹ thuật của nền tảng triển khai.

## **3.2 Functional Requirements**

**REQ-21:** Hệ thống phải phản hồi báo giá trong vòng 3 giây sau khi nhận yêu cầu hợp lệ.

**REQ-22:** Khi thanh toán đủ 100% giá trị hợp đồng, hệ thống phải chuyển đơn sang trạng thái "Đã xác nhận". Nếu thanh toán chưa đủ, hệ thống không được chuyển sang trạng thái này.

**REQ-23:** Sau khi khách hàng xác nhận thanh toán, báo giá bị khóa và không được phép chỉnh sửa.

**REQ-24:** Quy tắc trên được áp dụng thống nhất: chỉ được chỉnh sửa báo giá trước khi khách hàng xác nhận thanh toán.

**REQ-25**: Tính năng xuất báo giá PDF được xếp mức ưu tiên Must Have và phải được triển khai trong phiên bản hiện tại.

## **Sơ đồ ERD**

Đặt tại **3.2 Functional Requirements**, dùng để minh họa dữ liệu liên quan đến Yêu cầu đặt tour – Báo giá – Hợp đồng.

