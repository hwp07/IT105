**Bước 1 — Xác định đúng vị trí IEEE 830 cho toàn bộ nội dung/sơ đồ**  

| Nội dung | Vị trí đề xuất | Đúng/Sai — vị trí đúng nếu sai |
| ----- | ----- | ----- |
| Mục A (định nghĩa "Giỏ hàng") | 3.2 Functional Requirements | Sai — đúng là 2.2 Product Functions hoặc 1.2 Scope nếu dùng để giới hạn phạm vi/khái niệm của hệ thống  |
| Mục B (3 yêu cầu chức năng) | 3.2 Functional Requirements | Đúng |
| Danh sách Actor/Use Case tổng thể | 2.3 User Classes and Characteristics (Actor) và 2.2 Product Functions (Use Case/chức năng tổng quan)  | — |
| Sơ đồ Sequence áp mã giảm giá (minh họa REQ-02) | 3.2 Function Requirements | — |

**Bước 2 — Chuẩn hóa các yêu cầu chức năng theo đặc tính vàng** 

| Mã | Đặc tính vàng bị vi phạm | Viết lại đạt chuẩn |
| ----- | ----- | ----- |
| REQ-02 | Complete | Hệ thống phải kiểm tra mã giảm giá; nếu hợp lệ và còn hạn thì áp dụng giảm giá, nếu không hợp lệ/hết hạn thì thông báo lỗi |
| REQ-03 | Verifiable | Hệ thống phải xử lý thanh toán và trả kết quả trong \<= 3 giây  |

