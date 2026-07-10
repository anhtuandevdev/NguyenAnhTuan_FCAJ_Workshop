---
title: "Tuần 4: Nhật ký làm việc"
date: 2026-06-22
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu Tuần 4

- Thiết kế hạ tầng mạng Amazon Virtual Private Cloud (VPC) mạnh mẽ, bảo mật và cô lập[cite: 5].
- Cô lập các thành phần giao tiếp bên ngoài (public-facing) khỏi các cơ sở dữ liệu backend nội bộ giữa các Vùng sẵn sàng (AZ) riêng biệt[cite: 5].
- Loại bỏ các lỗ hổng bảo mật phổ biến bằng cách chặn các điểm truy cập trực tiếp từ bên ngoài vào mạng nội bộ[cite: 5].

### Các nhiệm vụ đã thực hiện trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Cấp phát một phân mạng lõi tùy chỉnh ban đầu sử dụng khối CIDR (Classless Inter-Domain Routing) chuyên dụng[cite: 5]. | 22/06/2026 | 22/06/2026 | VPC Networking Guide |
| 2 | Phân chia hạ tầng mạng đối xứng qua các tầng sẵn sàng tách biệt thành các Subnet Công khai (Public) và Riêng tư (Private)[cite: 5]. | 23/06/2026 | 23/06/2026 | Subnet Planning Tools |
| 3 | Triển khai một Internet Gateway (IGW) và ánh xạ các tuyến đường biên (border routes) ra ngoài Internet thông qua các bảng định tuyến công khai[cite: 5]. | 24/06/2026 | 24/06/2026 | AWS Routing Reference |
| 4 | Cấp phát một NAT Gateway đàn hồi bên trong tầng công khai để làm cầu nối kết nối Internet chiều đi (outbound) cho các nút nội bộ[cite: 5]. | 25/06/2026 | 25/06/2026 | NAT Gateway Manual |
| 5 | Thiết lập một EC2 Instance Connect Endpoint (EICE) để thực thi các lệnh terminal trực tiếp trên console mà không cần IP công khai[cite: 5]. | 26/06/2026 | 26/06/2026 | Systems Manager Docs |

### Kết quả đạt được trong Tuần 4

- Thực hiện thành công việc phân tách mạng lớp, cung cấp các cơ chế bảo vệ Tính sẵn sàng cao (High Availability)[cite: 5].
- Cấp quyền truy cập an toàn cho các cơ sở dữ liệu riêng tư để tải xuống các gói cập nhật bảo mật đi ra ngoài trong khi giữ các đường dẫn đi vào ẩn hoàn toàn[cite: 5].
- Vô hiệu hóa các hộp biên bastion host truyền thống không an toàn, loại bỏ hoàn toàn các bề mặt quét mục tiêu trên cổng 22[cite: 5].
- Thực hiện kiểm tra toàn diện các vết định tuyến, đạt điểm số hiệu năng 0% tỷ lệ mất gói tin[cite: 5].
- Thiết lập các kênh VPC Flow Logs nền tảng để ghi lại các luồng theo dõi thời gian thực hướng về các CloudWatch Log Groups[cite: 5].

### Kế hoạch tuần tới

- Tạo lập các khung quản lý chi phí và ngưỡng chi tiêu đám mây.
- Triển khai các mô hình ngân sách chi phí tài chính chi tiết sử dụng dashboard của AWS Budgets[cite: 3, 5].