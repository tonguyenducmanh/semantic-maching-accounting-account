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

### Xác định nghiệp vụ tài khoản kế toán

Dựa vào dòng diễn giải, xác định xem nghiệp vụ thuộc nhóm nghiệp vụ nào:

Tài sản; Nợ phải trả; Vốn chủ sở hữu; Doanh thu; Chi phí; Kết quả kinh doanh

Nguyên tắc kế toán kép (Double-entry accounting): mỗi tài khoản đều có tính chất (dư nợ, dư có hoặc lưỡng tính). Từ đó mới biết được khi nào ghi nợ, khi nào ghi có



### Pipeline gợi ý tài khoản kế toán

NLU (Natural Language Understanding) mapping to ontology
(Ánh xạ NLU (hiểu ngôn ngữ tự nhiên) vào bản thể học) - (bản thể học ở đây hiểu là bản chất của 1 số tài khoản, xây dựng ra hệ thống khái niệm của từng tài khoản)

User Input: "Thu tiền khách hàng Tô Mạnh"

Information Extraction: (Hành động, Đối tượng, Loại đối tượng)

- NER: phát hiện entity ("Khách hàng", "Nhà CC") có thể sử dụng thư viện spaCy hoặc underthesea của python kết hợp với model phoBERT
- SRL: hành động ("Thu")
- Relation Extraction

Semantic Representation: Chuẩn hóa dữ liệu

- Hành động = "Thu tiền"
- Loại = "Khách hàng"

Ontology / Knowledge Base:

- 1111: Tiền VN (thu/chi)
- 131: Thu tiền KH
- 331: Trả NCC
- 334: Trả NLĐ

Semantic Matching Engine:

- Encode (embedding)
- Similarity search
- Ánh xạ diễn giải → TK

Gợi ý tài khoản Nợ/Có:

- Nợ 1111, Có 131
