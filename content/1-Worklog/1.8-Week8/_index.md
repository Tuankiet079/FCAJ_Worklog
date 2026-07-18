---
title: "Worklog Week 8"
date: 2026-06-22
weight: 8
chapter: false
pre: " <b> 1.8. </b> "
---

### Week 8 Objectives:

* Learn database maintenance tasks for relational databases (PostgreSQL/Aurora) using `VACUUM` and `ANALYZE`.
* Master techniques for intervening in API Gateway using Stage Variables to flexibly open/close communication channels.
* Identify and design an automated system maintenance flow as a special project feature.
* Finalize and compare the complete system architecture.
* Review the architecture and create a detailed deployment plan with task assignments for each team.

### Tasks to be completed this week:

| Day | Task | Start Date | End Date | Documentation |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | ------------------ | ----------------- |
| Mon | - Learn DB maintenance: <br>+ `VACUUM`: clean dead tuples. <br>+ `ANALYZE`: update statistics for the query planner. <br> - Learn API Gateway: use SDK to update `stageVariables`, route traffic to a maintenance page, or return 503 when needed. | 22/06/2026 | 22/06/2026 | |
| Tue | - Complete, agree on, and review the architecture. <br> - Plan: split the system into small modules, assign implementation tasks, and delegate responsibilities to team members. | 23/06/2026 | 23/06/2026 | |
| Wed - Sun | - Implement and document step-by-step for: <br>+ Infrastructure: IAM Roles, policies, worst-case cost calculations, and AWS Budget limits. <br>+ Edge layer: deploy CloudFront and WAF with CloudFormation in the US region. <br>+ Database: deploy Aurora SQL and AWS Backup with S3 using CloudFormation. | 24/06/2026 | 28/06/2026 | |

### Week 8 Results:

* Mastered relational database maintenance for Aurora/PostgreSQL using `VACUUM` and `ANALYZE`.
* Learned how to use SDK to manage API Gateway and dynamically update `stageVariables` to route traffic to maintenance mode or protect the system.
* Finalized and reviewed the overall system architecture, ensuring component integration.
* Successfully created a detailed deployment plan: decomposed the system into modules, assigned teams, and clarified responsibilities for each member.
* Successfully implemented and documented core infrastructure and guidance for: <br> - Base infrastructure: IAM Roles, security policies, cost-risk calculations, and AWS Budget alerts. <br> - Edge layer: CloudFront and WAF deployment with CloudFormation in the US region. <br> - Database and storage: Aurora SQL deployment and automated backup to Amazon S3 using AWS Backup and CloudFormation. | 24/06/2026 | 28/06/2026 | |
