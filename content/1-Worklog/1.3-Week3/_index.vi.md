---
title: "Tuần 3: Nhật ký làm việc"
date: 2026-06-15
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu Tuần 3

- Thiết lập vành đai bảo mật cốt lõi sử dụng AWS Identity and Access Management (IAM)[cite: 5].
- Áp dụng Nguyên tắc đặc quyền tối thiểu (Principle of Least Privilege) trên các tài khoản quản trị và vận hành[cite: 10].
- Triển khai truy cập bảo mật theo lập trình và mã phiên tạm thời sử dụng IAM Roles và Điều kiện (Conditions)[cite: 10].

### Các nhiệm vụ đã thực hiện trong tuần

| Ngày | Nhiệm vụ | Ngày bắt đầu | Ngày hoàn thành | Tài liệu tham khảo |
| --- | --- | --- | --- | --- |
| 1 | Tạo các IAM Groups chuyên biệt để phân loại các thao tác quản trị, phát triển và vận hành hệ thống[cite: 5]. | 15/06/2026 | 15/06/2026 | AWS IAM User Guide |
| 2 | Cấp phát các tài khoản IAM quản trị độc lập để loại bỏ thói quen nguy hiểm là sử dụng trực tiếp tài khoản root[cite: 5]. | 16/06/2026 | 16/06/2026 | AWS Security Manual |
| 3 | Cấu hình các IAM Roles nâng cao kết hợp các Custom JSON Policies với phạm vi 'Allow' (Cho phép) và 'Deny' (Từ chối) rõ ràng[cite: 5, 10]. | 17/06/2026 | 17/06/2026 | JSON Schema Reference |
| 4 | Nhúng các khối Điều kiện (Condition) nghiêm ngặt vào policy dựa trên địa chỉ IP nguồn của doanh nghiệp và khung thời gian cụ thể[cite: 10]. | 18/06/2026 | 18/06/2026 | AWS Policy Conditions |
| 5 | Kiểm thử quy trình Ủy quyền (Assume Role) để lấy thông tin xác thực vận hành tạm thời thời gian thực thông qua AWS STS[cite: 10]. | 19/06/2026 | 19/06/2026 | AWS STS Documentation |

### Kết quả đạt được trong Tuần 3

- Cô lập thành công việc phân quyền cho nhà phát triển bằng cách nhóm các thành viên theo phạm vi đội nhóm thay vì các cá nhân riêng lẻ[cite: 5, 10].
- Bắt buộc áp dụng cơ chế xác thực đa yếu tố (MFA) bảo mật cho các kênh quản trị root[cite: 3].
- Loại bỏ các rủi ro từ thông tin xác thực tĩnh (static credentials) bằng cách chuyển hướng truy cập của con người sang các phiên xác thực tạm thời ngắn hạn[cite: 10].
- Thắt chặt các endpoint dịch vụ để chỉ chấp nhận yêu cầu thực thi trong lịch trình làm việc nghiêm ngặt của văn phòng địa phương và các IP được chỉ định[cite: 10].
- Xác nhận các luồng vết giám sát vận hành thông qua việc kiểm tra audit log của AWS CloudTrail trong các phiên thử nghiệm role[cite: 5].

### Kế hoạch tuần tới

- Xây dựng nền tảng mạng đám mây cốt lõi để lưu trữ an toàn các nút tính toán backend.
- Thiết kế và khởi chạy môi trường Virtual Private Cloud (VPC) đa vùng sẵn sàng (Multi-AZ)[cite: 5].