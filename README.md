# Dự án thu thập chất lượng bụi mịn PM2.5

Hiện nay, nhiều thành phố ở Việt Nam đang phải đối mặt với vấn đề ô nhiễm không khí nghiêm trọng, đặc biệt là tại các đô thị lớn như Hà Nội và TP. Hồ Chí Minh.
Tuy nhiên, việc thiếu dữ liệu công khai và minh bạch khiến cho các nhà nghiên cứu, cơ quan quản lý gặp khó khăn trong việc phân tích nguyên nhân và đưa ra giải pháp.
Dự án này được thực hiện với mục tiêu:
Thu thập và xử lý dữ liệu chất lượng không khí (PM2.5, PM10, khí tượng).
Phân tích xu hướng biến động nồng độ bụi mịn PM2.5.
Ứng dụng mô hình học máy để dự báo nồng độ PM2.5 trong ngắn hạn.
# Công nghệ sử dụng 

GitHub Actions: Tự động hóa việc thu thập dữ liệu, đảm bảo tính minh bạch và có thể theo dõi lịch sử thay đổi
Python: Ngôn ngữ lập trình chính được sử dụng để crawl dữ liệu
CSV: Định dạng lưu trữ dữ liệu
# Cấu trúc dữ liệu

Dữ liệu được lưu trữ trong các file CSV, được cập nhật định kỳ. Bạn có thể tìm thấy dữ liệu tại thư mục result/.
# Nguyên lý hoạt động

Dự án sử dụng bot tự động để thu thập dữ liệu từ trang web iqair.com với chu kỳ 1 giờ/lần. Các thông tin được thu thập bao gồm:

Thời gian đo
Tên thành phố
Chỉ số chất lượng không khí (AQI)
Điều kiện thời tiết
Tốc độ gió
Độ ẩm
Nhiệt độ
pm25
pm10
o3
no2
so2
co
# Tần suất cập nhật

Dữ liệu được cập nhật tự động mỗi giờ thông qua GitHub Actions, đảm bảo tính liên tục và độ tin cậy của dữ liệu.
