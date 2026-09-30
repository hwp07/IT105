## **Bước 1 — Xác định Entity, Attribute, Khóa chính**

| Entity | Attribute cần lưu | Khóa chính (PK) đề xuất |
| ----- | ----- | ----- |
| CAN\_HO | MaCH, DienTich, SoTang | MaCH |
| HOP\_DONG\_THUE | MaHD, NgayBatDau, NgayKetThuc | MaHD |
| KHU\_VUC | MaKhuVuc, TenKhuVuc | MaKhuVuc |

## **Bước 2 — Vẽ 2 loại quan hệ** 

[**ERD**](https://drive.google.com/file/d/1XMMm89duPRxaFFte6N2btgXAjAraPbGI/view?usp=sharing)

## **Bước 3 — Chuẩn hóa dữ liệu**

- Cột TenKhuVuc vi phạm 3NF: MaKhuVuc phụ thuộc TenCH, TenKhuVuc phu thuộc MaKhuVuc \-\> MaCH \- MaKhuVuc \- TenKhuVuc  
- Bảng CAN\_HO:

| MaCH | DienTich | SoTang | MaKhuVuc\_FK |
| :---: | :---: | :---: | :---: |
| CH01 | 45 | \- | KV01 |
| CH02 | 60 | \- | KV01 |
| CH03 | 50 | \-  | KV02 |

- Bảng KHU\_VUC:

| MaKhuVuc | TenKhuVuc |
| :---: | :---: |
| KV01 | Quận 1 |
| KV02 | Quận 7 |

