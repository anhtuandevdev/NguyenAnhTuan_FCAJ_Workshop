---
title: "Tuần 2: Nhật ký làm việc"
date: 2026-06-08
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu Tuần 2

- Phân tích các yêu cầu kỹ thuật và nghiệp vụ cho dự án Giám sát lãng phí năng lượng Smart Home[cite: 3, 4, 5].
- Thiết kế sơ đồ luồng dữ liệu cấu trúc và Sơ đồ quan hệ thực thể (ERD) cho ứng dụng[cite: 4].
- Đề xuất kiến trúc hệ thống cloud-native sử dụng các dịch vụ quản lý (managed services) của AWS[cite: 4].

### Các nhiệm vụ đã thực hiện trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Nghiên cứu yêu cầu dự án và lựa chọn các dịch vụ đám mây AWS cụ thể để mô phỏng các cảm biến nhà thông minh ảo[cite: 4, 5]. | 08/06/2026 | 08/06/2026 | Project Blueprint |
| 2 | Phân tích luồng nạp dữ liệu (data ingestion) theo thời gian thực cho các số liệu đo lường từ xa, lượng điện tiêu thụ và môi trường[cite: 4]. | 09/06/2026 | 09/06/2026 | AWS IoT Whitepapers |
| 3 | Sử dụng Draw.io để xây dựng sơ đồ kiến trúc tổng thể tích hợp hệ thống[cite: 4]. | 10/06/2026 | 10/06/2026 | Draw.io Tool |
| 4 | Thiết kế Sơ đồ quan hệ thực thể (ERD) để bố trí các bộ sưu tập dữ liệu (collections) lưu trữ lịch sử telemetry[cite: 4]. | 11/06/2026 | 11/06/2026 | Database Design Guides |
| 5 | Phát triển Sơ đồ tuần tự (Sequence Diagrams) mô phỏng các tiến trình đăng ký sự kiện, phân phối thông điệp và kích hoạt cảnh báo thời gian thực[cite: 4]. | 12/06/2026 | 12/06/2026 | UML Standard Docs |

### Kết quả đạt được trong Tuần 2

- Định nghĩa rõ ràng các thực thể cốt lõi của hệ thống bao gồm: Người dùng, Cảm biến ảo, Siêu dữ liệu thiết bị (Device Metadata) và Nhật ký cảnh báo (Alert Logs)[cite: 4].
- Phác thảo giải pháp đa tầng kết hợp các trình xử lý backend Node.js, schema MongoDB Atlas và cấu trúc dữ liệu AWS[cite: 4, 5].
- Thiết lập luồng xử lý hướng sự kiện (event-driven), nơi các sự kiện từ cảm biến ảo được truyền phát an toàn qua các microservice[cite: 4].
- Hoàn thiện bản thiết kế Kiến trúc Hệ thống chi tiết mô tả các điểm nạp dữ liệu, tính toán serverless và công cụ thông báo[cite: 4].
- Được người hướng dẫn kỹ thuật xem xét và phê duyệt báo cáo thiết kế kiến trúc chính thức[cite: 4].

### Kế hoạch tuần tới

- Khởi tạo tầng bảo mật bằng cách tổ chức định danh, phân quyền và kiểm soát dịch vụ trên AWS.
- Triển khai các tiêu chuẩn thực hành tốt nhất cho AWS Identity and Access Management (IAM)[cite: 5].