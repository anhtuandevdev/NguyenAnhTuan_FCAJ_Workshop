---
title: "Nhật ký công việc Tuần 4"
date: 2026-05-08
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu Tuần 4

- Thiết kế hạ tầng mạng Amazon Virtual Private Cloud (VPC) mạnh mẽ, an toàn và cô lập.
- Cô lập các thành phần giao tiếp bên ngoài với các cơ sở dữ liệu backend nội bộ giữa các Vùng sẵn sàng (AZ) khác nhau.
- Loại bỏ các lỗ hổng bảo mật phổ biến bằng cách xóa bỏ các điểm truy cập trực tiếp từ bên ngoài vào mạng riêng tư.

### Các tác vụ đã thực hiện trong tuần

| Ngày | Công việc cụ thể | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Cấp phát sơ đồ mạng lõi tùy chỉnh ban đầu sử dụng khối CIDR (Classless Inter-Domain Routing) chuyên dụng. | 08/05/2026 | 08/05/2026 | Hướng dẫn mạng VPC |
| 2 | Phân chia hạ tầng mạng đối xứng qua các tầng sẵn sàng độc lập thành các Phân vùng mạng công khai (Public Subnets) và riêng tư (Private Subnets). | 09/05/2026 | 09/05/2026 | Công cụ lập kế hoạch Subnet |
| 3 | Triển khai Cổng Internet (Internet Gateway - IGW) và thiết lập bản đồ định tuyến biên ra các luồng công khai trên bảng định tuyến. | 10/05/2026 | 10/05/2026 | Tham chiếu định tuyến AWS |
| 4 | Cấu hình một NAT Gateway có tính co giãn bên trong tầng công khai để làm cầu nối kết nối internet chiều đi cho các nút mạng riêng tư. | 11/05/2026 | 11/05/2026 | Hướng dẫn sử dụng NAT Gateway |
| 5 | Thiết lập một Điểm cuối kết nối thực thể EC2 (EC2 Instance Connect Endpoint - EICE) để thực thi các lệnh terminal trực tiếp trên bảng điều khiển mà không cần IP công cộng. | 12/05/2026 | 12/05/2026 | Tài liệu Systems Manager |

### Kết quả đạt được trong Tuần 4

- Thực thi thành công việc phân tách phân vùng mạng giúp cung cấp các cơ chế bảo vệ tính Sẵn sàng cao (High Availability).
- Cấp quyền truy cập an toàn cho các cơ sở dữ liệu riêng tư để tải xuống các gói cập nhật bảo mật bên ngoài trong khi vẫn ẩn hoàn toàn các luồng kết nối đi vào.
- Vô hiệu hóa mô hình máy chủ trung chuyển (bastion host) truyền thống kém an toàn, loại bỏ hoàn toàn các bề mặt quét mục tiêu trên cổng 22.
- Tiến hành kiểm tra chi tiết các dấu vết định tuyến và đạt hiệu suất không mất mát gói tin (0% packet loss).
- Thiết lập các kênh VPC Flow Logs cơ bản để thu thập dữ liệu theo dõi thời gian thực hướng tới các nhóm nhật ký CloudWatch (CloudWatch Log Groups).

### Kế hoạch cho tuần tiếp theo

- Xây dựng các khung quản lý chi phí và ngưỡng chi tiêu đám mây.
- Triển khai mô hình lập ngân sách tài chính chi tiết bằng bảng điều khiển AWS Budgets.