---
title: "Tuần 5: Nhật ký làm việc"
date: 2026-06-29
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu Tuần 5

- Thiết lập ma trận quan sát tài chính doanh nghiệp để giám sát chi phí vận hành tài nguyên trên AWS[cite: 3, 5].
- Ngăn chặn việc hóa đơn đám mây tăng đột biến bằng cách áp dụng các cảnh báo ngân sách[cite: 3, 5].
- Kiểm toán các cấu hình phân bổ tài nguyên cấu trúc sử dụng các bộ lọc hóa đơn toàn diện[cite: 3, 5].

### Các nhiệm vụ đã thực hiện trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Mở giao diện AWS Billing Dashboard chính để lập bản đồ xu hướng chi tiêu đám mây hiện tại[cite: 3, 5]. | 29/06/2026 | 29/06/2026 | AWS Cost Management |
| 2 | Tạo một giới hạn mục tiêu Ngân sách Chi phí Hàng tháng (Monthly Cost Budget) nghiêm ngặt để kiểm soát các biến số chi phí vận hành[cite: 3, 5]. | 30/06/2026 | 30/06/2026 | AWS Budgets Console |
| 3 | Triển khai chỉ số giám sát Ngân sách Sử dụng (Usage Budget) kỹ thuật nhằm theo dõi số giờ chạy thực tế của các nút tính toán cảm biến ảo[cite: 5]. | 01/07/2026 | 01/07/2026 | EC2 Pricing Matrices |
| 4 | Cấu hình các quy tắc thông báo tự động tùy chỉnh gửi cảnh báo trực tiếp đến các email được chỉ định của đội ngũ[cite: 3, 5]. | 02/07/2026 | 02/07/2026 | Amazon SNS Guides |
| 5 | Xây dựng các trình kiểm tra tự động để đánh giá phạm vi tiêu thụ gói cam kết thông qua dashboard Savings Plans và Reserved Instances[cite: 5]. | 03/07/2026 | 03/07/2026 | AWS Optimization Docs |

### Kết quả đạt được trong Tuần 5

- Thiết lập các bộ lọc tài chính chủ động giúp phát hiện ngay lập tức các mô hình tiêu thụ tài nguyên bất thường[cite: 5].
- Tích hợp các trình kích hoạt cảnh báo sớm tự động, thông báo cho ban lãnh đạo kỹ thuật trước khi các chu kỳ hóa đơn vượt quá điểm chuẩn[cite: 3, 5].
- Phát hiện các instance thử nghiệm không hoạt động nhưng vẫn tồn đọng bằng cách đọc các biểu đồ giờ tính toán chính xác bên trong nhật ký sử dụng[cite: 5].
- Tối ưu hóa khối lượng công việc trong môi trường sandbox để ngăn chặn việc vô tình vượt quá phạm vi của gói Free Tier tiêu chuẩn[cite: 3, 5].
- Xác minh tính chính xác của dữ liệu thực thi ngân sách trực tiếp từ các dashboard của Billing Console[cite: 3, 5].

### Kế hoạch tuần tới

- Triển khai và kiểm thử các nút truyền phát dữ liệu ảo (data streaming nodes).
- Khởi tạo mã nguồn xử lý cảm biến ảo trên các khung tính toán linh hoạt[cite: 3, 5].