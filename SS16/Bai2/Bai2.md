## **Bước 1 — Xác định Entity, Attribute, Khóa chính**

| Entity | Attribute cần lưu | Khóa chính (PK) đề xuất |
| ----- | ----- | ----- |
| HOC\_VIEN | MaHV, HoTen, NgaySinh | MaHV |
| KHOA\_HOC | MaKH, TenKH, SoTietHoc | MaKH |
| DON\_DK | MaHV\_FK, MaKH\_FK, DiemSo | MaHV\_FK, MaKH\_FK |

## **Bước 2 — Vẽ quan hệ qua thực thể trung gian**

[**ERD**](https://drive.google.com/file/d/1pCyR1LguUr0WOWq8JNTDQ6RQ_BuxJyPK/view?usp=sharing)

## **Bước 3 — Chuẩn hóa dữ liệu** 

- Cột **TenKH** vi phạm **2NF** \-\> `TenKH` chỉ phụ thuộc vào **`MaKH`**, chứ không phụ thuộc đầy đủ vào cả khóa ghép **`(MaHV, MaKH)`**   
    
- Bảng HOC\_VIEN:

| MaHV | HoTen | NgaySinh |
| :---- | :---- | :---- |
| HV01 |  |  |
| HV01 |  |  |

- Bảng KHOA\_HOC: 

| MaKH | TenKH | SoTietHoc |
| :---- | :---- | :---- |
| KH01 | Nhập môn Lập trình  |  |
| KH02 | Thiết kế CSDL  |  |

- Bảng DANG\_KY:

| MaHV\_FK | MaKH\_FK | DiemSo |
| :---- | :---- | :---- |
| HV01 | KH01 | 8.5 |
| HV01 | KH02 | 9.0 |
| HV02 | KH01 | 7.0 |

