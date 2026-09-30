## **Bước 1 — Xác định Entity, Attribute, Khóa chính**

| Entity | Attribute cần lưu | Khóa chính (PK) đề xuất |
| ----- | ----- | ----- |
| HOI\_VIEN | MaHV, HoTen, SoDienThoai, NgayDangKy | MaHV |
| BUOI\_TAP | MaBuoiTap, NgayTap, GioTap, TenHLV, MaHV\_FK | MaBuoiTap |

## **Bước 2 — Vẽ quan hệ bằng ký hiệu Chân quạ**
[ERD](https://drive.google.com/file/d/14nXabtSITAH5zQp4XSufZR6VfUO6HR7d/view?usp=sharing) 

## **Bước 3 — Chuẩn hóa dữ liệu** 

- Cột **SoDienThoai** của HV01 đang vi phạm chuẩn 1NF \- 1 ô chứa nhiều giá trị  
- HOI\_VIEN: 

| MaHV | HoTen | NgayDangKy |
| :---: | :---: | :---: |
| HV01  | Nguyễn Văn A  | - |
| HV02  | Trần Thị B  | - |

- SO\_DIEN\_THOAI:

| MaSoDienThoai | MaHV\_FK | SoDienThoai |
| :---: | :---: | :---: |
| SDT1 | HV01 | 0901111111  |
| SDT2 | HV01 | 0902222222  |
| SDT3 | HV02 | 0903333333  |

