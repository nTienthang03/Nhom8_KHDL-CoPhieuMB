# Nhom8_KHDL-CoPhieuMB

# Phân tích cổ phiếu MBB giai đoạn 2021–2026

## Giới thiệu
Dự án sử dụng Python để phân tích dữ liệu cổ phiếu MBB trong giai đoạn 2021–2026.

Mục tiêu của đề tài là kiểm tra một số tín hiệu giao dịch phổ biến trong thực tế, từ đó hỗ trợ nhà đầu tư ra quyết định dựa trên dữ liệu thay vì cảm tính hoặc tin đồn.

## Dữ liệu sử dụng

Dữ liệu gồm các cột:

```python
['Date', 'Open', 'High', 'Low', 'Close', 'AdjClose', 'Volume']
````

Thông tin dữ liệu:

* Số dòng: 1,338
* Từ ngày: 2021-01-04
* Đến ngày: 2026-05-21
* File dữ liệu: `data/dulieu.csv`

## Nội dung phân tích

### Q1 — Đỉnh 52 tuần

Phân tích sau khi MBB vượt đỉnh 52 tuần thì giá tiếp tục tăng hay đảo chiều.

### Q2 — Tỷ lệ ngày xanh theo tháng

Thống kê tháng nào MBB có nhiều phiên tăng giá nhất.

### Q3 — Bóng nến trên

Kiểm tra bóng nến trên dài có dự báo ngày hôm sau giảm không.

### Q4 — Đầu tháng và cuối tháng

So sánh MBB thường tăng tốt hơn vào đầu tháng hay cuối tháng.

### Q5 — Mean Reversion

Kiểm tra sau 3 phiên tăng hoặc giảm liên tiếp, MBB có xu hướng đảo chiều hay không.

## Kết quả chính

* Sau khi vượt đỉnh 52 tuần, MBB có xu hướng tăng tiếp trong nhiều trường hợp.
* Tháng 7 có tỷ lệ ngày tăng cao nhất trong dữ liệu.
* Bóng nến trên dài có liên quan đến áp lực bán nhưng tín hiệu chưa quá mạnh.
* Đầu tháng có hiệu suất nhỉnh hơn cuối tháng.
* Sau 3 phiên tăng hoặc giảm liên tiếp, hiện tượng đảo chiều chưa thật sự rõ ràng.

## Công nghệ sử dụng

* Python
* Pandas
* NumPy
* Matplotlib
* Jupyter Notebook

## Cấu trúc thư mục

```text
mbb-stock-analysis/
│
├── data/
│   └── dulieu.csv
│
├── analysis_mbb_v3.ipynb
│
├── Q1_dinh_52_tuan.png
├── Q2_ty_le_ngay_xanh.png
├── Q3_bong_nen_tren.png
├── Q4_dau_cuoi_thang.png
├── Q5_mean_reversion.png
│
└── README.md
```

## Hướng dẫn chạy

### 1. Tạo môi trường

```bash
conda create -n mbb-analysis python=3.10 -y
conda activate mbb-analysis
```

### 2. Cài thư viện

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### 3. Chạy notebook

```bash
jupyter notebook
```

Sau đó mở file:

```text
analysis_mbb_v3.ipynb
```

và chọn **Run All**.

Hoặc chạy bằng lệnh:

```bash
jupyter nbconvert --to notebook --execute analysis_mbb_v3.ipynb --output analysis_mbb_v3.out.ipynb
```

## Kết luận

Đề tài cho thấy phân tích dữ liệu có thể giúp kiểm chứng các tín hiệu giao dịch phổ biến trên cổ phiếu MBB. Tuy nhiên, không nên sử dụng một tín hiệu riêng lẻ để ra quyết định đầu tư mà cần kết hợp thêm xu hướng thị trường, khối lượng giao dịch và các yếu tố tài chính khác.

## Thành viên thực hiện

Nhóm 8 — Trường Đại học Kỹ thuật Công nghiệp Thái Nguyên

```
```
