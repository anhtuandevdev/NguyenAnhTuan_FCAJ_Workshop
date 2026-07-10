---
title: "Tuần 8: Nhật ký làm việc"
date: 2026-07-07
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu Tuần 8

- Thiết kế một quy trình quản lý sao lưu tự động tập trung giúp bảo vệ các kho lưu trữ dữ liệu khỏi thảm họa hỏng dữ liệu[cite: 7].
- Điều phối các chính sách phục hồi sau thảm họa (disaster recovery) lập bản đồ cho các điểm trạng thái lưu trữ tệp[cite: 7].
- Cấu hình các cấu trúc cảnh báo tức thời xác nhận việc hoàn thành các công việc sao lưu[cite: 7].

### Các nhiệm vụ đã thực hiện trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Kích hoạt bảng điều khiển AWS Backup trung tâm để điều phối các mô hình bảo vệ snapshot[cite: 7]. | 20/07/2026 | 20/07/2026 | AWS Backup User Guide |
| 2 | Xây dựng một Backup Plan tự động chuyên dụng để thiết lập các quy trình thời gian snapshot cho các mục tiêu lưu trữ quan trọng[cite: 7]. | 21/07/2026 | 21/07/2026 | Disaster Recovery Manual |
| 3 | Cấu hình các thùng chứa Backup Vault mã hóa bảo mật nhằm khóa các bản ghi dữ liệu dưới các khóa an toàn nâng cao[cite: 7]. | 22/07/2026 | 22/07/2026 | KMS Encryption Guide |
| 4 | Thực hiện các bài kiểm tra phục hồi thực tế diện rộng bằng cách tái cấu trúc các tập dữ liệu từ đầu sử dụng các điểm sao lưu lịch sử[cite: 7]. | 23/07/2026 | 23/07/2026 | Data Restoration Tests |
| 5 | Tích hợp một đường truyền cảnh báo bất đồng bộ sử dụng Amazon SNS để gửi email nhật ký hoàn thành sao lưu cho quản trị viên[cite: 7]. | 24/07/2026 | 24/07/2026 | Amazon SNS Publisher |

### Kết quả đạt được trong Tuần 8

- Loại bỏ hoàn toàn các tác vụ thủ công tẻ nhạt của con người bằng cách triển khai các kế hoạch lập lịch sao lưu tự động cấu hình một lần[cite: 7].
- Xác minh các mục tiêu độ tin cậy dữ liệu kinh doanh vận hành bằng cách khôi phục thành công các tệp văn bản bị xóa[cite: 7].
- Bảo vệ các bản sao snapshot cơ sở dữ liệu lịch sử sử dụng các tầng mã hóa phần cứng được quản lý[cite: 7].
- Thiết lập các email trạng thái tức thời thông báo cho các kỹ sư về bất kỳ sự tạm dừng đột xuất nào của script[cite: 7].
- Tạo lập các tài liệu tuân thủ mạnh mẽ cho các chính sách lưu trữ giữ lại dữ liệu của dự án[cite: 7].

### Kế hoạch tuần tới

- Đưa vào sử dụng các chiến lược dán nhãn định danh tài nguyên (resource labeling) trên toàn bộ triển khai.
- Tích hợp các nhóm phân bổ theo chương trình sử dụng AWS Resource Groups và các tiêu chí gắn Thẻ (Tagging) thống nhất[cite: 8].