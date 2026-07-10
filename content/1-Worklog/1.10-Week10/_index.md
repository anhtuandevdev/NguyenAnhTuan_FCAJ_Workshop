---
title: "Week 10 Worklog"
date: 2026-7-07
weight: 10
chapter: false
pre: " <b> 1.10. </b> "
---

### Week 10 Objectives

- Build an automated infrastructure scheduler to drastically curb runtime cloud bill waste[cite: 3, 8].
- Create event-driven Lambda logic that automatically suspends development systems when idle[cite: 3, 8].
- Bridge serverless engine authorizations cleanly to orchestrate infrastructure state transitions[cite: 3, 8, 10].

### Tasks Carried Out This Week

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 1 | Authored an automated script leveraging Boto3 Python kits to toggle infrastructure states based on resource tag values[cite: 8, 10]. | 08/03/2026 | 08/03/2026 | Python Boto3 SDK |
| 2 | Configured precise Amazon EventBridge Cron triggers firing automation scripts at fixed schedule marks[cite: 8]. | 08/04/2026 | 08/04/2026 | EventBridge Scheduling |
| 3 | Formed custom IAM execution roles giving Lambda granular permissions to trigger infrastructure state transitions[cite: 8, 10]. | 08/05/2026 | 08/05/2026 | IAM Least Privilege |
| 4 | Conducted testing by manually firing event schedules and tracking system states via CloudWatch[cite: 3, 8]. | 08/06/2026 | 08/06/2026 | CloudWatch Logs Engine |
| 5 | Audited real-time billing activity logs to measure cost reduction gains following scheduler deployment[cite: 5, 8]. | 08/07/2026 | 08/07/2026 | Cost Explorer Dashboard |

### Week 10 Achievements

- Successfully implemented a zero-touch infrastructure schedule that automatically parks test machines outside business hours[cite: 8].
- Drastically reduced sandbox infrastructure operating expenses by eliminating weekend and overnight runtime waste[cite: 8].
- Replaced unsafe personal keys by routing orchestration controls through secure native instance profiles[cite: 10].
- Preserved developer agility by ensuring testing sandboxes automatically spin back up before morning shifts start[cite: 8].
- Created a reusable cost-saving automation blueprint that can easily be adapted for future project components[cite: 8].

### Plan for Next Week

- Introduce horizontal elasticity and auto-recovery mechanics to the processing tier.
- Build resilient, load-balanced, and auto-scaling compute pools using EC2 Auto Scaling Groups[cite: 10].