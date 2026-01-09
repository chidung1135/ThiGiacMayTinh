LAB 1: XỬ LÝ ẢNH VỚI THƯ VIỆN PILLOW VÀ OPENCV

#1. Mục tiêu
#Làm quen với các thao tác cơ bản trên ảnh kỹ thuật số như: hiển thị ảnh, cắt ảnh (cropping), tách kênh màu.
#Hiểu rõ sự khác biệt về cấu trúc dữ liệu và cơ chế xử lý ảnh giữa hai thư viện Pillow (PIL) và OpenCV (cv2).
#Thực hành chuyển đổi không gian màu phổ biến: BGR, RGB và Grayscale.
#2. Công cụ sử dụng
#Ngôn ngữ: Python 3.x
#Thư viện:
#Pillow (PIL): Xử lý ảnh cơ bản, thao tác trực quan.
#opencv-python (cv2): Xử lý ảnh dưới dạng mảng đa chiều, tốc độ cao.
#numpy: Quản lý và thao tác ma trận điểm ảnh.
#matplotlib: Hiển thị ảnh và kết quả trực quan.
#3. Nội dung thực hiện
# Phần 1: Xử lý ảnh bằng Pillow (PIL)
#Các thao tác được thực hiện trong file '2.1.1_Images_with_python_library_PIL.ipynb':
1.Load Image
Sử dụng Image.open() để đọc file ảnh từ thư mục.
Kiểm tra các thuộc tính cơ bản của ảnh như size, mode.
2.Transform(Grayscale)
Chuyển ảnh màu sang ảnh xám bằng ImageOps.grayscale().
3.Color Channels
Tách ba kênh màu Red, Green, Blue bằng phương thức split().
Hiển thị từng kênh màu riêng biệt.
4.NumPy Integration
Chuyển đối tượng ảnh PIL sang mảng NumPy.
Trích xuất và kiểm tra giá trị cường độ pixel tại các tọa độ cụ thể.
# Phần 2: Xử lý ảnh bằng OpenCV
Các thao tác được thực hiện trong file '2.1.2_Images_with_python_library_CV.ipynb':
1.Cơ chế màu BGR
Đọc ảnh bằng cv2.imread() (mặc định theo thứ tự màu BGR).
Chuyển đổi sang RGB bằng cv2.cvtColor() để hiển thị chính xác trên Matplotlib.
2.Grayscale
Chuyển ảnh màu sang ảnh xám bằng cv2.COLOR_BGR2GRAY.
3.Thao tác mảng (Indexing / Slicing)
Cắt lấy nửa trên hoặc nửa bên trái của ảnh bằng thao tác slicing.
4.Tách kênh màu
Trích xuất từng kênh màu riêng lẻ bằng cách đặt các kênh còn lại về 0.
5.Lưu trữ ảnh
Xuất ảnh sau xử lý ra file .jpg bằng cv2.imwrite().


