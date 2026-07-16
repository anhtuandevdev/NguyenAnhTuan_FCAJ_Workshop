---
title: "Nhật ký công việc Tuần 7"
date: 2026-05-29
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu Tuần 7

- Triển khai các kho lưu trữ đối tượng có độ bền vững cao để ghi lại lịch sử thu thập dữ liệu từ cảm biến gửi về.
- Nắm vững các quy định đặt tên toàn cầu và quy ước đường dẫn trên các hồ dữ liệu đám mây (cloud data lakes).
- Triển khai các quy tắc vòng đời lưu trữ tối ưu chi phí để chuyển các kho lưu trữ dữ liệu cũ hơn sang các tầng có ngân sách thấp hơn.

### Các tác vụ đã thực hiện trong tuần

| Ngày | Công việc cụ thể | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Tạo các bucket dữ liệu dung lượng cao được cấu hình với các nhãn tên duy nhất trên toàn cầu trên Amazon S3. | 29/05/2026 | 29/05/2026 | Hướng dẫn cốt lõi Amazon S3 |
| 2 | Thiết lập các cấu trúc schema thư mục đối tượng để sắp xếp các tệp thành các khối loại cảm biến chi tiết. | 30/05/2026 | 30/05/2026 | Thực hành tốt nhất về thư mục S3 |
| 3 | Lập trình các tập lệnh nạp tệp để tải trực tiếp các dữ liệu đọc JSON thô lên các điểm đích S3 an toàn. | 31/05/2026 | 31/05/2026 | Tham chiếu API S3 |
| 4 | Triển khai các Chính sách vòng đời S3 (S3 Lifecycle Policies) tự động cho bucket để chuyển các nhật ký đo lường từ xa cũ sang các tầng lưu trữ lạnh hơn. | 01/06/2026 | 01/06/2026 | Cẩm nang vòng đời S3 |
| 5 | Tiến hành các kiểm tra mô phỏng truy cập dữ liệu để xác thực thời gian truy xuất cho các trạng thái hoạt động so với trạng thái lưu trữ. | 02/06/2026 | 02/06/2026 | Kiểm thử AWS Storage IA |

### Kết quả đạt được trong Tuần 7

- Xây dựng không gian làm việc lưu trữ đối tượng đảm bảo tính bền vững của dữ liệu.
- Áp dụng các phân vùng bucket được tối ưu hóa nhằm tách biệt các luồng dữ liệu theo dõi đang hoạt động khỏi kho lưu trữ tuân thủ dài hạn.
- Giảm thiểu rủi ro quá tải lưu trữ tổng thể bằng cách thiết lập các đối tượng cũ chuyển tiếp trực tiếp vào các tầng lạnh sâu Glacier.
- Thắt chặt các điểm truy cập bằng cách chặn các quyền xem công khai trên các ranh giới tệp nhạy cảm.
- Chứng minh hiệu suất điểm đích có khả năng mở rộng đáp ứng đúng các kỳ vọng về khối lượng dữ liệu đã lập kế hoạch.

### Kế hoạch cho tuần tiếp theo

- Bảo vệ các hồ nhật ký đo lường từ xa (telemetry log lakes) khỏi các sự cố hỏng hóc hoặc mất mát dữ liệu do vô tình.
- Triển khai các quy tắc sao lưu (snapshot) tự động sử dụng các giải pháp quản lý AWS Backup.