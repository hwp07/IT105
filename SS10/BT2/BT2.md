Lỗi 1 — Bước 2: Thực tập sinh dùng Async và tạo thêm Lifeline để kiểm tra định dạng thẻ là sai. Đây là xử lý nội bộ của chính Cổng Thanh Toán, nên phải dùng Self.

Lỗi 2 — Bước 6: sendReceiptEmail() phải là Async, vì Cổng Thanh Toán không được chờ EmailServer phản hồi. Nếu dùng Sync, luồng thanh toán có thể bị chặn khi EmailServer phản hồi chậm.

Điểm cần nhớ:
Self = xử lý nội bộ trên chính Lifeline; Sync = gọi và phải chờ; Async = gửi yêu cầu rồi đi tiếp, không mặc định có Return.