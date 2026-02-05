# TH_NhapMonPTDuLieuHocSau

**==============LAB 04 – Data Cleansing & Feature Engineering (Titanic)=================**
Thông tin sinh viên
Họ tên: Hồng Đăng Khoa
MSSV: 21748020101805
Môn học: Nhập môn Phân tích dữ liệu & Học sâu

1. Công nghệ sử dụng
Ngôn ngữ: Python
Thư viện:
pandas
numpy
matplotlib
seaborn
Môi trường chạy: Jupyter Notebook / Google Colab
Dataset: titanic_disaster.csv

3. Mô tả cách hoạt động
Bước 1: Đọc dữ liệu
Sử dụng pandas.read_csv() để đọc file Titanic
Kiểm tra nhanh dữ liệu bằng head(), info()
Bước 2: Kiểm tra và xử lý dữ liệu thiếu
Thống kê các cột bị thiếu dữ liệu
Dùng heatmap để quan sát trực quan dữ liệu thiếu
Bước 3: Chuẩn hóa dữ liệu
Chuẩn hóa cột Sex:
male → M
female → F
Bước 4: Xử lý giá trị thiếu của Age
Phân tích độ tuổi theo từng hạng vé (Pclass)
Thay thế Age bị thiếu bằng giá trị trung bình của từng Pclass
Bước 5: Tạo nhóm độ tuổi
Tạo cột AgeGroup gồm:
Kid
Teen
Adult
Older
Bước 6: Trích xuất danh xưng trong tên
Tách danh xưng từ cột Name (Mr, Mrs, Miss, Master…)
Gom các danh xưng hiếm vào nhóm Other
Bước 7: Xử lý thông tin gia đình
Tạo cột familySize = SibSp + Parch + 1
Tạo cột Alone để xác định hành khách đi một mình hay không
Bước 8: Xử lý dữ liệu Cabin
Lấy chữ cái đầu của Cabin để tạo cột typeCabin
Giá trị thiếu được thay bằng "Unknown"

3. Kết quả
Dữ liệu sau khi xử lý không còn thiếu các cột quan trọng
Dataset được bổ sung thêm nhiều thuộc tính có ý nghĩa
Kết quả EDA cho thấy:
Nữ có tỷ lệ sống sót cao hơn nam
Hạng vé và độ tuổi ảnh hưởng đến khả năng sống sót
Dữ liệu sẵn sàng để dùng cho các bước phân tích và xây dựng mô hình học máy
4. Kết luận
Qua bài lab này, em hiểu rõ hơn về:
Quy trình làm sạch dữ liệu

Cách tạo thêm thuộc tính từ dữ liệu ban đầu

Phân tích dữ liệu bằng biểu đồ để rút ra nhận xét
