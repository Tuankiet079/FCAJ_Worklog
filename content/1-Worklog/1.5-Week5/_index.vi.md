---
title: "Worklog Tuần 5"
date: 2026-06-01
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Mục tiêu tuần 5:
* Nghiên cứu dịch vụ quản lý cơ sở dữ liệu quan hệ đám mây tự động Amazon RDS.
* Áp dụng nguyên lý kiến trúc cô lập dữ liệu, thiết lập phân tách an toàn giữa tầng máy chủ và tầng lưu trữ.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :--- | :--- | :--- |
| **2** | - Khảo sát kiến trúc dữ liệu đám mây: So sánh rủi ro khi tự vận hành cơ sở dữ liệu trên máy chủ EC2 với lợi ích từ dịch vụ Managed Service của Amazon RDS. | 01/06/2026 | 01/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| **3** | - Tìm hiểu các công cụ hệ quản trị dữ liệu quan hệ được hỗ trợ rộng rãi bao gồm MySQL và PostgreSQL phục vụ hoạt động lưu trữ có cấu trúc cho ứng dụng. | 02/06/2026 | 02/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| **4** | - Nghiên cứu kiến trúc dự phòng thảm họa, đảm bảo tính sẵn sàng cao thông qua tính năng Multi-AZ Deployments và mở rộng năng lực đọc bằng cụm Read Replicas. | 03/06/2026 | 03/06/2026 | AWS RDS Console |
| **5** | - Khảo sát cơ chế nhóm dải mạng dữ liệu chuyên biệt DB Subnet Groups nhằm định vị các thực thể cơ sở dữ liệu ẩn hoàn toàn bên trong dải Private Subnet. | 04/06/2026 | 04/06/2026 | <https://cloudjourney.awsstudygroup.com/> |
| **6** | - Nghiên cứu nguyên lý thiết kế cấu hình bảo mật Security Group liên tầng: Chỉ cấp quyền gõ cửa cổng Database duy nhất cho định danh máy chủ EC2 trung gian.<br>- Tìm hiểu quy trình vận hành tự động sao lưu định kỳ (Automated Backups). | 05/06/2026 | 05/06/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 5:
* Làm chủ giải pháp thiết lập hạ tầng quản trị cơ sở dữ liệu đám mây Amazon RDS được bảo vệ cô lập tuyệt đối khỏi các mối nguy cơ từ Internet công cộng.
* Hiểu rõ nguyên lý thiết kế thắt chặt luồng dữ liệu liên tầng, ứng dụng thành công cơ chế cô lập an toàn cho tầng dữ liệu Backend.
