---
title: "Tuần 10: Nhật ký làm việc"
date: 2026-07-07
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Mục tiêu Tuần 10

- Xây dựng một trình lập lịch hạ tầng tự động để cắt giảm mạnh mẽ các lãng phí hóa đơn cloud runtime[cite: 3, 8].
- Tạo các logic Lambda hướng sự kiện tự động tạm dừng các hệ thống phát triển khi không hoạt động[cite: 3, 8].
- Liên kết các phân quyền của công cụ serverless một cách rõ ràng để điều phối các chuyển đổi trạng thái hạ tầng[cite: 3, 8, 10].

### Các nhiệm vụ đã thực hiện trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Viết một script tự động sử dụng bộ công cụ Boto3 Python để chuyển đổi các trạng thái hạ tầng dựa trên giá trị thẻ tài nguyên[cite: 8, 10]. | 03/08/2026 | 03/08/2026 | Python Boto3 SDK |
| 2 | Cấu hình các trình kích hoạt Amazon EventBridge Cron chính xác để khởi chạy các script tự động tại các mốc thời gian cố định[cite: 8]. | 04/08/2026 | 04/08/2026 | EventBridge Scheduling |
| 3 | Hình thành các execution roles IAM tùy chỉnh cấp cho Lambda các quyền hạn chi tiết để kích hoạt các chuyển đổi trạng thái hạ tầng[cite: 8, 10]. | 05/08/2026 | 05/08/2026 | IAM Least Privilege |
| 4 | Thực hiện kiểm thử bằng cách kích hoạt thủ công các lịch trình sự kiện và theo dõi trạng thái hệ thống qua CloudWatch[cite: 3, 8]. | 06/08/2026 | 06/08/2026 | CloudWatch Logs Engine |
| 5 | Kiểm toán các nhật ký hoạt động hóa đơn thời gian thực để đo lường mức giảm chi phí sau khi triển khai trình lập lịch[cite: 5, 8]. | 07/08/2026 | 07/08/2026 | Cost Explorer Dashboard |

### Kết quả đạt được trong Tuần 10

- Triển khai thành công một lịch trình hạ tầng không cần can thiệp thủ công (zero-touch), tự động tắt các máy thử nghiệm ngoài giờ làm việc[cite: 8].
- Giảm thiểu đáng kể chi phí vận hành hạ tầng sandbox bằng cách loại bỏ lãng phí runtime vào cuối tuần và qua đêm[cite: 8].
- Thay thế các khóa cá nhân không an toàn bằng cách định tuyến các kiểm soát điều phối qua các instance profile bản địa bảo mật[cite: 10].
- Duy trì tính linh hoạt của nhà phát triển bằng cách đảm bảo các hộp cát thử nghiệm tự động khởi động lại trước khi ca làm việc buổi sáng bắt đầu[cite: 8].
- Tạo ra một bản thiết kế tự động hóa tiết kiệm chi phí có thể tái sử dụng, dễ dàng áp dụng cho các thành phần dự án trong tương lai[cite: 8].

### Kế hoạch tuần tới

- Đưa các cơ chế co giãn ngang (horizontal elasticity) và tự động phục hồi vào tầng xử lý.
- Xây dựng các nhóm tính toán có khả năng phục hồi, cân bằng tải và tự động mở rộng sử dụng EC2 Auto Scaling Groups[cite: 10].