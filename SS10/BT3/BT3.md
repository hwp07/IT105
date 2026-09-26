Thứ tự công việc
1. Khách hàng gửi taoDonHang() tới App Điều Phối.
2. App Điều Phối gửi yêu cầu nhận đơn sang Điện thoại Tài xế (Async).
3. Điện thoại Tài xế phản hồi Đồng ý/Từ chối về cho App Điều Phối (Async).
4. App Điều Phối khởi tạo một bản ghi Chuyến Đi (Trip) mới (Create) — chỉ xảy ra nếu tài xế đồng ý.
5. (Chỉ ở nhánh đồng ý) Trip xác nhận tạo chuyến đi (Return).
6. App Điều Phối báo cho Khách hàng kết quả cuối cùng (Return) — luôn xảy ra dù đồng ý hay từ chối.   