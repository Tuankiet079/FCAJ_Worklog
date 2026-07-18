---
title: "Worklog Week 5"
date: 2026-06-01
weight: 5
chapter: false
pre: " <b> 1.5. </b> "
---

### Week 5 Objectives:

* Learn resource optimization techniques and system load management on AWS.
* Practice distributed system design by splitting the project into independent AWS Lambda functions.
* Understand optimization support services: Amazon RDS Proxy, Amazon ElastiCache, Amazon SQS, and Elastic Load Balancing.

### Tasks to be completed this week:

| Day | Task | Start Date | End Date | Documentation / Notes |
| ---- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Mon | - Analyze the project structure and design Microservices: <br>+ Decompose application logic into independent AWS Lambda functions. <br>+ Define boundaries and how functions communicate. | 01/06/2026 | 01/06/2026 | |
| Tue | - Learn database connection optimization: <br>+ Understand connection exhaustion when Lambda uses RDS. <br>+ Use Amazon RDS Proxy for connection pooling. | 02/06/2026 | 02/06/2026 | |
| Wed | - Learn read performance optimization: <br>+ How Amazon ElastiCache works. <br>+ Basic differences between Redis and Memcached. <br>+ Apply caching to reduce database load. | 03/06/2026 | 03/06/2026 | Theory was far from practice; applying cache for asynchronous processing is nearly impractical for current needs. |
| Thu | - Learn asynchronous processing and decoupling: <br>+ Amazon SQS. <br>+ How to use SQS as a buffer between services to avoid overload. | 04/06/2026 | 04/06/2026 | |
| Fri | - Learn load balancing for EC2: <br>+ Basic Elastic Load Balancing. <br>+ Differences between Application Load Balancer and Network Load Balancer. | 05/06/2026 | 05/06/2026 | |

### Week 5 Results:

* Developed the mindset of moving from Monolithic to Serverless Microservices by decomposing the project into specialized AWS Lambda functions.
* Understood the cause of database connection bottlenecks when Lambda scales up and how RDS Proxy preserves and reuses connections.
* Learned how to speed up responses and reduce main database load by caching frequently accessed data with Amazon ElastiCache.
* Understood the concept of decoupling system components with Amazon SQS and how to handle sudden traffic spikes with asynchronous queues.
* Distinguished ALB and NLB operational layers and learned how to choose the right load balancer to distribute traffic evenly.
