---
title: "Tuần 11: Nhật ký làm việc"
date: 2026-07-07
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu Tuần 11

- Triển khai các hệ thống phân phối tải lượng truy cập đàn hồi và mở rộng quy mô theo chiều ngang tự động[cite: 10].
- Bảo vệ các tầng xử lý khỏi các đợt tăng đột biến lượng truy cập người dùng[cite: 10].
- Cấu hình các trình kiểm tra sức khỏe (health-checks) tự động giúp cô lập và thay thế các nút tính toán không khỏe mạnh ngay lập tức[cite: 10].

### Các nhiệm vụ đã thực hiện trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Thiết lập một Launch Template bất biến chỉ định chính xác các hệ thống AMI, kích thước block và các security groups[cite: 10]. | 10/08/2026 | 10/08/2026 | EC2 Launch Templates |
| 2 | Xây dựng một Elastic Load Balancer (ELB) để phân phối lưu lượng truy cập đến một cách thông minh trên nhiều vùng sẵn sàng[cite: 10]. | 11/08/2026 | 11/08/2026 | Application Load Balancer |
| 3 | Cấu hình các Target Groups liên kết với các đường dẫn giám sát HTTP chủ động để xác minh trạng thái nhịp đập hệ thống[cite: 10]. | 12/08/2026 | 12/08/2026 | Target Group Configs |
| 4 | Thiết lập một Auto Scaling Group (ASG) được giao nhiệm vụ duy trì các ranh giới sức khỏe của nhóm máy chủ[cite: 10]. | 13/08/2026 | 13/08/2026 | ASG Core Documentation |
| 5 | Thực hiện các mô phỏng kiểm thử áp lực (stress-testing) bằng cách làm tràn ngập các điểm đi vào để xác minh các điều chỉnh auto-scaling của target tracking[cite: 10]. | 14/08/2026 | 14/08/2026 | Apache Bench Tools |

### Kết quả đạt được trong Tuần 11

- Loại bỏ các lỗ hổng điểm lỗi đơn nhất (single-point-of-failure) bằng cách triển khai các runtime ứng dụng trên nhiều Vùng sẵn sàng[cite: 10].
- Triển khai các số liệu theo dõi mục tiêu (target tracking) để tự động cấp phát thêm dung lượng tính toán khi lưu lượng tăng vọt[cite: 10].
- Bảo vệ các backend cơ sở dữ liệu khỏi việc xử lý các lượt nhập lỗi bằng cách giảm tải các bắt tay SSL/TLS lên các bộ cân bằng tải biên[cite: 10].
- Cấu hình các cơ chế tự chữa lành (self-healing) giúp phát hiện các instance bị rớt và tự động sinh ra các nút thay thế[cite: 10].
- Đạt được các cấu hình độ trễ (latency profiles) ổn định trong suốt các đợt thử nghiệm mô phỏng dữ liệu khối lượng lớn[cite: 10].

### Kế hoạch tuần tới

- Thực hiện một đợt kiểm toán bảo mật toàn diện và biên dịch các ma trận hiển thị mối đe dọa trung tâm.
- Kích hoạt AWS Security Hub và chạy các quy trình dọn dẹp môi trường cuối cùng trước khi hoàn thành dự án[cite: 6, 8].