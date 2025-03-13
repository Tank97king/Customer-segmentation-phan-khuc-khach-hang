# Customer Segmentation Using Unsupervised Learning

## 📌 Team 6
- **Đinh Thế Thành** (Team Leader)
- Trịnh Hoàng Hà
- Nguyễn Thanh Sơn
- Bùi Tuấn Đức

## 📖 Project Introduction

In the digital age, customer segmentation is an effective method that helps businesses better understand their customers. This helps optimize products, services, and marketing strategies, thereby increasing market value.

In this project, we use clustering algorithms in **Unsupervised Machine Learning** to automatically group customers based on shared characteristics. Specifically, the **K-Means** algorithm is applied for customer segmentation.

---
## 📌 Dataset
- **Filename**: `newCustomer.csv`
- **Key Data Columns**:
  - `CustomerID`: Customer ID (will be removed during preprocessing)
  - `Gender`: Customer gender
  - `Age`: Customer age
  - `Annual Income (k$)`: Annual income in thousand dollars
  - `Spending Score (1-100)`: Customer spending score (1-100)

---
## 🔧 Methodology

### 🛠 Data Preprocessing
- Check and remove null values.
- Remove the `CustomerID` column as it is not relevant for analysis.
- Convert categorical columns (`Gender`) into numeric values using **Label Encoding**.
- Normalize data using **StandardScaler** to bring values to a uniform scale.

### 📊 Data Visualization
- Use **Seaborn** distribution plots to visualize data.
- Create a heatmap to show relationships between variables.
- Apply **t-SNE** visualization to reduce dimensions and enhance interpretability.

### 🔍 Customer Clustering
- Use the **K-Means** algorithm to cluster customers based on their features.
- Determine the optimal number of clusters using the **Elbow Method**.
- Visualize clustering results in **2D and 3D scatter plots**.

---
## 🚀 How to Run the Project
### 1️⃣ Install Required Libraries
Run the following command in your terminal or notebook to install the necessary libraries:
```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

### 2️⃣ Run the Script
Open and execute the `Customer_Segmentation.py` script using Python:
```bash
python Customer_Segmentation.py
```

Alternatively, if using **Google Colab**, upload the necessary files (`Customer_Segmentation.ipynb`, `newCustomer.csv`) and execute each cell sequentially.

---
## 📈 Results
After applying **K-Means**, we identify **5 customer clusters** based on **age, income, and spending score**. The scatter plot clearly visualizes how customers are grouped.

---
## 🏁 Conclusion
Customer segmentation using **Unsupervised Machine Learning** helps businesses optimize marketing strategies and product development. The use of **Python** along with powerful libraries such as **Scikit-learn, Pandas, and Seaborn** ensures an efficient analysis and segmentation process.

---
## 📂 Related Files
- `Customer_Segmentation.py`: Main source code.
- `Customer_Segmentation.ipynb`: Jupyter Notebook (for Google Colab users).
- `newCustomer.csv`: Customer dataset.
- `README.md`: Project documentation.

🎯 **Run the project and discover customer segments now!** 🚀
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

