---
title: "Worklog Week 6"
date: 2026-06-08
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Objectives:

* Learn AWS storage and backup services: Amazon S3 and AWS Backup.
* Explore solutions using AWS Lambda to automatically export the database for cheaper off-cloud storage.
* Pause cloud tasks briefly and return to Node.js to solve the core backend game problem: designing an anti-cheat item system using deterministic random generation based on a `master seed`.

### Tasks to be completed this week:

| Day | Task | Start Date | End Date | Documentation / Notes |
| --------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------- | ------------------ | ----------------------------------------------------------------------------------------------------------------------------- |
| Mon | - Learn Amazon S3: <br>+ Storage tiers. <br>+ Versioning and Bucket Policies. <br>+ Overview of AWS Backup. | 08/06/2026 | 08/06/2026 | |
| Tue | - Investigate a custom backup solution: <br>+ Consider using Lambda scheduled triggers to export the database to files and upload them to S3. <br>+ Evaluate cost and feasibility. | 09/06/2026 | 09/06/2026 | A custom solution was unnecessary because standard Backup services are affordable and text data is lightweight. |
| Wed - Fri | - Learn Deterministic Random techniques. <br> - Build a pseudo-random number algorithm based on a server-issued `master seed`. <br> - Integrate and test: <br>+ Server creates and stores the seed for each session. <br>+ Validate item results submitted by the client by replaying the same seed on the server. | 10/06/2026 | 12/06/2026 | |

### Week 6 Results:

* Mastered how to manage static objects on Amazon S3 and set lifecycle policies to optimize long-term storage costs.
* Completed a feasibility assessment of using AWS Lambda to export the database automatically for separate storage.
* Strengthened backend Node.js development skills by solving a real game development problem.
* Successfully designed and implemented a Deterministic Random mechanism:
  * Understood the anti-cheat principle: the client does not decide item drop results; all random numbers are generated from a server-issued `master seed`.
  * Built a synchronized flow: the server creates the `master seed` at the start of a session and sends it to the client. When the client reports a drop result, the server replays the seed. If the results match, the item is recorded.
  * This method helps prevent cheating while keeping server load manageable because the server does not need to recalculate drop probabilities for every enemy.
