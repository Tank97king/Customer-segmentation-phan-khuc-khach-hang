# Phân Khúc Khách Hàng bằng Học Máy Không Giám Sát

## 📌 Nhóm 6
- **Đinh Thế Thành** (Nhóm trưởng)
- Trịnh Hoàng Hà
- Nguyễn Thanh Sơn
- Bùi Tuấn Đức

## 📖 Giới thiệu bài toán

Trong thời đại kỹ thuật số, việc phân khúc khách hàng là một phương pháp hiệu quả giúp các doanh nghiệp hiểu rõ hơn về khách hàng của mình. Điều này giúp tối ưu hóa sản phẩm, dịch vụ và chiến lược tiếp cận, từ đó nâng cao giá trị thị trường.

Trong dự án này, chúng ta sử dụng thuật toán phân cụm trong Học máy không giám sát để tự động nhóm khách hàng dựa trên các đặc điểm chung. Cụ thể, thuật toán **K-Means** sẽ được áp dụng để phân loại khách hàng.

---
## 📌 Dữ liệu
- **Tên tệp dữ liệu**: `newCustomer.csv`
- **Các cột dữ liệu chính**:
  - `CustomerID`: Mã khách hàng (sẽ bị loại bỏ trong quá trình xử lý)
  - `Gender`: Giới tính
  - `Age`: Tuổi khách hàng
  - `Annual Income (k$)`: Thu nhập hàng năm (nghìn USD)
  - `Spending Score (1-100)`: Điểm chi tiêu của khách hàng (1-100)

---
## 🔧 Phương pháp

### 🛠 Tiền xử lý dữ liệu
- Kiểm tra và loại bỏ giá trị null.
- Loại bỏ cột `CustomerID` vì không có ý nghĩa phân tích.
- Chuyển đổi cột phân loại (`Gender`) thành dạng số bằng Label Encoding.
- Chuẩn hóa dữ liệu bằng **StandardScaler** để đưa về cùng một thang đo.

### 📊 Hình ảnh hóa dữ liệu
- Dùng biểu đồ phân bố (**Seaborn**) để trực quan hóa dữ liệu.
- Tạo heatmap để hiển thị mối quan hệ giữa các biến.
- Dùng biểu đồ t-SNE để giảm chiều dữ liệu và trực quan hóa.

### 🔍 Phân cụm khách hàng
- Sử dụng thuật toán **K-Means** để phân nhóm khách hàng dựa trên đặc điểm.
- Dùng phương pháp "Khuỷu tay" (Elbow Method) để xác định số cụm tối ưu.
- Trực quan hóa kết quả phân cụm trên biểu đồ 2D và 3D.

---
## 🚀 Cách chạy dự án
### 1️⃣ Cài đặt các thư viện cần thiết
Chạy lệnh sau trong terminal hoặc notebook để cài đặt các thư viện cần thiết:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### 2️⃣ Chạy mã nguồn
Mở và chạy tệp `Customer_Segmentation.py` bằng Python:
```bash
python Customer_Segmentation.py
```

Hoặc nếu sử dụng Google Colab, tải lên các tệp cần thiết (`Customer_Segmentation.ipynb`, `newCustomer.csv`) và chạy từng cell theo thứ tự.

---
## 📈 Kết quả
Sau khi áp dụng phương pháp **K-Means**, chúng ta xác định được **5 cụm khách hàng** dựa trên độ tuổi, thu nhập và điểm chi tiêu. Biểu đồ phân tán hiển thị rõ ràng cách khách hàng được phân nhóm.

---
## 🏁 Kết luận
Phân khúc khách hàng bằng **Học máy không giám sát** giúp doanh nghiệp tối ưu hóa chiến lược tiếp thị và phát triển sản phẩm. Việc sử dụng Python cùng các thư viện mạnh mẽ như **Scikit-learn, Pandas, Seaborn** giúp thực hiện phân tích một cách hiệu quả.

---
## 📂 Các tệp liên quan
- `Customer_Segmentation.py`: Mã nguồn chính.
- `Customer_Segmentation.ipynb`: Notebook Jupyter (nếu sử dụng Google Colab).
- `newCustomer.csv`: Dữ liệu khách hàng.
- `README.md`: Hướng dẫn dự án.

🎯 **Hãy chạy thử và khám phá các phân khúc khách hàng!** 🚀