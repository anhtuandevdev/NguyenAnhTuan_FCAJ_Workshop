---
title: "Nhật ký công việc Tuần 10"
date: 2026-06-19
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu Tuần 10

- Xây dựng bộ lập lịch hạ tầng tự động để cắt giảm mạnh mẽ lượng chi phí đám mây lãng phí trong thời gian chạy.
- Tạo logic Lambda hướng sự kiện để tự động tạm dừng các hệ thống phát triển khi không hoạt động.
- Liên kết chặt chẽ các ủy quyền của công cụ serverless để điều phối quá trình chuyển đổi trạng thái hạ tầng.

### Các tác vụ đã thực hiện trong tuần

| Ngày | Công việc cụ thể | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Viết tập lệnh tự động sử dụng bộ công cụ Boto3 Python để chuyển đổi trạng thái hạ tầng dựa trên giá trị thẻ tài nguyên. | 19/06/2026 | 19/06/2026 | SDK Python Boto3 |
| 2 | Cấu hình các trình kích hoạt Cron Amazon EventBridge chính xác để khởi chạy các tập lệnh tự động theo các mốc lịch trình cố định. | 20/06/2026 | 20/06/2026 | Lập lịch EventBridge |
| 3 | Khởi tạo các vai trò thực thi IAM (IAM execution roles) tùy chỉnh nhằm cấp quyền chi tiết cho Lambda để kích hoạt chuyển đổi trạng thái hạ tầng. | 21/06/2026 | 21/06/2026 | Đặc quyền tối thiểu IAM |
| 4 | Tiến hành kiểm thử bằng cách kích hoạt lịch trình sự kiện thủ công và theo dõi các trạng thái hệ thống qua CloudWatch. | 22/06/2026 | 22/06/2026 | Công cụ CloudWatch Logs |
| 5 | Kiểm toán nhật ký hoạt động thanh toán theo thời gian thực để đo lường mức giảm chi phí sau khi triển khai bộ lập lịch. | 23/06/2026 | 23/06/2026 | Bảng điều khiển Cost Explorer |

### Kết quả đạt được trong Tuần 10

- Triển khai thành công lịch trình hạ tầng tự động hoàn toàn, giúp tự động tạm dừng các máy thử nghiệm ngoài giờ làm việc.
- Giảm mạnh chi phí vận hành hạ tầng môi trường sandbox bằng cách loại bỏ lãng phí thời gian chạy vào cuối tuần và qua đêm.
- Thay thế các khóa cá nhân không an toàn bằng cách định tuyến các kiểm soát điều phối qua các profile thực thể gốc an toàn.
- Duy trì sự linh hoạt của nhà phát triển bằng cách đảm bảo các môi trường sandbox thử nghiệm tự động khởi động lại trước khi ca làm việc buổi sáng bắt đầu.
- Tạo ra một bản thiết kế tự động hóa tiết kiệm chi phí có thể tái sử dụng, dễ dàng áp dụng cho các thành phần dự án trong tương lai.

### Kế hoạch cho tuần tiếp theo

- Giới thiệu các cơ chế co giãn theo chiều ngang và tự động khôi phục cho tầng xử lý dữ liệu.
- Xây dựng các nhóm tính toán có khả năng phục hồi, cân bằng tải và tự động mở rộng quy mô bằng EC2 Auto Scaling Groups.