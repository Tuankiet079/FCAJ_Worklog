---
title: "Worklog Tuần 6"
date: 2026-06-08
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Mục tiêu tuần 6:
* Nghiên cứu các giải pháp xây dựng hệ thống kiến trúc phân tán chịu tải lớn và đảm bảo tính sẵn sàng cao (High Availability).
* Khảo sát cơ chế điều phối lưu lượng qua bộ cân bằng tải Application Load Balancer và cụm tự động co giãn tài nguyên Auto Scaling Group.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :--- | :--- | :--- |
| **2** | - Học lý thuyết chuyên sâu về bộ cân bằng tải ứng dụng Elastic Load Balancing (ELB), tập trung vào phân hệ Application Load Balancer (ALB). | 08/06/2026 | 08/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| **3** | - Nghiên cứu tính năng giám sát sức khỏe máy chủ tự động (Health Check) và cơ chế cấu hình định hướng điều phối lưu lượng giao thức dựa trên Target Groups. | 09/06/2026 | 09/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| **4** | - Tìm hiểu nguyên lý hoạt động của cụm co giãn tài nguyên tự động thông minh dựa trên biến động phần cứng thực tế Auto Scaling Group (ASG). | 10/06/2026 | 10/06/2026 | AWS EC2/ASG Console |
| **5** | - Khảo sát cách thức thiết lập khuôn mẫu định nghĩa cấu hình máy chủ ảo tương thích Launch Template (quy định sẵn dòng tài nguyên, AMI và mã lệnh khởi tạo). | 11/06/2026 | 11/06/2026 | AWS ALB Console |
| **6** | - Nghiên cứu cơ chế cấu hình ngưỡng giới hạn quy mô hoạt động an toàn cho hệ thống máy chủ (Min, Max, Desired Capacity) và các chính sách co giãn linh hoạt (Scaling Policies). | 12/06/2026 | 12/06/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 6:
* Nắm chắc tư duy xây dựng kiến trúc hạ tầng tự động co giãn linh hoạt theo lưu lượng truy cập thực tế, tối ưu hóa chi phí đầu tư phần cứng.
* Hiểu sâu giải pháp phân phối lưu lượng luồng mạng qua bộ cân bằng tải ALB đứng trước, loại bỏ triệt độ nguy cơ sập hệ thống do lỗi đơn điểm (Single Point of Failure).
* Biết được thiết kế hạ tầng có tính sẵn sàng cao, ứng dụng các chỉ số đo đạc phần cứng làm thước đo điều phối hạ tầng tự động trên Cloud.