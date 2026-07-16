---
title: "Nhật ký công việc Tuần 3"
date: 2026-05-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu Tuần 3

- Thiết lập vành đai bảo mật cốt lõi sử dụng Dịch vụ Quản lý danh tính và truy cập của AWS (AWS IAM).
- Áp dụng Nguyên tắc đặc quyền tối thiểu (Principle of Least Privilege) trên các tài khoản quản trị và tài khoản vận hành.
- Triển khai quyền truy cập bảo mật theo lập trình và các token phiên tạm thời bằng cách sử dụng IAM Roles và Conditions (Điều kiện).

### Các tác vụ đã thực hiện trong tuần

| Ngày | Công việc cụ thể | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Tạo các nhóm IAM (IAM Groups) chuyên dụng để phân loại các hoạt động quản trị, phát triển và vận hành hệ thống. | 01/05/2026 | 01/05/2026 | Hướng dẫn sử dụng AWS IAM |
| 2 | Cung cấp các tài khoản người dùng quản trị IAM độc lập nhằm loại bỏ thói quen nguy hiểm là sử dụng trực tiếp tài khoản gốc (root). | 02/05/2026 | 02/05/2026 | Cẩm nang bảo mật AWS |
| 3 | Cấu hình các vai trò IAM (IAM Roles) nâng cao, kết hợp các Chính sách JSON tùy chỉnh (custom JSON Policies) với phạm vi 'Cho phép' (Allow) và 'Từ chối' (Deny) rõ ràng. | 03/05/2026 | 03/05/2026 | Tham chiếu JSON Schema |
| 4 | Nhúng các khối Điều kiện (Condition) nghiêm ngặt vào trong các chính sách dựa trên địa chỉ IP nguồn của doanh nghiệp và các khung thời gian cụ thể. | 04/05/2026 | 04/05/2026 | Điều kiện chính sách AWS |
| 5 | Kiểm thử quy trình Giả định vai trò (Assume Role) để nhận thông tin xác thực vận hành tạm thời theo thời gian thực thông qua dịch vụ AWS STS. | 05/05/2026 | 05/05/2026 | Tài liệu AWS STS |

### Kết quả đạt được trong Tuần 3

- Cô lập thành công việc gán quyền cho các nhà phát triển bằng cách nhóm các thành viên theo phạm vi nhóm thay vì phân quyền cho từng cá nhân riêng lẻ.
- Áp dụng cơ chế xác thực đa yếu tố (MFA) bảo mật cho các kênh quản trị tài khoản gốc (root account).
- Loại bỏ các thông tin xác thực tĩnh có rủi ro cao bằng cách chuyển đổi đường dẫn truy cập của con người sang các phiên sử dụng thông tin xác thực tạm thời trong thời gian ngắn.
- Thắt chặt các điểm cuối dịch vụ (service endpoints) để chỉ chấp nhận các yêu cầu thực thi trong lịch trình làm việc nghiêm ngặt của văn phòng địa phương và từ các IP được chỉ định.
- Xác nhận việc giám sát và theo dõi dấu vết vận hành bằng cách sử dụng nhật ký kiểm tra AWS CloudTrail trong các phiên kiểm thử vai trò (role testing).

### Kế hoạch cho tuần tiếp theo

- Xây dựng nền tảng mạng đám mây cốt lõi để lưu trữ an toàn các nút tính toán (computing nodes) ở phần backend.
- Thiết kế và khởi chạy môi trường Đám mây riêng ảo (VPC) đa vùng sẵn sàng (multi-AZ VPC).