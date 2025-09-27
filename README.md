## Project Nghiên cứu cách gợi ý tài khoản nợ có của chứng từ kế toán dựa vào diễn giải mà người dùng nhập liệu trên chứng từ

### Cách cài đặt các package

venv

```
python -m venv venv
source venv/bin/activate
```

install package

```
pip install -r requirements.txt
```

## Xác định nghiệp vụ tài khoản kế toán

### Kết cấu cụ thể của các loại tài khoản kế toán:

Tài sản = Nợ phải trả + Vốn chủ sở hữu

Doanh thu - Chi phí = Lợi nhuận

Trong đó:

- Tài sản: Ghi tăng bên nợ, ghi giảm bên có

- Nợ phải trả: Ghi giảm bên nợ, ghi tăng bên có

- Vốn chủ sở hữu: Ghi giảm bên nợ, ghi tăng bên có

- Doanh thu: Ghi giảm bên nợ, Ghi tăng bên có

- Chi phí: Ghi tăng bên nợ, ghi giảm bên có

- Lợi nhuận: Ghi giảm bên nợ, ghi tăng bên có

### Danh sách các nhóm tài khoản:

- Loại 1, loại 2 là tài sản

- Loại 3, loại 4 là nguồn vốn

- Loại 5, loại 7 là doanh thu, thu nhập

- Loại 6, loại 8 là chi phí

- Loại 9 xác định kết quả hoạt động kinh doanh

### Mỗi khi muốn điền tài khoản nợ, có, kế toán viên phải thực hiện 3 bước sau:

Ví dụ 1: Ngày 02/10/2025, Công ty TMDV Keto mua một máy Photocopy trị giá 50000000 đ. Công ty hẹn sẽ thanh toán chuyển khoản sau 1 tháng.

Bước 1: Xác định đối tượng kế toán và số hiệu tài khoản kế toán:

- Tài sản cố định hữu hình (Máy photocopy) (Tài sản): TK 221

- Phải trả cho người bán (Nợ phải trả): TK 331

Bước 2: Phân tích biến động tăng, giảm:

Tài sản = Nợ phải trả + Vốn chủ sở hữu

- Tài sản cố định tăng 50000000 đ (Ghi nợ)

- Phải trả cho người bán tăng 50000000 đ (Ghi có)

Bước 3: Bút toán kép (Định khoản kế toán):

- Tài khoản nợ: 221

- Tài khoản có: 331

Ví dụ 2: Ngày 01/10/2025, Nguyễn Văn Toán góp vốn đầu tư 100000000 đ vào Công ty TMDV Keto bằng tiền mặt.

Bước 1: Xác định đối tượng kế toán và số hiệu tài khoản kế toán:

- Tiền mặt (Tài sản): TK 111

- Vốn đầu tư chủ sở hữu (Vốn chủ sở hữu): TK 411

Bước 2: Phân tích biến động tăng, giảm:

Tài sản = Nợ phải trả + Vốn chủ sở hữu

- Tiền mặt tăng 100000000 đ (Ghi nợ)

- Vốn đầu tư của chủ sở hữu tăng 100000000 đ (Ghi có)

Bước 3: Bút toán kép (Định khoản kế toán):

- Tài khoản nợ: 111

- Tài khoản có: 411
