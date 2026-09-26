## Phần 1 — Phân biệt UI/UX

| Lỗi thuộc về UI (giao diện) | Lỗi thuộc về UX (trải nghiệm) |
|---|---|
| Nút **“Gửi yêu cầu”** và **“Hủy bỏ”** cùng màu xám nhạt, không phân biệt hành động chính/phụ. | Danh sách **15 lý do** quá dài khiến người dùng khó tìm và chọn đúng lý do, làm tăng khả năng bỏ dở. |

---

## Phần 2 — Nhận diện nguyên tắc UI vi phạm

| Hiện tượng trong tình huống | Nguyên tắc UI bị vi phạm | Vì sao |
|---|---|---|
| 4 bước thao tác cùng 1 kích cỡ chữ, không phân biệt chính-phụ | **Hierarchy** | Không tạo được thứ bậc thị giác nên người dùng khó xác định nội dung và bước quan trọng. |
| Ô nhập số lượng không phản hồi gì sau khi nhập | **Feedback** | Hệ thống không phản hồi để người dùng biết dữ liệu đã được nhận và có hợp lệ hay không. |
| Nút “Gửi yêu cầu” và “Hủy bỏ” cùng màu xám giống hệt nhau | **Hierarchy** | Không phân biệt được hành động chính và hành động phụ, dễ khiến người dùng chọn nhầm. |

---

## Phần 3 — Chọn đúng thành phần UI

| Tình huống | Thành phần UI phù hợp |
|---|---|
| Chọn 1 lý do từ danh sách 15 lựa chọn | **Dropdown List** |
| Nhập số lượng sản phẩm cần đổi/trả | **Number Input** |
| Tải lên ảnh chụp sản phẩm lỗi | **File Upload** |
| Thông báo “Gửi yêu cầu thành công” tự động biến mất sau vài giây | **Toast Notification** |

---

## Phần 4 — Ánh xạ Use Case sang UI

| Bước Use Case | UI Element |
|---|---|
| 1. Khách hàng chọn 1 lý do đổi/trả | **Dropdown List** |
| 2. Khách hàng nhập số lượng sản phẩm | **Number Input** |
| 3. Khách hàng tải lên ảnh sản phẩm lỗi | **File Upload** |
| 4. Khách hàng nhấn nút xác nhận gửi yêu cầu | **Button** |

---

## Phần 5 — Phân biệt Wireframe / Mockup / Prototype

| Mô tả | Thuật ngữ |
|---|---|
| Bản phác thảo đen trắng, chỉ có khối và chữ giả, dùng để chốt bố cục | **Wireframe** |
| Bản thiết kế tĩnh, đầy đủ màu sắc và font chữ thật, dùng để chốt thẩm mỹ | **Mockup** |
| Mockup có thêm tương tác (bấm nút chuyển màn hình), dùng để mô phỏng trải nghiệm thực tế | **Prototype** |