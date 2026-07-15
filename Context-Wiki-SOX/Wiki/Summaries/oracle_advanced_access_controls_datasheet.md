---
type: summary
title: Oracle Advanced Access Controls Cloud Service (datasheet)
description: Oracle datasheet describing the Advanced Access Controls (AAC) Cloud Service for continuous, fine-grained monitoring of access policies and segregation-of-duties conflicts in Oracle ERP Cloud.
resource: https://www.oracle.com/a/ocom/docs/applications/erp/oracle-adv-access-controls-cloud-ds.pdf
source_file: Raw/05_it_controls/oracle_advanced_access_controls_datasheet.pdf
tags:
  - oracle
  - access-controls
  - segregation-of-duties
  - continuous-monitoring
  - erp
  - sox
---

## Overview

This [[Oracle]] datasheet (version 0119) describes Advanced
Access Controls (AAC) Cloud Service, a module embedded in
Oracle ERP Cloud that enables [[Continuous Controls Monitoring]] of access policies, potential violations, insider
threats, and fraud. AAC automates security analysis to enforce
[[Segregation of Duties]] and access-policy compliance, and is
positioned explicitly as a tool for meeting audit requirements
and mandates such as the [[Sarbanes-Oxley Act]].

## Key capabilities

- Continuous monitoring of all [[Access Controls]] policies in
  Oracle ERP Cloud.
- Pre-built library of best-practice SoD controls, drawing on
  6,000+ ERP Cloud access entitlements and access points.
- Graphical authoring workbench: users build new access
  controls with conditional filters and Boolean logic (AND/OR)
  without coding.
- Complete scans of full access paths — role hierarchies, user
  assignments, functional and data privileges — to detect users
  whose combined privileges violate SoD policies, while
  eliminating false positives.
- Fine-grained analysis: the datasheet argues that
  coarse-grained SoD analysis of composite/enterprise roles
  becomes inaccurate over time and leads to audit objections;
  only fine-grained, pre-integrated analysis is scalable.
- Visualization of access paths from role to privilege to
  identify the root cause of each conflict.
- Simulation of remediation actions before deployment, plus
  automatic closure of conflicts once resolved.
- Embedded dashboards with analytics for executives.

## Segregation of duties and remediation

- Example conflicting-duty pairs from the pre-built library:
  reconcile bank accounts vs. enter customer receipts; create
  payments vs. create purchase orders; create payables
  invoices vs. receive goods and services.
- Organizations can remediate conflicts (redesign roles) or
  accept them and deploy compensating transaction-monitoring
  controls via the companion Advanced Financial Controls
  service — a pragmatic balance between control and
  productivity.
- Time-boxed elevated access: rather than changing role
  definitions, temporary excess privileges can be granted for a
  limited window with activity monitoring, generating audit
  evidence — a controlled alternative to standing SoD
  violations.
- Role optimization: identifying intra-role conflicts lets
  organizations design SoD-clean roles before Cloud ERP
  go-live.

## Support for SOX 404 compliance

- Auditing access privileges provides objective evidence for
  [[ICFR]] and [[SOX Section 404]] assessments; control
  analysis results are documented as verifiable audit evidence.
- Access certification workflows document SoD analysis results
  and force line-manager review of privileges, reinforcing
  accountability — a recurring [[External Auditor]] request.
- Integration with Oracle Financial Reporting Compliance Cloud
  links access-analysis results to documented financial
  reporting risks and [[Internal Control]] frameworks.
- Fraud prevention by ensuring no user can perform end-to-end
  financial transactions independently addresses the classic
  SoD assertions tested in [[IT General Controls]] and
  [[IT Application Controls]] reviews.
- Continuous, automated detection replaces periodic manual
  reviews, an example of [[Continuous Controls Monitoring]]
  reducing audit cost and detecting issues between assessment
  cycles.

## Related services

- Oracle Financial Reporting Compliance Cloud Service
  (internal assessments and compliance).
- Oracle Advanced Financial Controls Cloud Service
  (transaction monitoring / compensating controls).
- Oracle Cloud Access Security Broker (multi-cloud and network
  monitoring).

## Related concepts

- [[Segregation of Duties]]
- [[Access Controls]]
- [[Continuous Controls Monitoring]]
- [[SOX Section 404]]
- [[ICFR]]
- [[IT General Controls]]
- [[Compensating Controls]]
- [[User Access Review|Access Certification]]
- [[Role-Based Access Control]]
- [[Oracle]]
