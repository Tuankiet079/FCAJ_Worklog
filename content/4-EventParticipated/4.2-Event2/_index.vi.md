---
title: "Event 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 4.2. </b> "
---


# Bài thu hoạch “FCAJ Community Day: Cloud-Native & Advanced Tech Sharing Session”

### Mục Đích Của Sự Kiện

- Chia sẻ các kiến thức cốt lõi và lộ trình dịch chuyển hạ tầng từ truyền thống (On-Premise) sang Cloud & DevOps.
- Cập nhật các giải pháp tiên phong trong kỷ nguyên trí tuệ nhân tạo (GraphRAG với Amazon Neptune) và giải pháp bảo mật thông minh kết hợp AWS WAF với Machine Learning.
- Trang bị phương pháp luận để nâng cao hiệu suất làm việc nhóm và kỹ năng quản lý dự án hiệu quả.
- Giới thiệu các công nghệ hiện đại hóa ứng dụng bao gồm cơ chế kết nối thời gian thực cho Game trên Cloud (WebSockets) và công nghệ đóng gói Container (Docker).

### Danh Sách Diễn Giả

- **Vinh Trần** – *System Administrator tại Central Retail Group*
- **Việt Phát** – *AI Research Majoring tại Swinburne University of Technology*
- **Trương Huy Phước** – *Team Productivity & Project Management Specialist*
- **Nguyễn Quốc Bảo** – *Cloud & Multiplayer Game Network Developer*
- **Lê Hoàng Gia Đại** – *Cyber Security & Machine Learning Researcher, HUTECH University*
- **Bảo Huỳnh** – *Junior Cloud Native Developer tại Endava Vietnam, Founder ITea Lab*

---

### Nội Dung Nổi Bật

#### 1. Lộ trình từ IT Helpdesk lên Senior Sysadmin: Hành trình chuyển dịch sang Cloud-DevOps
Diễn giả Vinh Trần đã chia sẻ một hành trình thực tế đầy cảm hứng về sự chuyển dịch tư duy và kỹ năng kỹ thuật từ hạ tầng truyền thống lên điện toán đám mây:
- **Kỹ năng cốt lõi từ Helpdesk:** Rèn luyện tư duy giải quyết vấn đề (problem-solving) dưới áp lực cao, kỹ năng giao tiếp với người dùng cuối và hiểu cách vận hành cơ bản của hệ thống IT.
- **Bước ngoặt dịch chuyển tư duy (Cloud Mindset):** Thay đổi từ việc quản lý máy chủ vật lý, cấu hình thủ công (On-Premise) sang tư duy co giãn linh hoạt (elastic scaling), chi trả theo mức độ sử dụng (pay-as-you-go) và tận dụng các dịch vụ quản lý (managed services) của AWS.
- **Trụ cột hạ tầng hiện đại:** Làm chủ hạ tầng dạng mã (Infrastructure as Code - Terraform), kiểm soát phiên (Version Control) và xây dựng văn hóa DevOps thông qua tự động hóa CI/CD, Container hóa.
- **Bài học xương máu:** Tuyệt đối không bao giờ được phép kiểm thử trực tiếp trên môi trường Production (`Never test in production`) để bảo vệ tính sẵn sàng của hệ thống và uy tín của đội ngũ.

#### 2. AWS Neptune for Building a Graph Knowledge Base for GenAI (GraphRAG)
Diễn giả Việt Phát giới thiệu phương pháp kết hợp Graph với LLM để giải quyết các giới hạn của RAG truyền thống trong kỷ nguyên trí tuệ nhân tạo:
- **Hạn chế của RAG thông thường:** Gặp khó khăn với các câu hỏi đòi hỏi tư duy đa bước (Multi-hop Reasoning) hoặc các câu hỏi cần hiểu sâu về mối quan hệ đan xen giữa nhiều thực thể, văn bản.
- **Sức mạnh của GraphRAG:** Lưu trữ các mối quan hệ một cách tường minh thông qua các cạnh (edges), tăng khả năng nhận thức ngữ cảnh sâu sắc (Relationship Awareness).
- **Hai hướng tiếp cận trên AWS:**
  * **Fully Managed Route (Quản lý hoàn toàn):** Sử dụng *Amazon Bedrock Knowledge Bases* để tự động cắt nhỏ dữ liệu, trích xuất thực thể, tạo Embeddings; kết hợp với *Amazon Neptune Analytics* đóng vai trò làm "bộ não đồ thị" để lưu trữ và khám phá mối quan hệ.
  * **Custom Route (Tùy biến nâng cao):** Sử dụng *LlamaIndex* để chuẩn bị dữ liệu và dựng đồ thị, sau đó lưu trữ vào *Amazon Neptune* và truy vấn dữ liệu đa bước thông qua ngôn ngữ truy vấn Cypher Query.

#### 3. Cách làm việc nhóm hiệu quả và tối ưu hóa năng suất dự án
Diễn giả Trương Huy Phước đúc kết các phương pháp luận cốt lõi để xây dựng đội ngũ và tối ưu hóa hiệu suất làm việc tập thể:
- **4 Nguyên tắc Vàng (The 4 Golden Rules):** 
  1. Mục tiêu chung phải rõ ràng và được chia sẻ đồng thuận (Clear & Shared Goals).
  2. Đặt đúng người vào đúng vị trí năng lực (Right Person, Right Place).
  3. Giao tiếp cởi mở và chủ động lắng nghe (Open Communication & Active Listening).
  4. Nâng cao tinh thần trách nhiệm cá nhân đối với kết quả chung (Personal Accountability).
- **Ứng dụng công cụ số (Digital Tools):** Quản lý tiến độ trực quan qua *Trello, ClickUp*; tối ưu không gian làm việc và chia sẻ tài liệu đồng bộ qua *Google Workspace, Slack, Discord*.

#### 4. Multiplayer in the Cloud: Connecting Godot Clients with AWS WebSockets
Diễn giả Nguyễn Quốc Bảo đã trình diễn giải pháp xây dựng hệ thống Game Multiplayer dựa trên kiến trúc Serverless thời gian thực:
- **Lựa chọn giao thức:** So với HTTP Polling (độ trễ cao) hay UDP/ENet (phức tạp), WebSocket là lựa chọn tối ưu cho các dòng game turn-based, hệ thống phòng chờ (lobby) hoặc chat nhờ khả năng truyền dữ liệu hai chiều thời gian thực (full-duplex) và đáng tin cậy.
- **Thiết kế kiến trúc AWS Serverless:** 
  * **Godot Client:** Sử dụng `WebSocketPeer` bằng GDScript để kết nối.
  * **Amazon API Gateway (WebSocket API):** Quản lý các kết nối duy trì và định tuyến yêu cầu dựa trên Route Key (`$request.body.action`).
  * **AWS Lambda & Amazon DynamoDB:** Lambda xử lý logic trò chơi một cách bất đồng bộ; DynamoDB lưu trữ trạng thái `connectionId` của người chơi.
- **Thử thách kỹ thuật:** Đối mặt với vấn đề kết nối rác (Stale connections/GoneException), chi phí quét bảng DynamoDB (Scan Cost) và tính chất không lưu trạng thái (Stateless) của Lambda, từ đó mở ra hướng phát triển tiếp theo với *AWS GameLift* cho các dòng game tốc độ cao.

#### 5. Combining AWS WAF with Machine Learning for Advanced Network Intrusion Detection
Diễn giả Lê Hoàng Gia Đại mang đến giải pháp bảo mật thông minh dựa trên dữ liệu và AI để bảo vệ hạ tầng đám mây:
- **Vấn đề của AWS WAF truyền thống:** Hoạt động dựa trên các dấu hiệu nhận dạng có sẵn (Signature-based), do đó không đủ linh hoạt để đối phó với các hình thức tấn công mới hoặc các biến thể tinh vi (anomalous requests).
- **Hệ thống NIDS dựa trên Học máy:** Sử dụng tập dữ liệu tiêu chuẩn `CSE-CIC-IDS2018` để huấn luyện mô hình ML có khả năng phát hiện các hành vi bất thường, giải quyết bài toán mất cân bằng dữ liệu (data imbalance) đối với các lớp tấn công thiểu số.
- **Luồng vận hành phối hợp:** Đưa ra dự đoán từ mô hình học máy (ML-based NIDS) kết hợp đồng bộ với các sự kiện ghi nhận từ *AWS WAF*, biểu diễn trực quan qua hệ thống bảng điều khiển (Dashboard) thời gian thực, giúp nâng cao toàn diện khả năng giám sát an ninh (Threat Visibility).

#### 6. Docker - A Containerization Technology
Diễn giả Bảo Huỳnh mang đến góc nhìn hệ thống sâu sắc về sự tiến hóa từ ảo hóa truyền thống sang công nghệ container:
- **Hạn chế của Ảo hóa cũ (Virtual Machines):** Mỗi VM đều yêu cầu một hệ điều hành (OS) riêng biệt, gây tiêu tốn tài nguyên CPU, RAM, dung lượng lưu trữ nặng nề và phức tạp trong việc cập nhật bản vá hệ thống.
- **Bản chất của Containerization:** Đóng gói ứng dụng cùng toàn bộ các thư viện phụ thuộc (dependencies) và cấu hình cần thiết vào một gói duy nhất, giúp ứng dụng chạy đồng nhất trên mọi môi trường từ máy Dev đến Production.
- **Kiến trúc Dockerfile & Lớp ảnh (Image Layers):** Mỗi câu lệnh trong Dockerfile (`FROM`, `RUN`, `COPY`, `CMD`) tạo ra một lớp ảnh (layer). Docker tối ưu hóa quá trình Build bằng cách tái sử dụng các lớp không thay đổi từ bộ nhớ đệm (Cache). Nếu một lớp thay đổi, chỉ lớp đó và các lớp phía sau nó mới được dựng lại.

---

### Những Gì Học Được

#### Tư Duy Thiết Kế
- **Tư duy hướng sản phẩm thực tế (Portfolio-first):** Hiểu rằng kinh nghiệm thực chiến thông qua việc tự xây dựng và vận hành các dự án thực tế có giá trị tuyển dụng cao hơn rất nhiều so với việc chỉ sở hữu các chứng chỉ lý thuyết suông.
- **Tư duy dựa trên mối quan hệ (Graph Thinking):** Nhận thức được dữ liệu không tồn tại độc lập mà liên kết chặt chẽ với nhau; việc mô hình hóa dữ liệu dạng đồ thị (Nodes/Edges) giúp giải quyết các bài toán GenAI phức tạp một cách thông minh hơn.
- **Tư duy an ninh chủ động:** Bảo mật hạ tầng hiện đại không chỉ là dựng tường lửa cứng (WAF) mà phải kết hợp giám sát hành vi bằng học máy (Machine Learning) để phát hiện rủi ro từ sớm.

#### Kiến Trúc Kỹ Thuật
- Hiểu sâu về cơ chế phân lớp (Layering) và bộ nhớ đệm (Caching) của **Docker**, biết cách viết một Dockerfile chuẩn hóa, tối ưu dung lượng và tốc độ đóng gói.
- Nắm vững kiến trúc **Serverless WebSockets** trên AWS bằng cách phối hợp nhịp nhàng giữa `API Gateway, Lambda và DynamoDB` nhằm xây dựng các ứng dụng giao tiếp thời gian thực, tối ưu chi phí.
- Biết cách phân loại và lựa chọn giải pháp GraphRAG (Managed vs Custom) tùy thuộc vào quy mô dự án và yêu cầu kiểm soát mã nguồn dựa trên nền tảng Amazon Neptune.

---

### Ứng Dụng Vào Công Việc

- **Áp dụng Docker vào đồ án:** Container hóa toàn bộ các dự án, bài tập lớn hiện tại bằng Docker để đảm bảo môi trường chạy đồng nhất từ máy cá nhân lên môi trường kiểm thử.
- **Cải tổ Portfolio tuyển dụng cá nhân:** Sắp xếp lại CV, tập trung làm nổi bật các dự án thực tế, các giải pháp kiến trúc đã từng tự tay thiết kế và cấu hình thay vì liệt kê lý thuyết chung chung theo đúng lời khuyên từ nhà tuyển dụng.
- **Áp dụng 4 nguyên tắc vàng khi làm bài tập nhóm:** Sử dụng Trello/ClickUp để phân rã công việc cụ thể cho từng thành viên, thiết lập kênh Discord riêng để tăng tương tác và tính minh bạch khi làm việc chung.
- **Thử nghiệm kiến trúc thời gian thực:** Triển khai một ứng dụng chat mini hoặc game turn-based cơ bản sử dụng AWS API Gateway WebSocket và Lambda để trực tiếp thực hành cơ chế quản lý trạng thái kết nối.

---

### Trải nghiệm trong event

Tham gia chuỗi chia sẻ tại **FCAJ Community Day** mang lại cho tôi những trải nghiệm công nghệ vô cùng toàn diện, kết nối từ những kỹ năng mềm thiết yếu đến các kiến trúc kỹ thuật chuyên sâu.

#### Học hỏi từ các diễn giả có chuyên môn cao
- Các bài chia sẻ vô cùng thực tế, phản ánh đúng những bài toán thực chiến tại doanh nghiệp lớn như Central Retail Group hay Endava. 
- Lời khuyên định hướng nghề nghiệp từ anh Vinh Trần giúp tôi tránh được sai lầm phổ biến là học quá nhiều thứ cùng một lúc mà không đào sâu vào bất kỳ năng lực cốt lõi nào.

#### Trải nghiệm kỹ thuật thực tế
- Được tiếp cận trực quan sơ đồ kiến trúc hệ thống mạng của các giải pháp thực tế. Việc thấy cách một tín hiệu từ Godot Client chạy qua API Gateway kích hoạt Lambda, hay cách các tệp dữ liệu được chuyển hóa thành Knowledge Graph trên Amazon Neptune giúp tôi có tư duy hệ thống rất rõ ràng.
- Hiểu được các thách thức vận hành thực tế như xử lý mất cân bằng dữ liệu trong AI bảo mật hay tối ưu chi phí Scan dữ liệu trên Cloud.

#### Kết nối và trao đổi
- Sự kiện tạo ra một không gian trao đổi cởi mở, nơi các thành viên thoải mái đặt câu hỏi, phản biện và học hỏi lẫn nhau theo đúng tinh thần "Continuous Learning" và văn hóa chia sẻ trách nhiệm của cộng đồng FCAJ.

#### Bài học rút ra
- Điểm xuất phát không quan trọng, sự kiên trì và tích lũy từng bước nhỏ thông qua các dự án thực tế mới là chìa khóa để dịch chuyển thành công sang Cloud & DevOps.
- Signature-based bảo mật hay RAG truyền thống đã không còn đủ cho các bài toán hiện đại; việc làm chủ ML, Graph Database (Amazon Neptune) và kiến trúc hướng sự kiện (Serverless WebSockets) chính là lợi thế cạnh tranh cốt lõi của một kỹ sư Cloud thế hệ mới.

---

### Một Số Hình Ảnh Khi Tham Gia Sự Kiện

<div align="center" style="width: 100%; margin: 0 auto; padding: 10px;">
  <div style="display: flex; flex-wrap: nowrap; justify-content: center; gap: 6px; line-height: 0; margin-bottom: 6px;">
    <!-- HÀNG 1: 3 hình -->
    <img src="/images/4-Event/Event2/event2(1).jpg" style="width: 33.33%; display: block; object-fit: cover; aspect-ratio: 4/3; margin: 0;" />
    <img src="/images/4-Event/Event2/event2(2).jpg" style="width: 33.33%; display: block; object-fit: cover; aspect-ratio: 4/3; margin: 0;" />
    <img src="/images/4-Event/Event2/event2(3).jpg" style="width: 33.33%; display: block; object-fit: cover; aspect-ratio: 4/3; margin: 0;" />
  </div>
  
  <div style="display: flex; flex-wrap: nowrap; justify-content: center; gap: 6px; line-height: 0;">
    <!-- HÀNG 2: 3 hình -->
    <img src="/images/4-Event/Event2/event2(4).jpg" style="width: 33.33%; display: block; object-fit: cover; aspect-ratio: 4/3; margin: 0;" />
    <img src="/images/4-Event/Event2/event2(5).jpg" style="width: 33.33%; display: block; object-fit: cover; aspect-ratio: 4/3; margin: 0;" />
    <img src="/images/4-Event/Event2/event2(6).jpg" style="width: 33.33%; display: block; object-fit: cover; aspect-ratio: 4/3; margin: 0;" />
  </div>
  
  <p style="margin-top: 20px; margin-bottom: 0;"><i>Ảnh chụp các bài thuyết trình tại FCAJ Community Day</i></p>
</div>