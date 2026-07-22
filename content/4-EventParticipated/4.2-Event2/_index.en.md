---
title: "Event 2"
date: 2024-01-01
weight: 1
chapter: false
pre: " <b> 4.2. </b> "
---


# Summary Report: "FCAJ Community Day: Cloud-Native & Advanced Tech Sharing Session"

### Purpose of the Event

- Share core knowledge and career pathways for transitioning infrastructure from traditional On-Premise environments to Cloud & DevOps.
- Update pioneering solutions in the era of Artificial Intelligence (GraphRAG with Amazon Neptune) and intelligent security combining AWS WAF with Machine Learning.
- Equip participants with methodologies to enhance team collaboration efficiency and effective project management skills.
- Introduce application modernization technologies, including real-time communication mechanisms for Cloud Gaming (WebSockets) and containerization concepts (Docker).

### Speaker List

- **Vinh Tran** – *System Administrator at Central Retail Group*
- **Viet Phat** – *AI Research Major at Swinburne University of Technology*
- **Truong Huy Phuoc** – *Team Productivity & Project Management Specialist*
- **Nguyen Quoc Bao** – *Cloud & Multiplayer Game Network Developer*
- **Le Hoang Gia Dai** – *Cyber Security & Machine Learning Researcher, HUTECH University*
- **Bao Huynh** – *Junior Cloud Native Developer at Endava Vietnam, Founder of ITea Lab*

---

### Key Highlights

#### 1. Career Path from IT Helpdesk to Senior Sysadmin: Navigating the Shift to Cloud-DevOps
Speaker Vinh Tran shared an inspiring, real-world career trajectory on shifting mindsets and technical skills from legacy infrastructure to cloud computing:
- **Core Skills from Helpdesk:** Cultivating problem-solving mindsets under pressure, mastering end-user communication, and understanding foundational IT operations.
- **The Cloud Mindset Pivot:** Shifting from managing physical servers and manual configurations (On-Premise) toward elastic scaling, pay-as-you-go economic models, and leveraging AWS Managed Services.
- **Modern Infrastructure Pillars:** Mastering Infrastructure as Code (IaC via Terraform), Version Control Systems, and building DevOps culture through automated CI/CD pipelines and containerization.
- **Crucial Lesson:** Never test directly in Production (`Never test in production`) to protect system availability and team reputation.

#### 2. AWS Neptune for Building a Graph Knowledge Base for GenAI (GraphRAG)
Speaker Viet Phat introduced a hybrid Graph + LLM approach to address the inherent limitations of traditional Retrieval-Augmented Generation (RAG) in AI:
- **Limitations of Traditional RAG:** Struggles with multi-hop reasoning or questions demanding deep comprehension of interconnected entities across multiple documents.
- **The Power of GraphRAG:** Explicitly stores relationships using edges, significantly enhancing Relationship Awareness and contextual intelligence.
- **Two Deployment Routes on AWS:**
  * **Fully Managed Route:** Utilize *Amazon Bedrock Knowledge Bases* to automatically chunk data, extract entities, and generate embeddings; combined with *Amazon Neptune Analytics* acting as the graph engine to store and traverse relationships.
  * **Custom Advanced Route:** Utilize *LlamaIndex* for data preparation and graph construction, followed by persistent storage in *Amazon Neptune* and multi-hop querying via Cypher Query Language.

#### 3. High-Performance Teamwork and Project Productivity Optimization
Speaker Truong Huy Phuoc synthesized core methodologies for team building and optimizing collective productivity:
- **The 4 Golden Rules:** 
  1. Clear and aligned shared goals (Clear & Shared Goals).
  2. Assigning the right person to the right position based on competency (Right Person, Right Place).
  3. Fostering open communication and active listening (Open Communication & Active Listening).
  4. Elevating personal accountability toward shared outcomes (Personal Accountability).
- **Leveraging Digital Tools:** Visualizing project progress via *Trello, ClickUp*; optimizing collaborative workspaces and document sharing through *Google Workspace, Slack, Discord*.

#### 4. Multiplayer in the Cloud: Connecting Godot Clients with AWS WebSockets
Speaker Nguyen Quoc Bao demonstrated real-time multiplayer game system architectures built entirely on AWS Serverless:
- **Protocol Selection:** Compared to HTTP Polling (high latency) or UDP/ENet (complex configuration), WebSockets represent the optimal choice for turn-based games, lobbies, and chat features due to full-duplex, reliable real-time communication.
- **AWS Serverless Architecture Design:** 
  * **Godot Client:** Connects using GDScript via `WebSocketPeer`.
  * **Amazon API Gateway (WebSocket API):** Manages persistent connections and routes requests using Route Keys (`$request.body.action`).
  * **AWS Lambda & Amazon DynamoDB:** Lambda executes game logic asynchronously; DynamoDB tracks player `connectionId` states.
  * **Technical Challenges:** Managing stale connections (`GoneException`), optimizing DynamoDB table scan costs, and handling Lambda's stateless nature—opening pathways toward *AWS GameLift* for high-frequency competitive games.

#### 5. Combining AWS WAF with Machine Learning for Advanced Network Intrusion Detection
Speaker Le Hoang Gia Dai presented an AI and data-driven security solution to safeguard cloud infrastructure:
- **Limitations of Traditional AWS WAF:** Relies heavily on signature-based matching rules, making it inflexible against zero-day exploits or complex anomalous requests.
- **ML-Based Network Intrusion Detection Systems (NIDS):** Trained machine learning models on the benchmark `CSE-CIC-IDS2018` dataset to detect anomalous behavior while addressing data imbalance across minority attack classes.
- **Collaborative Security Workflow:** Combined ML predictions with real-time logs from *AWS WAF*, visualized through live monitoring dashboards to significantly boost Threat Visibility.

#### 6. Docker - A Containerization Technology
Speaker Bao Huynh delivered deep architectural insights into the evolution from traditional virtualization to containerization:
- **Drawbacks of Legacy Virtual Machines:** Each VM requires a full guest Operating System (OS), consuming massive CPU, RAM, and storage overhead while complicating patch management.
- **Essence of Containerization:** Packages applications along with all dependencies and configurations into a single isolated unit, guaranteeing consistent execution across environments from Local Dev to Production.
- **Dockerfile Architecture & Image Layering:** Every Dockerfile instruction (`FROM`, `RUN`, `COPY`, `CMD`) produces a distinct layer. Docker optimizes build processes by reusing cached, unchanged layers. When a layer changes, only that layer and subsequent layers are rebuilt.

---

### Key Takeaways

#### Design Mindset
- **Portfolio-First Mindset:** Practical experience gained by designing, deploying, and operating real-world projects carries far greater value in hiring than holding theoretical certifications alone.
- **Graph-Oriented Thinking:** Data does not exist in isolation but in complex interconnectivity; modeling data as graphs (Nodes/Edges) allows AI systems to solve complex GenAI problems with higher precision.
- **Proactive Defense Mindset:** Modern infrastructure security goes beyond static firewalls (WAF), requiring behavioral monitoring via Machine Learning to detect risks proactively.

#### Technical Architecture
- Deeply understood **Docker** image layering and build caching mechanisms, enabling the creation of standardized, optimized Dockerfiles.
- Mastered **Serverless WebSockets** architecture on AWS by combining `API Gateway, Lambda, and DynamoDB` to build cost-effective, real-time interactive systems.
- Learned to evaluate and select appropriate GraphRAG solutions (Managed vs Custom) on Amazon Neptune based on project scale and control requirements.

---

### Practical Application

- **Implement Docker in Academic Projects:** Containerize existing course projects using Docker to ensure environment parity from local machines to test environments.
- **Revamp Professional Resume & Portfolio:** Restructure CVs to highlight hands-on projects and architectural solutions designed from scratch, aligning with enterprise hiring expectations.
- **Apply the 4 Golden Rules to Group Work:** Use Trello/ClickUp to break down tasks clearly among teammates and establish dedicated Discord channels for transparent communication.
- **Experiment with Real-Time Architectures:** Build a mini chat application or basic turn-based game using AWS API Gateway WebSockets and Lambda to practice managing persistent connection states.

---

### Event Experience

Attending the **FCAJ Community Day** sharing sessions provided me with a comprehensive technical experience, bridging foundational soft skills with deep architectural concepts.

#### Insights from Industry Experts
- Presentations reflected real enterprise challenges from major organizations like Central Retail Group and Endava.
- Career advice from Mr. Vinh Tran helped me avoid the common pitfall of learning too many technologies at once without mastering a core competency.

#### Hands-On Technical Experience
- Gained visual clarity on system architecture diagrams for production systems. Seeing signals traverse from Godot Clients through API Gateway to trigger Lambda, or how raw data transforms into Knowledge Graphs on Amazon Neptune, significantly strengthened my systems thinking.
- Understood practical operational challenges, such as handling dataset imbalances in security AI and optimizing cloud database scan costs.

#### Networking & Exchange
- The event cultivated an open environment where participants freely asked questions, debated ideas, and learned from one another, embodying the FCAJ community's culture of Continuous Learning and Shared Responsibility.

#### Lessons Learned
- Starting points do not dictate success; persistence and incremental progress through hands-on projects are key to successfully transitioning into Cloud & DevOps.
- Traditional signature-based firewalls and standard RAG models are no longer sufficient for modern workloads; mastering Machine Learning, Graph Databases (Amazon Neptune), and Event-Driven Architectures (Serverless WebSockets) forms the core competitive edge for next-generation Cloud Engineers.

---

### Event Gallery

<div align="center" style="width: 100%; margin: 0 auto; padding: 10px;">
  <div style="display: flex; flex-wrap: nowrap; justify-content: center; gap: 6px; line-height: 0; margin-bottom: 6px;">
    <!-- ROW 1: 3 images -->
    <img src="../../images/4-Event/Event2/event2(1).jpg" style="width: 33.33%; display: block; object-fit: cover; aspect-ratio: 4/3; margin: 0;" />
    <img src=../../images/4-Event/Event2/event2(2).jpg" style="width: 33.33%; display: block; object-fit: cover; aspect-ratio: 4/3; margin: 0;" />
    <img src="../../images/4-Event/Event2/event2(3).jpg" style="width: 33.33%; display: block; object-fit: cover; aspect-ratio: 4/3; margin: 0;" />
  </div>
  
  <div style="display: flex; flex-wrap: nowrap; justify-content: center; gap: 6px; line-height: 0;">
    <!-- ROW 2: 3 images -->
    <img src="../../images/4-Event/Event2/event2(4).jpg" style="width: 33.33%; display: block; object-fit: cover; aspect-ratio: 4/3; margin: 0;" />
    <img src="../../images/4-Event/Event2/event2(5).jpg" style="width: 33.33%; display: block; object-fit: cover; aspect-ratio: 4/3; margin: 0;" />
    <img src="../../images/4-Event/Event2/event2(6).jpg" style="width: 33.33%; display: block; object-fit: cover; aspect-ratio: 4/3; margin: 0;" />
  </div>
  
  <p style="margin-top: 20px; margin-bottom: 0;"><i>Presentations at FCAJ Community Day</i></p>
</div>