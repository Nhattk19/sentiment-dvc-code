# 📊 Sentiment Analysis Data Versioning with DVC

Dự án này minh họa cách sử dụng **Git** và **Data Version Control (DVC)** để quản lý các phiên bản của một tập dữ liệu phân tích cảm xúc (Sentiment Analysis). 

Dự án áp dụng nguyên tắc tách biệt không gian lưu trữ: 
- **Mã nguồn và tệp cấu hình (Metadata):** Lưu trữ trên GitHub (`sentiment-dvc-code`).
- **Dữ liệu thực tế (Dataset):** Lưu trữ trên đám mây tại DagsHub (`sentiment-dvc-data`).

---

## 📁 Cấu trúc thư mục

```text
sentiment-dvc/
├── .dvc/                       # Thư mục cấu hình cốt lõi của DVC
├── data/
│   └── raw/
│       ├── .gitignore          # Ẩn file csv thật khỏi Git
│       └── sentiment.csv.dvc   # File siêu dữ liệu do DVC tạo ra để theo dõi dataset
├── .dvcignore
└── README.md
