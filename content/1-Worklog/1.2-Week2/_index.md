---
title: "Worklog Week 2"
date: 2026-05-11
weight: 2
chapter: false
pre: " <b> 1.2. </b> "
---

### Week 2 Objectives:

* Learn AWS services and free modules that can be directly applied to the project.
* Deploy the actual project on an EC2 virtual machine and an RDS database.

### Tasks to be completed this week:

| Day | Task | Start Date | End Date | Documentation |
| --- | --- | --- | --- | --- |
| Mon | - Learn AWS services and free modules applicable to the project: <br>&emsp; + EC2 (t3.micro) <br>&emsp; + RDS (db.t4g.micro) <br>&emsp; + Amazon GameLift <br>&emsp; + ElastiCache (cache.t3.micro) | 11/05/2026 | 11/05/2026 | |
| Tue - Thu | - Initialize core resources: <br>&emsp; + Create an EC2 instance (t3.micro) with Ubuntu Linux. <br>&emsp; + Create an RDS instance (db.t4g.micro) running MySQL. <br>&emsp; + Configure a static IP for the server using Elastic IP. | 12/05/2026 | 14/05/2026 | |
| Fri - Sat | - Configure and link resources: <br>&emsp; + Connect the RDS database to EC2. <br>&emsp; + Set inbound rules (launch-wizard-x). <br>&emsp; + Use spare disk space to create swap memory. | 15/05/2026 | 16/05/2026 | |
| Sun | - Deploy the project: <br>&emsp; + Use pm2 to deploy directly on the EC2 VM. <br>&emsp; + Open ports so other machines can access the public IP. | 17/05/2026 | 17/05/2026 | |

### Week 2 Results:

* Identified the free AWS services/modules suitable for the project: EC2, RDS, Amazon GameLift, ElastiCache.
* Successfully deployed the EC2 virtual machine (Ubuntu Linux, t3.micro) and the MySQL RDS database (db.t4g.micro).
* Configured a static IP for the server using Elastic IP.
* Completed the RDS-to-EC2 connection and inbound rule setup (launch-wizard-x) to allow access.
* Optimized the VM by using spare disk space as swap memory.
* Used pm2 to deploy the project directly on EC2 and opened access successfully via the public IP.
