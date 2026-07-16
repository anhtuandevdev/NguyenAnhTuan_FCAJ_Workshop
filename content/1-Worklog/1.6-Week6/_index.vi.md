---
title: "Nhật ký công việc Tuần 6"
date: 2026-05-22
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu Tuần 6

- Triển khai các thực thể tính toán (compute instances) bên trong các phân vùng riêng tư để mô phỏng các điểm cuối cảm biến ảo của nhà thông minh.
- Xây dựng các nút logic thực thi để biên soạn nhật ký đo lường từ xa (telemetry logs) giả lập đại diện cho các chỉ số thiết bị.
- Xác nhận các đường truyền liên lạc đầu-cuối ổn định từ các thực thể riêng tư bị cô lập ra ngoài ranh giới internet.

### Các tác vụ đã thực hiện trong tuần

| Ngày | Công việc cụ thể | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Cấp phát các nút tính toán ảo bằng cách sử dụng các thực thể Amazon Linux tiêu chuẩn được triển khai trong các subnet riêng tư. | 22/05/2026 | 22/05/2026 | Hồ sơ khởi tạo EC2 |
| 2 | Viết các tập lệnh tạo dữ liệu đo lường từ xa mô phỏng các mức điện áp, mức tăng vọt công suất và trạng thái cảm biến ảo. | 23/05/2026 | 23/05/2026 | Lập trình Node.js |
| 3 | Đính kèm các EC2 Instance Profiles chuyên dụng để cấp quyền liên lạc an toàn rõ ràng cho các máy ảo nội bộ. | 24/05/2026 | 24/05/2026 | Hướng dẫn AWS Instance Profile |
| 4 | Xác minh các đường dẫn định tuyến từ hệ thống xử lý nội bộ ra các địa chỉ công cộng thông qua NAT Gateway. | 25/05/2026 | 25/05/2026 | Công cụ chẩn đoán mạng |
| 5 | Kiểm toán các luồng thực thi bằng nhật ký giám sát CloudWatch để phát hiện các sự cố sụt giảm đường truyền hoặc lỗi tập lệnh. | 26/05/2026 | 26/05/2026 | Cẩm nang CloudWatch Logs |

### Kết quả đạt được trong Tuần 6

- Cấu hình thành công các nút tính toán cô lập có khả năng phát dữ liệu luồng mà không để lộ các điểm truy cập công cộng nguy hiểm ra bên ngoài.
- Loại bỏ các biến bí mật (secrets) được mã hóa cứng có rủi ro cao khỏi các thư mục ứng dụng bằng cách sử dụng cơ chế cấp mã token theo lập trình.
- Xác thực thành công các kết nối truyền phát thời gian thực từ bên trong các phân vùng cô lập ra các bộ thu mục tiêu công cộng.
- Đảm bảo các hành vi xử lý dữ liệu đo lường từ xa ổn định với tỷ lệ sụt giảm đường ống runtime bằng 0.
- Hoàn thành thiết lập môi trường nền tảng cần thiết cho các khối lượng công việc thu thập dữ liệu.

### Kế hoạch cho tuần tiếp theo

- Thiết lập các tầng lưu trữ cấu trúc bền vững để tổng hợp các tệp theo dõi lịch sử của nhà thông minh.
- Cấu hình các bucket tài nguyên bằng dịch vụ Amazon Simple Storage Service (S3).