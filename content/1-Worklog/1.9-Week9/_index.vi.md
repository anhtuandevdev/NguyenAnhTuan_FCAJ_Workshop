---
title: "Nhật ký công việc Tuần 9"
date: 2026-06-12
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu Tuần 9

- Triển khai hệ thống phân cấp phân loại siêu dữ liệu bằng cách áp dụng các Thẻ (Tags) tài nguyên tùy chỉnh.
- Tối ưu hóa việc quản lý các tài sản đám mây đang mở rộng bằng cách tổ chức các Nhóm tài nguyên AWS (AWS Resource Groups) trung tâm.
- Thiết lập các liên kết theo dõi phân bổ chi phí chi tiết, kết nối các báo cáo tài chính với các thành phần hệ thống cụ thể.

### Các tác vụ đã thực hiện trong tuần

| Ngày | Công việc cụ thể | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Xác định schema gắn thẻ key-value chuẩn của tổ chức để phân tách các tài nguyên theo môi trường và mục đích sử dụng. | 12/06/2026 | 12/06/2026 | Thực hành tốt nhất về gắn thẻ AWS |
| 2 | Gắn các cờ thẻ siêu dữ liệu theo lập trình trên các máy tính ảo, thực thể cơ sở dữ liệu và không gian lưu trữ hiện có. | 13/06/2026 | 13/06/2026 | Điều khiển công cụ AWS CLI |
| 3 | Xây dựng các AWS Resource Groups động dựa trên thẻ để tự động tập hợp các thành phần dự án có liên quan. | 14/06/2026 | 14/06/2026 | Hướng dẫn về Resource Groups |
| 4 | Cấu hình Thẻ phân bổ chi phí (Cost Allocation Tags) tùy chỉnh để nhóm các hạng mục dự án một cách rõ ràng trong các báo cáo ngân sách. | 15/06/2026 | 15/06/2026 | Cẩm nang phân bổ chi phí AWS |
| 5 | Thực thi các kiểm tra truy vấn để xác minh rằng các thành phần hạ tầng mới khởi tạo sẽ tự động tham gia vào không gian nhóm mục tiêu. | 16/06/2026 | 16/06/2026 | AWS Systems Manager |

### Kết quả đạt được trong Tuần 9

- Chuẩn hóa bối cảnh đa tài nguyên thành các cấu trúc logic có thể quét được thông qua việc gắn nhãn meta đồng nhất.
- Cắt giảm đáng kể thời gian quản trị bằng cách cho phép thực hiện các hành động cấu hình hàng loạt trên toàn bộ các khối tài nguyên.
- Đạt được độ chính xác cao trong các tóm tắt chi phí, tách biệt chi phí hạ tầng theo các biến môi trường.
- Phát hiện các phân vùng lưu trữ bị bỏ trống và không được gắn thẻ bằng cách sử dụng các quét kiểm kê hệ thống có mục tiêu.
- Thay thế việc theo dõi từng thành phần riêng lẻ rườm rà bằng các chế độ xem không gian làm việc dự án thống nhất ở cấp độ cao.

### Kế hoạch cho tuần tiếp theo

- Tự động hóa lịch trình tối ưu hóa chi phí trên các thực thể tính toán đang hoạt động.
- Phát triển các trình kích hoạt cron sự kiện không máy chủ sử dụng AWS Lambda để tự động tạm dừng phần cứng thử nghiệm trong giờ thấp điểm.