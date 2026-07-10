---
title: "Tuần 7: Nhật ký làm việc"
date: 2026-07-07
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu Tuần 7

- Triển khai các kho lưu trữ đối tượng (object storage) có độ bền cao để ghi lại các dữ liệu lịch sử cảm biến thu nhận được[cite: 7].
- Nắm vững các quy định đặt tên toàn cầu (global naming) và quy ước đường dẫn trên các hồ dữ liệu đám mây (cloud data lakes)[cite: 7].
- Triển khai các quy tắc vòng đời lưu trữ (lifecycle rules) hiệu quả về chi phí để chuyển các tệp lưu trữ cũ hơn sang các tầng ngân sách thấp[cite: 3, 7].

### Các nhiệm vụ đã thực hiện trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Tạo các bucket dữ liệu dung lượng cao được cấu hình với các nhãn tên duy nhất trên toàn cầu trên Amazon S3[cite: 7]. | 13/07/2026 | 13/07/2026 | Amazon S3 Core Guide |
| 2 | Thiết lập các cấu trúc thư mục đối tượng để tổ chức các tệp thành các khối loại cảm biến chi tiết[cite: 4, 7]. | 14/07/2026 | 14/07/2026 | S3 Folder Best Practices |
| 3 | Lập trình các script nạp dữ liệu để tải các kết quả đọc JSON thô trực tiếp lên các đích đến S3 bảo mật[cite: 7]. | 15/07/2026 | 15/07/2026 | S3 API Reference |
| 4 | Triển khai các S3 Lifecycle Policies tự động cho bucket để chuyển các log telemetry cũ hơn vào các tầng lưu trữ lạnh hơn[cite: 3, 7]. | 16/07/2026 | 16/07/2026 | S3 Lifecycle Manual |
| 5 | Thực hiện các bài kiểm tra mô phỏng truy cập dữ liệu để xác định thời gian truy xuất cho các trạng thái hoạt động so với trạng thái lưu trữ[cite: 7]. | 17/07/2026 | 17/07/2026 | AWS Storage IA Testing |

### Kết quả đạt được trong Tuần 7

- Xây dựng một không gian lưu trữ đối tượng đảm bảo các cam kết về độ bền vững của dữ liệu[cite: 7].
- Áp dụng các phân vùng bucket tối ưu giúp tách biệt luồng dữ liệu theo dõi đang hoạt động khỏi kho lưu trữ tuân thủ dài hạn[cite: 7].
- Giảm thiểu các rủi ro chi phí lưu trữ tổng thể bằng cách thiết lập các đối tượng cũ chuyển đổi trực tiếp vào tầng lạnh sâu Glacier[cite: 7].
- Thắt chặt các điểm truy cập bằng cách chặn quyền xem công khai (public) trên các ranh giới tệp nhạy cảm[cite: 7].
- Chứng minh hiệu năng của điểm đến mục tiêu có khả năng mở rộng đáp ứng các kỳ vọng về khối lượng dữ liệu đã lên kế hoạch[cite: 7].

### Kế hoạch tuần tới

- Bảo vệ hồ dữ liệu log telemetry khỏi các sự cố hỏng hóc hoặc mất mát dữ liệu ngoài ý muốn.
- Triển khai các quy tắc snapshot tự động sử dụng các giải pháp quản lý AWS Backup[cite: 7].