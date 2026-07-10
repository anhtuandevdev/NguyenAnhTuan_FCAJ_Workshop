---
title: "Week 3 Worklog"
date: 2026-06-15
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
---

### Week 3 Objectives

- Establish the core security perimeter using AWS Identity and Access Management (IAM)[cite: 5].
- Enforce the Principle of Least Privilege across administrative and operator accounts[cite: 10].
- Implement programmatic security access and temporary session tokens using IAM Roles and Conditions[cite: 10].

### Tasks Carried Out This Week

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 1 | Created specialized IAM Groups to categorize administrative, development, and operational operations[cite: 5]. | 06/15/2026 | 06/15/2026 | AWS IAM User Guide |
| 2 | Provisioned isolated IAM administrative users to eliminate the dangerous habit of using the root account directly[cite: 5]. | 06/16/2026 | 06/16/2026 | AWS Security Manual |
| 3 | Configured advanced IAM Roles incorporating custom JSON Policies with explicit 'Allow' and 'Deny' scopes[cite: 5, 10]. | 06/17/2026 | 06/17/2026 | JSON Schema Reference |
| 4 | Embedded strict Condition blocks inside policies based on corporate source IP addresses and specific time windows[cite: 10]. | 06/18/2026 | 06/18/2026 | AWS Policy Conditions |
| 5 | Tested the Assume Role workflow to acquire short-term real-time operational credentials via AWS STS[cite: 10]. | 06/19/2026 | 06/19/2026 | AWS STS Documentation |

### Week 3 Achievements

- Successfully isolated developer user assignments by grouping members under team scopes instead of standalone individuals[cite: 5, 10].
- Enforced a secure multi-factor authentication (MFA) regime for administrative root channels[cite: 3].
- Removed high-risk static credentials by shifting human access paths over to short-term temporary credential sessions[cite: 10].
- Hardened service endpoints to accept execution requests exclusively within strict local office schedules and designated IPs[cite: 10].
- Confirmed operational trace monitoring using AWS CloudTrail audit logs during role testing sessions[cite: 5].

### Plan for Next Week

- Build the core cloud networking foundation to securely host backend computing nodes.
- Design and launch a multi-AZ Virtual Private Cloud (VPC) environment[cite: 5].