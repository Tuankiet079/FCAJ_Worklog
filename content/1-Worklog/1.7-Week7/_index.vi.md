---
title: "Worklog Tuần 7"
date: 2026-06-15
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Mục tiêu tuần 7:
* Nghiên cứu giải pháp tăng tốc phân phối nội dung toàn cầu Amazon CloudFront (CDN) đạt độ trễ cực thấp.
* Tìm hiểu phương pháp tối ưu bộ nhớ đệm biên và các giải pháp tường lửa ứng dụng bảo vệ lớp phân phối mạng.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :--- | :--- | :--- |
| **2** | - Học nguyên lý hoạt động của kiến trúc mạng lưới phân phối nội dung Content Delivery Network (CDN) và vai trò của các điểm biên toàn cầu (Edge Locations). | 15/06/2026 | 15/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| **3** | - Nghiên cứu giải pháp bảo mật nâng cao lớp ứng dụng Web tích hợp đi kèm AWS WAF (Web Application Firewall) nhằm ngăn chặn mã độc bắn phá CDN. | 16/06/2026 | 16/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| **4** | - Khảo sát quy trình thiết lập cổng phân phối Amazon CloudFront Distribution lấy nguồn tài nguyên gốc (Origin) định vị từ S3 Bucket hoặc Load Balancer. | 17/06/2026 | 17/06/2026 | AWS CloudFront Console |
| **5** | - Nghiên cứu các quy tắc tối ưu hóa bộ nhớ đệm biên (Cache Behaviors) và thiết lập thời gian lưu trữ dữ liệu tạm thời tối ưu (TTL - Time To Live). | 18/06/2026 | 18/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| **6** | - Khảo sát các thông số kỹ thuật phân tích luồng dữ liệu trả về trong HTTP Header.<br>- Tổng rà soát lại toàn bộ chuỗi kiến thức 7 tuần nghiên cứu dịch vụ nền tảng đám mây lõi. | 19/06/2026 | 19/06/2026 |  |

### Kết quả đạt được tuần 7:
* Hiểu giải pháp công nghệ tăng tốc độ phản hồi và hiển thị giao diện ứng dụng web thông qua mạng lưới Edge Locations toàn cầu.
* Có tư duy quản lý lưu trữ bộ nhớ đệm biên, giúp tiết kiệm tối đa chi phí đường truyền băng thông cho hệ thống máy chủ gốc.
