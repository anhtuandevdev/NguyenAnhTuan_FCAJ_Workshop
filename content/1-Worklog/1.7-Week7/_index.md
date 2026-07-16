---
title: "Week 7 Worklog"
date: 2026-05-29
weight: 7
chapter: false
pre: " <b> 1.7. </b> "
---

### Week 7 Objectives

- Deploy high-durability object storage repositories to log incoming sensor historical captures.
- Master global naming specifications and path conventions across cloud data lakes.
- Implement cost-effective storage lifecycle rules to shift older data archives onto budget tiers.

### Tasks Carried Out This Week

| Day | Task | Start Date | Completion Date | Reference Material |
| --- | --- | --- | --- | --- |
| 1 | Created high-capacity data buckets configured with globally unique naming labels on Amazon S3. | 29/05/2026 | 29/05/2026 | Amazon S3 Core Guide |
| 2 | Established structured object folder schemas organizing files into granular sensor type blocks. | 30/05/2026 | 30/05/2026 | S3 Folder Best Practices |
| 3 | Programmed file ingestion scripts uploading raw JSON readings directly to secure S3 destinations. | 31/05/2026 | 31/05/2026 | S3 API Reference |
| 4 | Implemented automatic bucket S3 Lifecycle Policies mapping aging telemetry logs into colder tiers. | 01/06/2026 | 01/06/2026 | S3 Lifecycle Manual |
| 5 | Conducted data access simulation checks validating retrieval times for active versus archived states. | 02/06/2026 | 02/06/2026 | AWS Storage IA Testing |

### Week 7 Achievements

- Built an object storage workspace featuring data durability guarantees.
- Applied optimized bucket partitions separating active tracking data streams from long-term compliance storage.
- Cut overall storage overhead risks by staging aging objects to transition directly into cold Glacier deep layers.
- Hardened access points by blocking public visual permissions across sensitive file boundaries.
- Demonstrated scalable target destination performance matching planned volume expectations.

### Plan for Next Week

- Protect telemetry log lakes against corruption or accidental loss events.
- Implement automated snapshot rules using AWS Backup management solutions.