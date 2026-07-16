---
title: "Week 3 Worklog"
date: 2026-05-01
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives

- Establish the core security perimeter using AWS Identity and Access Management (IAM).
- Enforce the Principle of Least Privilege across administrative and operator accounts.
- Implement programmatic security access and temporary session tokens using IAM Roles and Conditions.

### Tasks Carried Out This Week

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 1 | Created specialized IAM Groups to categorize administrative, development, and operational operations. | 01/05/2026 | 01/05/2026 | AWS IAM User Guide |
| 2 | Provisioned isolated IAM administrative users to eliminate the dangerous habit of using the root account directly. | 02/05/2026 | 02/05/2026 | AWS Security Manual |
| 3 | Configured advanced IAM Roles incorporating custom JSON Policies with explicit 'Allow' and 'Deny' scopes. | 03/05/2026 | 03/05/2026 | JSON Schema Reference |
| 4 | Embedded strict Condition blocks inside policies based on corporate source IP addresses and specific time windows. | 04/05/2026 | 04/05/2026 | AWS Policy Conditions |
| 5 | Tested the Assume Role workflow to acquire short-term real-time operational credentials via AWS STS. | 05/05/2026 | 05/05/2026 | AWS STS Documentation |

### Week 3 Achievements

- Successfully isolated developer user assignments by grouping members under team scopes instead of standalone individuals.
- Enforced a secure multi-factor authentication (MFA) regime for administrative root channels.
- Removed high-risk static credentials by shifting human access paths over to short-term temporary credential sessions.
- Hardened service endpoints to accept execution requests exclusively within strict local office schedules and designated IPs.
- Confirmed operational trace monitoring using AWS CloudTrail audit logs during role testing sessions.

### Plan for Next Week

- Build the core cloud networking foundation to securely host backend computing nodes.
- Design and launch a multi-AZ Virtual Private Cloud (VPC) environment.