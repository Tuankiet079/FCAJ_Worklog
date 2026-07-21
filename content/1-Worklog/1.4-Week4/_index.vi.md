---
title: "Worklog Tuần 4"
date: 2026-05-25
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Mục tiêu tuần 4:
* Hiểu sâu bản chất hệ thống mạng ảo riêng biệt cô lập an toàn Amazon VPC (Virtual Private Cloud).
* Thiết kế mô hình phân khu hệ thống mạng đa tầng, định tuyến luồng dữ liệu mạng diện rộng bảo mật.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :--- | :--- | :--- |
| **2** | - Tìm hiểu lý thuyết cốt lõi về Amazon VPC: Kiến trúc phân hoạch dải IP hệ thống dựa trên sơ đồ quy chuẩn CIDR Blocks. | 25/05/2026 | 25/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| **3** | - Phân biệt ranh giới logic và vai trò của hai phân khu mạng: Public Subnet (vùng kết nối trực tiếp Internet) và Private Subnet (vùng cô lập an toàn dữ liệu). | 26/05/2026 | 26/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| **4** | - Nghiên cứu cơ chế cổng kết nối mạng Internet Gateway (IGW) và cách thức thiết lập điều phối luồng dữ liệu thông qua bảng định tuyến Route Table. | 27/05/2026 | 27/05/2026 | AWS VPC Console |
| **5** | - Khảo sát giải pháp dịch địa chỉ mạng NAT Gateway nhằm cấp quyền truy cập Internet một chiều ra ngoài an toàn cho các máy chủ ẩn trong Private Subnet. | 28/05/2026 | 28/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| **6** | - Nghiên cứu phân hệ tường lửa kiểm soát gói tin đa tầng bảo vệ luồng mạng bao gồm: Network ACLs (cấp độ đường mạng Subnet) và Security Groups (cấp độ thực thể Instance). | 29/05/2026 | 29/05/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 4:
* Đạt được tư duy chuyên nghiệp trong thiết kế hạ tầng mạng đám mây doanh nghiệp (VPC Core Topology).
* Làm chủ phương pháp cấu trúc phân tách luồng mạng an toàn thành hai phân khu rõ ràng phục vụ mục đích đón nhận lưu lượng công cộng và cô lập dữ liệu nội bộ.
* Thành thạo cơ chế điều hướng giao thức, liên kết cổng mạng và thiết lập tường lửa bảo mật đa tầng kiên cố cho hệ thống.