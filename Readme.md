# 📊 Phân Tích Cổ Phiếu FPT - Bài Tập Khai Phá Dữ Liệu

## 👥 Thông Tin Nhóm

| STT | Họ và Tên | MSSV | 
|-----|-----------|------|
| 1 | **Nguyễn Đức Minh** | 24022404 | 
| 2 | **Dương Lý Khánh Hạ** | 23020362 | 

**Môn học:** Khai phá và Phân tích Dữ liệu  
**Giảng viên:** [Tên giảng viên]  
**Học kỳ:** II - 2024/2025  
**Mã cổ phiếu được chọn:** **FPT** (Công ty Cổ phần FPT)

---

## 📋 Giới Thiệu Dự Án

Dự án này thực hiện phân tích toàn diện dữ liệu cổ phiếu **FPT Corporation** - một trong những công ty công nghệ hàng đầu Việt Nam. Chúng tôi phân tích:

- 📈 **Lịch sử giá** cổ phiếu 5 năm (2020-2025)
- 💰 **Các chỉ số tài chính** theo quý
- 🔍 **Mối tương quan** giữa các yếu tố tài chính và giá cổ phiếu
- 💡 **Insights và khuyến nghị** đầu tư dựa trên dữ liệu

## 🎯 Mục Tiêu Bài Tập

1. **Hiểu dữ liệu** (Data Understanding)
   - Làm quen với dữ liệu tài chính và thị trường chứng khoán
   - Áp dụng domain knowledge vào phân tích

2. **Thống kê mô tả** (Descriptive Statistics)
   - Five-number summary
   - Mean, median, variance, standard deviation
   - Skewness, kurtosis

3. **Trực quan hóa** (Data Visualization)
   - Time series plots
   - Distribution analysis
   - Correlation heatmaps

4. **Phân tích tương quan** (Correlation Analysis)
   - Pearson correlation
   - Risk factors identification
   - Statistical significance testing

## 📁 Cấu Trúc Files

```
📦 FPT_Stock_Analysis/
├── 📂 Data/
│   ├── 📊 Simplize_FPT_PriceHistory_20250315.xlsx
│   └── 📊 Simplize_FPT_FinancialIndicator_20250315.xlsx
│
├── 📂 Notebooks/
│   ├── 📓 FPT_analysis.ipynb (Original)
│   ├── 📓 FPT_analysis_improved_final.ipynb ⭐ (Recommended)
│   └── 📓 FPT_analysis_complete.ipynb
│
├── 📂 Reports/
│   ├── 📄 FPT_analysis.pdf
│   └── 📊 FPT_Analysis_Results.xlsx
│
└── 📄 README.md (this file)
```

## 🛠️ Công Nghệ & Thư Viện

### Requirements
- **Python 3.8+**
- **Jupyter Notebook/Lab**

### Thư viện Python
```python
pandas==2.2.3          # Xử lý dữ liệu
numpy==1.24.3          # Tính toán số học
matplotlib==3.7.1      # Vẽ biểu đồ
seaborn==0.12.2       # Visualization nâng cao
scipy==1.10.1         # Thống kê & kiểm định
openpyxl==3.1.2       # Đọc/ghi Excel files
```

## 🚀 Hướng Dẫn Chạy

### 1. Clone/Download Project
```bash
# Clone từ git (nếu có)
git clone [repository_url]

# Hoặc download và giải nén files
```

### 2. Cài đặt Dependencies
```bash
# Cài đặt tất cả thư viện cần thiết
pip install pandas numpy matplotlib seaborn scipy openpyxl

# Hoặc dùng requirements.txt (nếu có)
pip install -r requirements.txt
```

### 3. Chạy Jupyter Notebook
```bash
# Khởi động Jupyter
jupyter notebook

# Mở file FPT_analysis_improved_final.ipynb
# Chạy từng cell theo thứ tự (Shift + Enter)
```

### 4. Điều chỉnh đường dẫn (nếu cần)
```python
# Sửa path trong code cho phù hợp với máy của bạn
price_path = r'Your_Path\Simplize_FPT_PriceHistory_20250315.xlsx'
financial_path = r'Your_Path\Simplize_FPT_FinancialIndicator_20250315.xlsx'
```

## 📊 Kết Quả Chính

### 📈 1. Thống Kê Tổng Quan
| Chỉ số | Giá trị |
|--------|---------|
| **Giá cao nhất** | 154,300 VNĐ |
| **Giá thấp nhất** | 38,548 VNĐ |
| **Giá trung bình** | 78,715 VNĐ |
| **Độ lệch chuẩn** | 32,046 VNĐ |
| **Hệ số biến thiên** | 40.7% |

### ⚠️ 2. Chỉ Số Rủi Ro
| Risk Metric | Value |
|-------------|--------|
| **Daily VaR (95%)** | -2.30% |
| **Daily CVaR (95%)** | -3.67% |
| **Max Drawdown** | 30.8% |
| **Annualized Volatility** | 26.1% |
| **Sharpe Ratio** | 1.196 |

### 🔗 3. Top 5 Yếu Tố Tương Quan
| Rank | Yếu tố | Correlation | Ý nghĩa |
|------|--------|-------------|---------|
| 1 | **P/E Ratio** | 0.823 | *** |
| 2 | **ROA** | 0.822 | *** |
| 3 | **Vòng quay tài sản** | 0.689 | ** |
| 4 | **ROE** | 0.608 | ** |
| 5 | **Khả năng thanh toán** | 0.593 | ** |

*Chú thích: *** p<0.001, ** p<0.01, * p<0.05*

## 💡 Insights & Khuyến Nghị

### ✅ Điểm Mạnh
- 🚀 **Tăng trưởng dài hạn tốt** - Xu hướng uptrend rõ ràng
- 💼 **P/E = 20.2** - Hợp lý cho ngành công nghệ
- 📊 **ROE = 27.3%** - Hiệu quả sử dụng vốn xuất sắc
- 🏢 **Vị thế dẫn đầu** - Top IT company tại Việt Nam

### ⚠️ Rủi Ro Cần Lưu Ý
- 📉 **Volatility cao** (26.1% annualized)
- 🎢 **Biến động ngắn hạn lớn**
- 🌍 **Phụ thuộc thị trường quốc tế**

### 📈 Khuyến Nghị Đầu Tư
1. ✅ **Phù hợp cho:** Nhà đầu tư dài hạn (>1 năm)
2. 📊 **Theo dõi chỉ số:** P/E, ROE, Asset Turnover
3. 💰 **Chiến lược:** Dollar Cost Averaging (DCA)
4. ⏰ **Entry point:** Khi P/E < 20, giá < MA50

## ✅ Checklist Hoàn Thành Yêu Cầu

### Phần 1: Quan sát và hiểu dữ liệu
- [x] Thống kê mô tả (five-number summary) ✅
- [x] Mean, median, std, variance ✅
- [x] Vẽ biểu đồ biến động giá ✅
- [x] Phân tích background công ty ✅

### Phần 2: Tiền xử lý dữ liệu
- [x] Tạo bảng dữ liệu mới từ 2 bảng ✅
- [x] Tính giá TB theo quý (±14 ngày) ✅
- [x] Merge các chỉ số tài chính ✅
- [x] In 5 dòng đầu của bảng mới ✅

### Phần 3: Phân tích tương quan
- [x] Tính Pearson correlation ✅
- [x] Xác định risk factors ✅
- [x] Kiểm định ý nghĩa thống kê ✅

### Phần 4: Báo cáo
- [x] Trình bày code rõ ràng ✅
- [x] Biểu đồ có title và labels ✅
- [x] Nhận xét và insights ✅
- [x] Format ipynb/pdf ✅

## 📚 Tài Liệu Tham Khảo

1. **FPT Corporation** - Annual Report 2024
2. **SSI Research** - Vietnam IT Industry Analysis
3. **Vietstock** - Historical Trading Data
4. **Simplize** - Financial Data Platform
5. **Python Documentation** - pandas, numpy, matplotlib

## 🏆 Điểm Nổi Bật Của Bài Làm

1. **Code chất lượng cao**
   - Clean, well-commented
   - Error handling
   - Modular functions

2. **Phân tích sâu**
   - Multiple statistical tests
   - Risk metrics calculation
   - Time series analysis

3. **Visualizations đẹp**
   - Professional charts
   - Proper labeling
   - Multiple plot types

4. **Insights có giá trị**
   - Domain knowledge application
   - Practical recommendations
   - Risk-return analysis

## ⚖️ Disclaimer

> ⚠️ **Lưu ý quan trọng:** Đây là bài tập học thuật, phân tích dữ liệu lịch sử cho mục đích học tập. KHÔNG PHẢI là khuyến nghị đầu tư. Mọi quyết định đầu tư cần được cân nhắc kỹ lưỡng với tư vấn chuyên môn.


*© 2025 - Bài tập môn Khai phá và Phân tích Dữ liệu*