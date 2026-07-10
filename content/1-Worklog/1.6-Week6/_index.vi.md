---
title: "Tuần 6: Nhật ký làm việc"
date: 2026-07-06
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu Tuần 6

- Triển khai các instance tính toán bên trong các phân vùng riêng tư để mô phỏng các endpoint cảm biến ảo trong nhà thông minh[cite: 3, 5].
- Xây dựng logic thực thi mã nguồn để biên dịch các log đo lường từ xa giả lập biểu thị các chỉ số thiết bị[cite: 4, 5].
- Xác nhận các đường truyền liên lạc ổn định từ đầu đến cuối từ các instance riêng tư bị cô lập ra đến biên Internet[cite: 5].

### Các nhiệm vụ đã thực hiện trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Cấp phát các nút tính toán ảo sử dụng các instance Amazon Linux tiêu chuẩn được triển khai trong các subnet riêng tư[cite: 5]. | 06/07/2026 | 06/07/2026 | EC2 Launch Profiles |
| 2 | Viết các script tạo dữ liệu telemetry mô phỏng các mức điện áp, đỉnh công suất và trạng thái cảm biến ảo[cite: 4, 5]. | 07/07/2026 | 07/07/2026 | Node.js Programming |
| 3 | Gắn các EC2 Instance Profiles chuyên dụng để cấp quyền ủy quyền liên lạc bảo mật rõ ràng cho các máy ảo nội bộ[cite: 5, 10]. | 08/07/2026 | 08/07/2026 | AWS Instance Profile Guide |
| 4 | Xác minh các đường dẫn định tuyến từ các hệ thống xử lý nội bộ ra các địa chỉ công khai thông qua NAT Gateway[cite: 5]. | 09/07/2026 | 09/07/2026 | Network Diagnostic Tools |
| 5 | Kiểm toán các luồng thực thi sử dụng log giám sát của CloudWatch để phát hiện tình trạng rớt gói tin hoặc lỗi script[cite: 5]. | 10/07/2026 | 10/07/2026 | CloudWatch Logs Manual |

### Kết quả đạt được trong Tuần 6

- Cấu hình thành công các nút tính toán độc lập phát dữ liệu stream mà không mở ra các rủi ro tiếp xúc public nguy hiểm[cite: 5].
- Loại bỏ các biến bí mật (secrets) được hardcode nguy hiểm khỏi các thư mục ứng dụng bằng cách sử dụng cấp phát token theo lập trình[cite: 10].
- Kiểm chứng các kết nối stream thời gian thực từ bên trong các vùng cô lập ra đến các bộ thu mục tiêu công khai[cite: 5].
- Đảm bảo các hành vi xử lý dữ liệu telemetry ổn định và không gặp tình trạng đứt gãy luồng xử lý tại runtime[cite: 5].
- Hoàn thành thiết lập môi trường nền tảng cần thiết cho các tác vụ thu thập dữ liệu[cite: 3, 5].

### Kế hoạch tuần tới

- Thiết lập các tầng lưu trữ cấu trúc bền vững để tổng hợp các tệp theo dõi lịch sử nhà thông minh.
- Cấu hình các bucket tài sản sử dụng Amazon Simple Storage Service (S3)[cite: 7].