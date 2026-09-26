## **Phần 1: Đề xuất giải pháp**

PA1: Kế thừa với Abstract Class&nbsp;

- Lớp cha: abstract class Payment&nbsp;  
- Lớp con: CreditCardPayment, EWalletPayment, BankTransferPayment extends Payment&nbsp;

PA2: Hiện thực hóa Interface kết hợp Composition / Độc lập

- Interface: interface IPayment  
- Lớp thực thi: CreditCardPayment, EWalletPayment, BankTransferPayment implements IPayment  
- Thực thể dữ liệu: PaymentTransaction

&nbsp;

## **Phần 2: Bảng so sánh trade-off**&nbsp;

| Tiêu chí | Phương án 1: Abstract Class (Payment) | Phương án 2: Interface (IPayment) thuần túy |
| :---- | :---- | :---- |
| **Tái sử dụng mã nguồn (DRY)** | Rất tốt: Thuộc tính chung (transactionId, amount,...) và các hàm dùng chung (log, validate số tiền \> 0\) được tập trung tại lớp cha. | Kém hơn: Nếu không dùng thêm Composition, các thuộc tính sẽ bị khai báo lặp lại ở từng lớp thực thi. |
| **Nguyên tắc OCP (Open/Closed)** | Tốt: Thêm phương thức thanh toán mới chỉ cần tạo lớp con mới mà không sửa lớp cha hay code xử lý cũ. | Rất tốt: Cực kỳ linh hoạt khi tích hợp với Strategy Pattern; không bị gò bó vào cây kế thừa. |
| **Tính đa hình & Mở rộng API** | Hỗ trợ phương thức trừu tượng processPayment() để mỗi lớp con tự gọi API riêng (VNPay, Momo, Stripe). | Mỗi lớp tự do implement logic gọi API của đối tác bên thứ ba mà không chịu ràng buộc trạng thái của cha. |
| **Khả năng kế thừa đa tầng** | Bị giới hạn bởi cơ chế đơn kế thừa (ở các ngôn ngữ như Java, C\#, PHP). Không thể kế thừa thêm lớp nào khác. | Linh hoạt, một class có thể implement nhiều interface (IPayment, IRefundable, ICancellable). |
| **Mức độ phức tạp thiết kế** | Đơn giản, trực quan, phù hợp trực tiếp với mô hình dữ liệu Transaction/Payment. | Cần thiết kế thêm lớp giữ dữ liệu (DTO/Entity) để tránh vi phạm DRY, tăng số lượng class. |

&nbsp;

&nbsp;

## **Phần 3 \- Triển khai thiết kế**

[Class Diagram](https://drive.google.com/file/d/179BDGq5c2vYFJ270IZ9JT0BXiThl2Ov1/view?usp=sharing)