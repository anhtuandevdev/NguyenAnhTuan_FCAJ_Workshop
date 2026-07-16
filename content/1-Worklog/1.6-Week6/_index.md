---
title: "Week 6 Worklog"
date: 2026-05-22
weight: 6
chapter: false
pre: " <b> 1.6. </b> "
---

### Week 6 Objectives

- Deploy compute instances inside private zones to simulate smart home virtual sensor endpoints.
- Formulate execution logic nodes compiling mock telemetry logs representing appliance metrics.
- Confirm steady end-to-end communication pathways from isolated private instances out to internet boundaries.

### Tasks Carried Out This Week

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 1 | Provisioned virtual compute nodes using standard Amazon Linux instances deployed within private subnets. | 22/05/2026 | 22/05/2026 | EC2 Launch Profiles |
| 2 | Wrote telemetry generator scripts modeling voltage levels, power spikes, and virtual sensor states. | 23/05/2026 | 23/05/2026 | Node.js Programming |
| 3 | Attached dedicated EC2 Instance Profiles giving internal virtual machines explicit secure communication authorization. | 24/05/2026 | 24/05/2026 | AWS Instance Profile Guide |
| 4 | Verified routing paths from internal processing systems out to public addresses through the NAT Gateway. | 25/05/2026 | 25/05/2026 | Network Diagnostic Tools |
| 5 | Audited execution flows using CloudWatch monitoring logs to catch transmission drops or script faults. | 26/05/2026 | 26/05/2026 | CloudWatch Logs Manual |

### Week 6 Achievements

- Successfully configured isolated compute nodes that emit streaming data without opening dangerous public ingress exposures.
- Removed high-risk hardcoded secret variables from application directories by utilizing programmatic token assignments.
- Validated real-time streaming connections from inside isolated zones out to public target receivers.
- Assured stable telemetry processing behaviors with zero runtime pipeline drops.
- Completed the foundational environment setup required for data collection workloads.

### Plan for Next Week

- Establish durable structural storage layers to aggregate historical smart home tracking files.
- Configure asset buckets using Amazon Simple Storage Service (S3).