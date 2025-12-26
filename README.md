# 📊 Student Performance Analysis Project

[![Python](https://img.shields.io/badge/Python-3.9%2B-blue)](https://www.python.org/)
[![Status](https://img.shields.io/badge/Status-Completed-success)]()
[![License](https://img.shields.io/badge/License-MIT-green)]()

## 📝 Giới thiệu (Introduction)
Dự án này là bài tập lớn môn **Lập trình Python**, tập trung vào việc phân tích các yếu tố ảnh hưởng đến kết quả học tập của học sinh. Chương trình thực hiện trọn vẹn quy trình Khoa học dữ liệu (Data Science Pipeline) từ thu thập, làm sạch, xử lý ngoại lai (outliers) đến trực quan hóa dữ liệu.

Dữ liệu được lấy từ nguồn [Kaggle: Student Performance in Exams](https://www.kaggle.com/spscientist/students-performance-in-exams).

## 🚀 Tính năng chính (Key Features)
* **Data Loading:** Đọc dữ liệu từ CSV và hiển thị thống kê mô tả cơ bản.
* **Data Cleaning:**
    * Chuẩn hóa tên cột.
    * Xử lý dữ liệu trùng lặp.
    * Xử lý ngoại lai (Outliers) bằng phương pháp **IQR (Interquartile Range)**.
* **Feature Engineering:** Tạo cột điểm trung bình (`average_score`) và xếp loại học lực (`grade_rank`).
* **Visualization:**
    * Biểu đồ phân phối (Histogram/Boxplot).
    * Biểu đồ nhiệt tương quan (Correlation Heatmap).
    * Phân tích đa biến (Multivariate Analysis).

## 📂 Cấu trúc dự án (Project Structure)
```text
Python_Final_Project/
│
├── data/
│   ├── raw_data.csv        # Dữ liệu thô ban đầu
│   └── processed_data.csv  # Dữ liệu sạch sau khi chạy chương trình
│
├── src/                    # Mã nguồn chính (Packages)
│   ├── __init__.py
│   ├── data_loader.py      # Module đọc và kiểm tra dữ liệu
│   ├── data_cleaner.py     # Module xử lý, làm sạch và feature engineering
│   └── visualizer.py       # Module vẽ biểu đồ phân tích
│
├── main.py                 # File thực thi chính
├── requirements.txt        # Danh sách thư viện phụ thuộc
└── README.md               # Tài liệu hướng dẫn
