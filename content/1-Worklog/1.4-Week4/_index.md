---
title: "Worklog Week 4"
date: 2026-05-25
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---
### Week 4 Objectives:

* Understand Serverless architecture concepts on AWS.
* Get familiar with AWS Lambda and serverless databases (DynamoDB, Aurora).
* Explore edge networking and security services: API Gateway, CloudFront, AWS WAF.

### Tasks to be completed this week:

| Day | Task                                                                                                                                                | Start Date | End Date   | Documentation |
| --- | --------------------------------------------------------------------------------------------------------------------------------------------------- | ---------- | ---------- | ------------- |
| Mon | - Learn Serverless architecture on AWS:+ Serverless concepts. + Pros and cons versus traditional servers. + Explore AWS Lambda.                     | 25/05/2026 | 25/05/2026 |               |
| Tue | - Learn serverless-supported databases:+ Amazon DynamoDB. + Amazon Aurora Serverless. + Use cases for each database type.                           | 26/05/2026 | 26/05/2026 |               |
| Wed | - Initialize Amazon Aurora. - Try packaging the entire project into one Lambda.                                                                     | 27/05/2026 | 27/05/2026 |               |
| Thu | - Learn edge networking:+ Amazon API Gateway. + Amazon CloudFront. + AWS WAF.  - Use CloudFormation to build the edge layer for the Lambda project. | 28/05/2026 | 28/05/2026 |               |

### Week 4 Results:

* Understood Serverless principles, cost optimization, and reduced server operation overhead.
* Learned how AWS Lambda works, including triggers and execution permissions.
* Distinguished between DynamoDB and Aurora Serverless and when to use each in the project.
* Successfully deployed an all-in-one Serverless model.
* Understood edge services roles:  - API Gateway as the gateway for managing API calls to Lambda.  - CloudFront for low-latency content delivery.  - AWS WAF for blocking malicious traffic before it reaches the backend.
* Learned the end-to-end service flow: `End-user -> CloudFront -> API Gateway -> Lambda -> DynamoDB`.
