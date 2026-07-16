---
title: "Week 4 Worklog"
date: 2026-05-08
weight: 4
chapter: false
pre: " <b> 1.4. </b> "
---

### Week 4 Objectives

- Architect a robust, secure, and isolated Amazon Virtual Private Cloud (VPC) network infrastructure.
- Isolate public-facing components from internal backend databases across distinct Availability Zones (AZ).
- Eliminate common security vulnerabilities by removing direct external entry points into private networks.

### Tasks Carried Out This Week

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 1 | Provisioned an initial custom core network mapping using a dedicated Classless Inter-Domain Routing (CIDR) block. | 08/05/2026 | 08/05/2026 | VPC Networking Guide |
| 2 | Divided the network infrastructure symmetrically across separate availability layers into Public and Private Subnets. | 09/05/2026 | 09/05/2026 | Subnet Planning Tools |
| 3 | Deployed an Internet Gateway (IGW) and mapped border routes out to public pathways across public tables. | 10/05/2026 | 10/05/2026 | AWS Routing Reference |
| 4 | Provisioned an elastic NAT Gateway inside the public layer to bridge outbound internet connectivity for private nodes. | 11/05/2026 | 11/05/2026 | NAT Gateway Manual |
| 5 | Set up an EC2 Instance Connect Endpoint (EICE) to execute native terminal commands directly over the console without public IPs. | 12/05/2026 | 12/05/2026 | Systems Manager Docs |

### Week 4 Achievements

- Successfully executed network segregation splits providing High Availability (HA) protections.
- Granted private databases secure access to download outbound security packages while keeping incoming pathways entirely hidden.
- Disabled traditional insecure edge bastion host boxes, entirely eliminating target scanning surfaces on port 22.
- Conducted exhaustive routing trace verifications achieving 0% packet loss performance scores.
- Established foundational VPC Flow Logs channels capturing real-time tracking streams toward CloudWatch Log Groups.

### Plan for Next Week

- Create cost management frameworks and spending thresholds.
- Implement detailed financial cost budgeting models using AWS Budgets dashboards.