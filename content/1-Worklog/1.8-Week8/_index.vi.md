---
title: "Nhật ký công việc Tuần 8"
date: 2026-06-05
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Mục tiêu Tuần 8

- Thiết kế quy trình quản lý sao lưu tự động và tập trung để bảo vệ các kho lưu trữ dữ liệu khỏi sự cố hỏng hóc nghiêm trọng.
- Xây dựng các chính sách khôi phục sau thảm họa (disaster recovery) ánh xạ các điểm trạng thái lưu trữ tệp.
- Cấu hình các cấu trúc cảnh báo tức thời để xác nhận việc hoàn thành các tác vụ sao lưu.

### Các tác vụ đã thực hiện trong tuần

| Ngày | Công việc cụ thể | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Kích hoạt bảng điều khiển AWS Backup trung tâm để phối hợp các mô hình bảo vệ ảnh chụp nhanh (snapshot). | 05/06/2026 | 05/06/2026 | Hướng dẫn sử dụng AWS Backup |
| 2 | Xây dựng Kế hoạch sao lưu (Backup Plan) tự động chuyên dụng, lập lịch trình thời gian chụp ảnh nhanh cho các mục tiêu lưu trữ quan trọng. | 06/06/2026 | 06/06/2026 | Cẩm nang khôi phục sau thảm họa |
| 3 | Cấu hình các thùng chứa Backup Vault được mã hóa an toàn, khóa các bản ghi dữ liệu dưới các khóa bảo mật nâng cao. | 07/06/2026 | 07/06/2026 | Hướng dẫn mã hóa KMS |
| 4 | Tiến hành kiểm thử khôi phục trực tiếp trên diện rộng bằng cách tái cấu trúc các tập dữ liệu từ đầu bằng các điểm sao lưu lịch sử. | 08/06/2026 | 08/06/2026 | Kiểm thử khôi phục dữ liệu |
| 5 | Tích hợp đường ống cảnh báo bất đồng bộ bằng Amazon SNS để gửi email nhật ký hoàn thành sao lưu cho quản trị viên. | 09/06/2026 | 09/06/2026 | Trình xuất bản Amazon SNS |

### Kết quả đạt được trong Tuần 8

- Loại bỏ hoàn toàn các tác vụ thủ công tẻ nhạt bằng cách triển khai các kế hoạch lập lịch sao lưu tự động theo cơ chế thiết lập một lần.
- Xác minh các mục tiêu về tính tin cậy của dữ liệu vận hành bằng cách khôi phục thành công các tệp văn bản đã bị xóa.
- Bảo mật các bản sao chụp nhanh cơ sở dữ liệu lịch sử bằng cách sử dụng các tầng mã hóa phần cứng được quản lý.
- Thiết lập email trạng thái tức thời để thông báo cho các kỹ sư về bất kỳ sự cố dừng phân phối tập lệnh không mong muốn nào.
- Tạo tài liệu tuân thủ mạnh mẽ cho các chính sách giữ lại dữ liệu của dự án.

### Kế hoạch cho tuần tiếp theo

- Giới thiệu các chiến lược gắn nhãn nhận dạng tài nguyên trong toàn bộ quá trình triển khai.
- Tích hợp việc nhóm phân bổ theo lập trình bằng cách sử dụng AWS Resource Groups và các tiêu chí Gắn thẻ (Tagging) thống nhất.