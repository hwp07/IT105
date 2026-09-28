# RÀ SOÁT NHANH MÀN HÌNH "YÊU CẦU ĐỔI/TRẢ HÀNG" FASTMART-ONLINE

---

## Phần 1 — Phân biệt UI/UX

| Lỗi thuộc về UI (Giao diện) | Lỗi thuộc về UX (Trải nghiệm) |
| :--- | :--- |
| Nút "Gửi yêu cầu" và "Hủy bỏ" dùng chung một màu xám nhạt với kiểu dáng giống hệt nhau, không thể hiện được cấp độ thị giác (Primary vs Secondary). | Khách hàng nhập số lượng nhưng hệ thống không đưa ra bất kỳ phản hồi hay cảnh báo lỗi nào (nhập 0 hoặc để trống), khiến họ hoang mang không biết dữ liệu đã hợp lệ chưa và dễ dẫn đến bỏ dở quy trình. |

---

## Phần 2 — Nhận diện nguyên tắc UI vi phạm

| Hiện tượng trong tình huống | Nguyên tắc UI bị vi phạm | Vì sao |
| :--- | :--- | :--- |
| **4 bước thao tác cùng 1 kích cỡ chữ, không phân biệt chính-phụ** | **Hierarchy** *(Phân cấp thị giác)* | Giao diện thiếu sự phân cấp về độ lớn, độ đậm của typography để định hướng mắt người dùng nhận biết đâu là tiêu đề bước, đâu là nội dung thao tác chính. |
| **Ô nhập số lượng không phản hồi gì sau khi nhập** | **Feedback** *(Phản hồi)* | Hệ thống không cung cấp tín hiệu xác nhận dữ liệu hợp lệ hoặc cảnh báo lỗi khi nhập sai/nhập 0, vi phạm nguyên tắc giữ cho người dùng luôn nắm bắt được trạng thái hệ thống. |
| **Nút "Gửi yêu cầu" và "Hủy bỏ" cùng màu xám giống hệt nhau** | **Clarity** *(Rõ ràng)* | Hai hành động đối nghịch (hoàn tất quy trình vs huỷ bỏ thao tác) không có sự tương phản thị giác rõ rệt, dễ gây nhầm lẫn hoặc kích hoạt thao tác sai lầm. |

---

## Phần 3 — Chọn đúng thành phần UI

| Tình huống | Thành phần UI phù hợp |
| :--- | :--- |
| Chọn 1 lý do từ danh sách 15 lựa chọn | Dropdown List (Select Menu) |
| Nhập số lượng sản phẩm cần đổi/trả | Number Stepper (Number Input) |
| Tải lên ảnh chụp sản phẩm lỗi | File Uploader (Image Picker) |
| Thông báo "Gửi yêu cầu thành công" tự động biến mất sau vài giây | Toast Notification (Snackbar) |

---

## Phần 4 — Ánh xạ Use Case sang UI

| Bước Use Case | UI Element |
| :--- | :--- |
| 1. Khách hàng chọn 1 lý do đổi/trả | Dropdown List |
| 2. Khách hàng nhập số lượng sản phẩm | Number Stepper / Number Input Field |
| 3. Khách hàng tải lên ảnh sản phẩm lỗi | File Uploader / Image Upload Area |
| 4. Khách hàng nhấn nút xác nhận gửi yêu cầu | Primary Button (CTA Button) |

---

## Phần 5 — Phân biệt Wireframe / Mockup / Prototype

| Mô tả | Thuật ngữ |
| :--- | :--- |
| Bản phác thảo đen trắng, chỉ có khối và chữ giả, dùng để chốt bố cục | **Wireframe** |
| Bản thiết kế tĩnh, đầy đủ màu sắc và font chữ thật, dùng để chốt thẩm mỹ | **Mockup** |
| Mockup có thêm tương tác (bấm nút chuyển màn hình), dùng để mô phỏng trải nghiệm thực tế | **Prototype** |