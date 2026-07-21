---
title: "Worklog Tuần 3"
date: 2026-05-18
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Mục tiêu tuần 3:
* Nắm vững kiến thức hạ tầng về dịch vụ lưu trữ đối tượng không giới hạn Amazon S3.
* Cấu hình các cơ chế chính sách bảo mật, phân quyền dữ liệu và tìm hiểu giải pháp lưu trữ trang web tĩnh.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu |
| :--- | :--- | :--- | :--- | :--- |
| **2** | - Tìm hiểu cấu trúc kiến trúc Object Storage của Amazon S3: Định nghĩa về thực thể dữ liệu (Object) và kho chứa (Bucket). | 18/05/2026 | 18/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| **3** | - Phân biệt đặc tính kỹ thuật và chi phí vận hành của các lớp dữ liệu lưu trữ (Storage Classes) bao gồm S3 Standard, Intelligent-Tiering, Glacier phục vụ lưu trữ lâu dài. | 19/05/2026 | 19/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| **4** | - Khảo sát quy trình quản lý tệp tin, phân cấp cấu trúc thư mục logic và cách thức đồng bộ hóa dữ liệu từ xa lên kho chứa đám mây. | 20/05/2026 | 20/05/2026 | AWS Management Console |
| **5** | - Nghiên cứu chuyên sâu các cơ chế bảo mật dữ liệu tĩnh trên Amazon S3 bao gồm: Quy tắc chặn truy cập công cộng (Block Public Access) và chính sách kiểm soát quyền hạn Bucket Policy. | 21/05/2026 | 21/05/2026 | <https://cloudjourney.awsstudygroup.com/> |
| **6** | - Khảo sát nguyên lý hoạt động của giải pháp lưu trữ và phân phối trang web tĩnh (Static Website Hosting) được tích hợp sẵn trên nền tảng Amazon S3.<br>- Thiết lập các chính sách JSON phân quyền mở rộng (ACLs) và chính sách vòng đời dữ liệu (Lifecycle Policies). | 22/05/2026 | 22/05/2026 | <https://cloudjourney.awsstudygroup.com/> |

### Kết quả đạt được tuần 3:
* Hiểu sâu kiến trúc lưu trữ dạng đối tượng đám mây, phân biệt rõ bản chất sử dụng giữa lưu trữ dạng khối (EBS) và dạng đối tượng không cấu trúc (S3).
* Xây dựng tư duy kiểm soát an toàn thông tin vững chắc, viết cấu trúc chính sách JSON phân quyền chính xác để bảo vệ kho lưu trữ dữ liệu lớn.
* Nắm vững phương pháp đưa vào vận hành, cấu hình Endpoint phân phối một trang web HTML tĩnh chạy trực tiếp an toàn trên hạ tầng dịch vụ Amazon S3.