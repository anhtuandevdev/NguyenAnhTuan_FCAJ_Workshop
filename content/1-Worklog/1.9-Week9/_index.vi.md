---
title: "Tuần 9: Nhật ký làm việc"
date: 2026-07-07
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu Tuần 9

- Triển khai một hệ thống phân cấp phân loại siêu dữ liệu (metadata) bằng cách áp dụng các thẻ (Tags) tài nguyên tùy chỉnh[cite: 8].
- Tối ưu hóa việc quản lý đối với các tài sản đám mây dàn trải bằng cách điều phối trung tâm các AWS Resource Groups[cite: 8].
- Thiết lập các liên kết theo dõi phân bổ chi phí chi tiết kết nối các báo cáo tài chính với các thành phần hệ thống cụ thể[cite: 5, 8].

### Các nhiệm vụ đã thực hiện trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Định nghĩa một schema gắn thẻ khóa-giá trị tổ chức tiêu chuẩn giúp phân tách các tài nguyên theo môi trường và mục đích[cite: 8]. | 27/07/2026 | 27/07/2026 | AWS Tagging Best Practices |
| 2 | Gắn các cờ thẻ siêu dữ liệu theo lập trình trên các máy tính toán ảo hiện có, các thực thể cơ sở dữ liệu và các không gian lưu trữ[cite: 8]. | 28/07/2026 | 28/07/2026 | AWS CLI Engine Controls |
| 3 | Xây dựng các AWS Resource Groups động dựa trên thẻ để tự động tổng hợp các thành phần dự án có liên quan[cite: 8]. | 29/07/2026 | 29/07/2026 | Resource Groups Guide |
| 4 | Cấu hình các Cost Allocation Tags tùy chỉnh để nhóm các hạng mục chi phí dự án một cách rõ ràng trong các báo cáo ngân sách[cite: 5, 8]. | 30/07/2026 | 30/07/2026 | AWS Cost Allocation Manual |
| 5 | Thực hiện các truy vấn kiểm tra để xác minh rằng các cấu phần hạ tầng mới sinh ra sẽ tự động ghi danh vào các không gian nhóm mục tiêu[cite: 8]. | 31/07/2026 | 31/07/2026 | AWS Systems Manager |

### Kết quả đạt được trong Tuần 9

- Chuẩn hóa bức tranh đa tài nguyên thành các cấu trúc logic dễ nắm bắt thông qua việc dán nhãn meta đồng nhất[cite: 8].
- Giảm bớt các chi phí quản trị bằng cách cho phép các hành động cấu hình hàng loạt trên toàn bộ các khối tài nguyên[cite: 8].
- Mở khóa độ chính xác cao trong các tóm tắt chi phí, phân tách chi phí hạ tầng theo các biến môi trường[cite: 5, 8].
- Phát hiện các volume lưu trữ bị bỏ quên và không được gắn thẻ thông qua các đợt quét kiểm kê hệ thống có mục tiêu[cite: 8].
- Thay thế việc theo dõi từng thành phần riêng lẻ bằng các góc nhìn không gian làm việc dự án thống nhất cấp cao[cite: 8].

### Kế hoạch tuần tới

- Tự động hóa các lịch trình tối ưu hóa chi phí trên các instance tính toán đang hoạt động.
- Phát triển các trình kích hoạt cron event serverless sử dụng AWS Lambda để tự động tắt các phần cứng thử nghiệm trong các giờ thấp điểm[cite: 8].