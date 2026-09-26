# PHÂN TÍCH TRADE-OFF BỐ CỤC BỘ LỌC SẢN PHẨM RIKKEISHOP

## Phần 1 — So sánh Trade-off

| Tiêu chí | A. Sidebar Filter | B. Top Horizontal Bar |
|---|---|---|
| **Không gian hiển thị** | Chiếm một phần chiều ngang cố định nhưng khu vực sản phẩm vẫn rộng và dễ quan sát. | Tiết kiệm chiều ngang, toàn bộ chiều rộng có thể dành cho sản phẩm. Tuy nhiên khi nhiều bộ lọc sẽ chiếm nhiều chiều cao. |
| **Khi số tiêu chí tăng** | **Dễ mở rộng** theo chiều dọc. Có thể thêm Danh mục, Giá, Size, Màu sắc... mà không làm giao diện quá rối. | **Khó mở rộng**. Nhiều tiêu chí sẽ khiến thanh lọc dài, phải xuống dòng, thu gọn hoặc mở dropdown. |
| **Thao tác nhiều điều kiện** | Người dùng nhìn thấy nhiều nhóm lọc cùng lúc → thuận tiện kết hợp nhiều điều kiện. | Người dùng có thể phải mở từng nhóm lọc → nhiều thao tác hơn khi lọc sâu. |
| **Phù hợp 50.000+ sản phẩm** | **Phù hợp** với website có nhiều tiêu chí lọc. | Phù hợp hơn khi số tiêu chí lọc ít. |
| **Nhược điểm chính** | Chiếm diện tích ngang của danh sách sản phẩm. | Khi số tiêu chí tăng, giao diện dễ trở nên dài và phức tạp. |

### → Giải pháp được chọn: A — Sidebar Filter

**Lý do:** RikkeiShop có hơn **50.000 sản phẩm** và bộ lọc gồm nhiều nhóm tiêu chí. Sidebar cho phép mở rộng bộ lọc theo chiều dọc mà không làm thanh lọc phía trên trở nên quá dài hoặc khó thao tác.

> **Trade-off:** Sidebar hy sinh một phần chiều rộng hiển thị sản phẩm để đổi lấy khả năng lọc nhiều tiêu chí và khả năng mở rộng tốt hơn.

---

# Phần 2 — Thiết kế Empty State

Khi người dùng chọn tổ hợp điều kiện không có sản phẩm, khu vực danh sách **không được để trống** mà cần hiển thị:

**[Icon minh họa]**

### Không tìm thấy sản phẩm phù hợp

*Hãy thử thay đổi hoặc xóa bớt bộ lọc để xem thêm sản phẩm.*

**[ Xóa tất cả bộ lọc ]**

### Luồng UX

**Người dùng chọn bộ lọc**

↓

**Hệ thống tìm kiếm**

↓

**0 sản phẩm**

↓

**Hiển thị Empty State**

↓

**Người dùng nhấn "Xóa tất cả bộ lọc"**

↓

**Hiển thị lại danh sách sản phẩm**

### Nội dung có thể ghi trực tiếp vào bài

> **Empty State giúp người dùng hiểu rõ nguyên nhân không có kết quả và cung cấp hành động khắc phục ngay lập tức. Nút “Xóa tất cả bộ lọc” giúp đưa người dùng trở lại danh sách sản phẩm đầy đủ, tránh tình trạng màn hình trắng khiến người dùng không biết phải làm gì tiếp theo.**

## Bản ngắn gọn để nộp

> **Chọn A – Sidebar Filter** vì phù hợp với RikkeiShop có số lượng sản phẩm lớn và nhiều tiêu chí lọc. Sidebar chiếm một phần không gian ngang nhưng có khả năng mở rộng tốt theo chiều dọc, giúp người dùng dễ kết hợp nhiều điều kiện lọc. Khi không có kết quả, hệ thống hiển thị Empty State gồm icon, thông báo **“Không tìm thấy sản phẩm phù hợp”** và nút **“Xóa tất cả bộ lọc”** để người dùng nhanh chóng quay lại danh sách sản phẩm.

## Link thiết kế Figma

[🔗 Mở thiết kế RikkeiShop trên Figma](https://www.figma.com/design/wC0v5rUPOnFijH91DSlzHN/RikkeiShop-%E2%80%94-Danh-m%E1%BB%A5c-s%E1%BA%A3n-ph%E1%BA%A9m?node-id=0-1&t=4hOD1Wk3mQ0g1eY8-1)
