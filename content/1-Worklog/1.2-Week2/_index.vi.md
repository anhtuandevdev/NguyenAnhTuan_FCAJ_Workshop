---
title: "Nhật ký công việc Tuần 2"
date: 2026-04-24
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Mục tiêu Tuần 2

- Phân tích các yêu cầu kỹ thuật và nghiệp vụ cho dự án Giám sát lãng phí năng lượng nhà thông minh.
- Thiết kế sơ đồ luồng dữ liệu cấu trúc và Sơ đồ quan hệ thực thể (ERD) cho ứng dụng.
- Đề xuất kiến trúc hệ thống cloud-native sử dụng các dịch vụ quản lý của AWS.

### Các tác vụ đã thực hiện trong tuần

| Ngày | Công việc cụ thể | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Nghiên cứu các yêu cầu của dự án và lựa chọn các dịch vụ đám mây AWS cụ thể để mô phỏng các cảm biến ảo trong nhà thông minh. | 24/04/2026 | 24/04/2026 | Bản thiết kế dự án |
| 2 | Phân tích luồng nạp dữ liệu thời gian thực cho dữ liệu đo lường từ xa (telemetry), lượng tiêu thụ năng lượng và các chỉ số môi trường. | 25/04/2026 | 25/04/2026 | Sách trắng về AWS IoT |
| 3 | Sử dụng công cụ Draw.io để xây dựng và tích hợp sơ đồ kiến trúc tổng thể của hệ thống. | 26/04/2026 | 26/04/2026 | Công cụ Draw.io |
| 4 | Thiết kế Sơ đồ quan hệ thực thể (ERD) để bố trí các tập hợp dữ liệu (collections) cho lịch sử dữ liệu đo lường từ xa. | 27/04/2026 | 27/04/2026 | Hướng dẫn thiết kế DB |
| 5 | Xây dựng Sơ đồ tuần tự (Sequence Diagrams) để phác thảo các tuyến đăng ký sự kiện, phân phối tin nhắn và kích hoạt cảnh báo thời gian thực. | 28/04/2026 | 28/04/2026 | Tài liệu chuẩn UML |

### Kết quả đạt được trong Tuần 2

- Xác định các thực thể cốt lõi của hệ thống bao gồm Người dùng (Users), Cảm biến ảo (Virtual Sensors), Siêu dữ liệu thiết bị (Device Metadata) và Nhật ký cảnh báo (Alert Logs).
- Phác thảo giải pháp đa tầng kết hợp các bộ xử lý backend Node.js, schema MongoDB Atlas và cấu trúc dữ liệu AWS.
- Thiết lập luồng xử lý hướng sự kiện (event-driven), nơi các sự kiện từ cảm biến ảo được truyền phát an toàn qua các microservice vận hành.
- Hoàn thành bản thiết kế Kiến trúc hệ thống, vạch rõ các điểm nạp dữ liệu, tính toán không máy chủ (serverless) và công cụ thông báo.
- Báo cáo thiết kế kiến trúc chính thức đã được xem xét và phê duyệt bởi người hướng dẫn kỹ thuật.

### Kế hoạch cho tuần tiếp theo

- Khởi tạo tầng bảo mật bằng cách tổ chức các định danh, phân quyền và kiểm soát dịch vụ trên AWS.
- Triển khai các thực hành tốt nhất về Quản lý danh tính và truy cập của AWS (AWS IAM).