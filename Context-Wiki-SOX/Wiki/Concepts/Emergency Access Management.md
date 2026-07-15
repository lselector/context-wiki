---
type: concept
title: Emergency Access Management
description: Controlled, temporary elevated access ("firefighter" access) granted for emergencies under a formal regime of ownership, logging, and review.
tags:
  - emergency-access
  - firefighter
  - access-controls
  - sap
  - sox
---

Emergency Access Management (EAM) provides controlled, temporary elevated access — "firefighter" access — for emergencies, avoiding standing broad privileges that would violate [[Least Privilege]] and [[Segregation of Duties]]. [[SAP]] Access Control's EAM module is the reference implementation in the summaries.

Key facts:

- Each firefighter ID has an **Owner** (maintains assignments) and a **Controller** (reviews usage logs); firefighters log on via an EAM launchpad, must select reason codes and describe planned activities, and every session is logged, with logon notifications to controllers.
- Review reports create the [[Audit Trail]] auditors expect: Consolidated Log Report, Firefighter Log Summary, Reason Code and Activity Report, Transaction Log and Session Details, Invalid Emergency Access Report, and an SoD Conflict Report for firefighter IDs.
- Centralized and decentralized configurations are supported, with scheduled log-collection and master-data sync jobs.
- [[Oracle]] offers an analogous pattern: time-boxed elevated access granted for a limited window with activity monitoring, generating audit evidence instead of standing SoD violations.
- Firefighter session logs are part of the documented, re-performable evidence required for [[ICFR]] testing under the [[Sarbanes-Oxley Act]].

## Related concepts

[[Access Controls]], [[Segregation of Duties]], [[Least Privilege]], [[User Access Review]], [[Audit Trail]], [[IT General Controls]], [[SAP]]

## Sources

- [[sap_access_control_administration_guide]]
- [[oracle_advanced_access_controls_datasheet]]
