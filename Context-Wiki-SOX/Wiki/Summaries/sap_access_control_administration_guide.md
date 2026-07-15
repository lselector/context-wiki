---
type: summary
title: SAP Access Control 10.1 Administration Guide
description: SAP's 258-page administration guide for SAP Access Control 10.1, the GRC application for access requests, access risk (SoD) analysis, business role management, emergency access ("firefighter") management, and periodic access reviews.
resource: https://help.sap.com/doc/ca8a8544445e47f5bb0cbc8220ae01b2/10.1.18/en-US/loio8bdd50b2b1f34e049c45ded84788789c_8bdd50b2b1f34e049c45ded84788789c_EN.pdf
source_file: Raw/05_it_controls/sap_access_control_administration_guide.pdf
tags:
  - sap
  - grc
  - access-control
  - segregation-of-duties
  - emergency-access
  - sox
---

## Overview

SAP Access Control 10.1 (an add-on to SAP NetWeaver 7.40,
guide published 2017) is [[SAP]]'s enterprise application for
access governance: it "enables organizations to control access
and prevent fraud across the enterprise, while minimizing the
time and cost of compliance." It works with SAP applications
(Finance, Sales and Distribution) and non-SAP systems such as
[[Oracle]] and JD Edwards, and integrates with SAP Process
Control and SAP Risk Management. Its capabilities map directly
to the [[Access Controls]] and [[Segregation of Duties]]
requirements tested in [[SOX Section 404]] audits of [[ICFR]].

## Core modules

- Access Requests (ARQ) — workflow-driven creation and
  approval of user access requests. Approvers must review SoD
  and access risks before approving, rejecting, or modifying a
  request; provisioning logs record the outcome.
- Access Risk Analysis (ARA) — the SoD engine. Security
  analysts and business process owners run risk analysis at
  user, role, profile, and HR-object level, identify root
  causes of violations, simulate changes, and remediate or
  mitigate risks.
- Business Role Management (BRM) — role lifecycle management:
  role creation methodology, role maintenance with built-in
  risk analysis, role mining, role comparison, role reaffirm,
  and mass maintenance.
- Emergency Access Management (EAM) — controlled "firefighter"
  access for emergencies (see below).
- Periodic Reviews — recurring [[User Access Review]] and SoD
  review campaigns with workflow, reviewer assignment, and
  history reporting.

## Access risk analysis and SoD rules

- Rule architecture: access risks are defined from functions
  (groups of actions/permissions); the system generates a
  distinct rule for each conflicting action combination and
  target system (e.g., one risk can expand to tens of
  thousands of generated rules; hard cap 1,679,615 rules per
  risk).
- Rule setup includes exception access rules, organization
  rules (scoping by org level), supplementary rules (to
  suppress or include false positives via table lookups), and
  critical access rules for sensitive single-function access.
- Simulation: user-level and role-level "what-if" analysis
  shows the SoD impact of proposed access before it is granted
  — a preventive [[Internal Control]].
- Mitigation: where conflicts cannot be removed, [[Compensating Controls|Mitigating Controls]] are assigned to users, roles, profiles, or HR
  objects with owners, monitors, and validity periods; alerts
  flag conflicting or critical action execution.
- Risk analysis is embedded at every entry point: submitting
  requests, approving requests, and maintaining roles.

## Emergency Access Management (firefighting)

- Firefighter IDs grant temporary, elevated emergency access
  under a formal control regime: each ID has an Owner (who
  maintains assignments) and a Controller (who reviews usage
  logs).
- Firefighters log on via an EAM launchpad, must select reason
  codes and describe planned activities, and every session is
  logged; controllers receive logon notifications.
- Review reports create the [[Audit Trail]] auditors expect:
  Consolidated Log Report, Firefighter Log Summary, Reason
  Code and Activity Report, Transaction Log and Session
  Details, Invalid Emergency Access Report, and an SoD
  Conflict Report for Firefighter IDs.
- Centralized and decentralized configurations are supported,
  with scheduled log-collection and master-data sync jobs.

## Reporting and dashboards

- Access dashboards: risk violations, user analysis, role
  analysis, alerts, mitigating control library, access rule
  library, provisioning, and service-level dashboards.
- Access risk analysis reports: user/role/profile risk
  violation reports, access rule summary/detail, mitigating
  control and mitigated-object reports.
- Access request reports: requests with conflicts and
  mitigations, SoD review history, user access review history
  — evidence packages for [[External Auditor]] testing.
- Role management reports include PFCG change history and
  master-to-derived role relationship reports supporting
  [[IT General Controls]] change-tracking assertions.

## Support for SOX 404 compliance

- Preventive SoD checking during provisioning plus detective
  batch risk analysis together operationalize [[Segregation of Duties]], the most commonly cited access-related source of a
  [[Material Weakness]].
- Workflow approvals, provisioning logs, periodic [[User Access Review]] campaigns, and firefighter session logs
  provide the documented, re-performable evidence required for
  [[ICFR]] testing under the [[Sarbanes-Oxley Act]].
- Ongoing alerting and scheduled background risk-analysis jobs
  are a form of [[Continuous Controls Monitoring]] over ERP
  access.

## Related concepts

- [[Segregation of Duties]]
- [[Access Controls]]
- [[Emergency Access Management]]
- [[User Access Review]]
- [[Compensating Controls|Mitigating Controls]]
- [[Audit Trail]]
- [[Role-Based Access Control]]
- [[IT General Controls]]
- [[SOX Section 404]]
- [[SAP]]
