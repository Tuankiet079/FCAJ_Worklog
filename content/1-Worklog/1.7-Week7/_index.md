---
title: "Worklog Week 7"
date: 2026-06-15
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives:

* Build the overall project system architecture diagram.
* Review and compare classmates' assignments/projects to extract optimal solutions for the team project.
* Explore and analyze the pros and cons of different architecture variants: traditional servers, Serverless, and hybrid architecture.

### Tasks to be completed this week:

| Day | Task | Start Date | End Date | Documentation |
| ---- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | ------------------ | ----------------- |
| Mon | - Review classmates' project evaluations: <br>+ Analyze the architecture models used by other groups. <br>+ Discuss ideas with the team to select suitable solutions for the project. | 15/06/2026 | 15/06/2026 | |
| Tue | - Design a traditional server architecture: <br>+ Draw a diagram: EC2 + RDS + Load Balancer. <br>+ Evaluate scalability and operational cost. | 16/06/2026 | 16/06/2026 | |
| Wed | - Design hybrid architectures: <br>+ Model 1: EC2 + Supabase + Supabase Pooling. <br>+ Model 2: EC2 + RDS + RDS Proxy + Load Balancer. | 17/06/2026 | 17/06/2026 | |
| Thu | - Design pure Serverless architectures: <br>+ Model 1: Lambda + AuroraDB + RDS Proxy. <br>+ Model 2: Lambda + AuroraDB + ElastiCache + RDS Proxy. | 18/06/2026 | 18/06/2026 | |
| Fri | - Synthesize and finalize the project architecture: <br>+ Compare latency, cost, and maintainability across variants. <br>+ Finalize the architecture for the group project. | 19/06/2026 | 19/06/2026 | |

### Week 7 Results:

* Completed the review and cross-evaluation of classmates' projects, gaining new perspectives on resource allocation and data flow design for the team project.
* Finished sketching and visualizing five infrastructure architecture variants:
  * Traditional architecture: `EC2 + RDS + Load Balancer` — easy to understand but incurs fixed operational cost and requires careful Auto Scaling.
  * Hybrid architecture 1: `EC2 + Supabase + Supabase Pooling` — combines EC2 compute with Backend-as-a-Service and reduces direct Postgres connections.
  * Hybrid architecture 2: `EC2 + RDS + RDS Proxy + Load Balancer` — addresses database connection bottlenecks in the traditional model with an RDS Proxy buffer.
  * Serverless architecture 1: `Lambda + AuroraDB + RDS Proxy` — cost-effective pay-per-use, with RDS Proxy preserving connection pooling and preventing Lambda from opening too many database connections under burst traffic.
  * Serverless architecture 2: `Lambda + AuroraDB + ElastiCache + RDS Proxy` — the most comprehensive model. Adding ElastiCache reduces database queries and improves response time, but costs exceed the current project scale.
* Sketching multiple variants helped the team understand tradeoffs between maintainability, performance, and cost, giving enough basis to finalize the system architecture.
