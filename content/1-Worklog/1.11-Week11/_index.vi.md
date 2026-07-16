---
title: "Nhật ký công việc Tuần 11"
date: 2026-06-26
weight: 11
chapter: false
pre: " <b> 1.11. </b> "
---

### Mục tiêu Tuần 11

- Triển khai các hệ thống tự động mở rộng theo chiều ngang và phân phối cân bằng tải lưu lượng linh hoạt.
- Bảo vệ các tầng xử lý dữ liệu chống lại sự gia tăng đột biến của lưu lượng truy cập từ người dùng.
- Cấu hình các kiểm tra trạng thái tự động (automated health-checks) giúp cô lập và thay thế các nút tính toán lỗi ngay lập tức.

### Các tác vụ đã thực hiện trong tuần

| Ngày | Công việc cụ thể | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Xây dựng Mẫu khởi tạo (Launch Template) bất biến, chỉ định chính xác các hệ thống AMI, kích thước block và các nhóm bảo mật (security groups). | 26/06/2026 | 26/06/2026 | Mẫu khởi tạo EC2 |
| 2 | Xây dựng bộ cân bằng tải Elastic Load Balancer (ELB) để phân chia thông minh lưu lượng truy cập đến trên nhiều phân vùng sẵn sàng (Availability Zones). | 27/06/2026 | 27/06/2026 | Application Load Balancer |
| 3 | Cấu hình Target Groups liên kết với các đường dẫn giám sát HTTP chủ động để xác thực trạng thái nhịp tim của hệ thống. | 28/06/2026 | 28/06/2026 | Cấu hình Target Group |
| 4 | Thiết lập Nhóm tự động mở rộng Auto Scaling Group (ASG) với nhiệm vụ duy trì các ranh giới tình trạng sức khỏe của nhóm máy chủ. | 29/06/2026 | 29/06/2026 | Tài liệu cốt lõi ASG |
| 5 | Tiến hành các mô phỏng kiểm thử áp lực (stress-testing) bằng cách gửi lượng lớn yêu cầu vào các điểm đầu vào nhằm xác thực các điều chỉnh tự động mở rộng theo mục tiêu theo dõi. | 30/06/2026 | 30/06/2026 | Công cụ Apache Bench |

### Kết quả đạt được trong Tuần 11

- Loại bỏ các lỗ hổng điểm lỗi đơn lẻ (single-point-of-failure) bằng cách triển khai môi trường runtime của ứng dụng trên nhiều Availability Zones.
- Triển khai các chỉ số theo dõi mục tiêu (target tracking metrics) tự động cấp phát thêm dung lượng tính toán khi lưu lượng truy cập tăng vọt.
- Bảo vệ các backend cơ sở dữ liệu khỏi việc xử lý các tiến trình bị lỗi bằng cách giảm tải các quá trình bắt tay SSL/TLS lên các bộ cân bằng tải biên.
- Cấu hình cơ chế tự phục hồi (self-healing) giúp phát hiện các sự cố sụt giảm thực thể và tự động khởi tạo các nút thay thế.
- Đạt được cấu hình độ trễ ổn định trong các thử nghiệm mô phỏng dữ liệu khối lượng lớn.

### Kế hoạch cho tuần tiếp theo

- Thực hiện kiểm toán bảo mật toàn diện và biên soạn các ma trận hiển thị mối đe dọa trung tâm.
- Kích hoạt AWS Security Hub và chạy các quy trình dọn dẹp môi trường cuối cùng trước khi hoàn thành dự án.