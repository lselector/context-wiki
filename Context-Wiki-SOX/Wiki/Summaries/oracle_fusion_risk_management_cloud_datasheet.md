---
type: summary
title: Oracle Fusion Cloud Risk Management and Compliance (datasheet)
description: Oracle datasheet (v4.0, 2026) describing the Risk Management and Compliance module of Oracle Fusion Cloud ERP, which uses embedded AI and 300+ algorithms for continuous SoD, access, configuration, and transaction monitoring in support of SOX and ICFR.
resource: https://www.oracle.com/a/ocom/docs/applications/erp/oracle-risk-management-cloud-ds.pdf
source_file: Raw/05_it_controls/oracle_fusion_risk_management_cloud_datasheet.pdf
tags:
  - oracle
  - risk-management
  - icfr
  - sox
  - continuous-monitoring
  - ai
  - erp
---

## Overview

This [[Oracle]] datasheet (version 4.0, 2026; text recovered
via OCR from an image-based PDF) describes Oracle Fusion Cloud
Risk Management and Compliance (RMC), an Oracle Cloud ERP
module that helps manage cybersecurity risk in Fusion SaaS,
enforce [[ICFR]], meet [[Sarbanes-Oxley Act]] ([[SOX Section 404]]) compliance requirements, and ensure audit readiness.
RMC positions audit as data-driven continuous assurance rather
than a "check the box" exercise, using embedded AI and 300+
prebuilt algorithms to monitor millions of transactions,
configuration changes, and user access events.

## Included and related modules

- Advanced Access Controls — ensures [[Segregation of Duties]] in role design, provisioning, and ongoing access.
- Advanced Financial Controls — monitors actual financial
  transactions for fraud, error, and policy breaches.
- Financial Reporting Compliance — streamlines internal
  assessments and [[Internal Control]] certification.
- Advanced HCM Controls (related module) — the equivalent
  monitoring product for HCM user access and activity.

## Key features

- Automated monitoring of intra-role violations to prevent
  inherent risk in ERP role design.
- Preventive SoD analysis during user access provisioning —
  violations are caught before access is granted.
- Deep SoD analysis with visualization and simulation of
  conflicts, plus monitoring of actual SoD violations in
  transactions (not just potential access).
- [[Continuous Controls Monitoring]] of sensitive ERP
  configurations and critical ERP transactions.
- Monitoring of IT admin/superuser, business superuser, and
  nonhuman (API/integration) account access and activity,
  including [[Audit Trail]] monitoring for risky drift.
- Library of pre-built algorithms plus an intuitive workbench
  for authoring custom algorithms; 28,000+ business data
  points and reference control frameworks for ICFR and
  cybersecurity.
- Graphical, persona-based dashboards for actionable insight.

## AI agents

- Certification Advisor — generates plain-language briefings
  for each user/role decision in [[User Access Review]] and
  certification campaigns (role contents, peer comparison,
  incident history), producing documented rationale and
  stronger audit evidence.
- ERP Access Assistant — guides business users through role
  requests, auto-builds the request, runs preventive SoD and
  security analysis, and gives approvers a plain-language risk
  summary with audit-ready evidence by default.
- Assurance Advisor — assesses internal controls across
  source-to-settle, record-to-report, order-to-cash, and
  hire-to-retire processes using 100+ algorithms; flags toxic
  access combinations, SoD-violating transactions, duplicate
  suppliers, and at-risk control objectives.

## Example SoD algorithms (source-to-settle)

- Create Suppliers and Create Payables Invoices (same user).
- Maintain Supplier Bank Accounts and Create Payables Invoices.
- Payables invoices approved and payment created by same user.
- Suppliers and purchase orders managed by the same user.
- Detection of unauthorized suppliers and payments.

## Support for SOX 404 compliance

- Streamlines assessment and certification of [[ICFR]] for
  [[SOX Section 404]] assurance and audit readiness, giving
  process owners data-backed confidence when certifying
  controls.
- Automates [[Access Controls]] enforcement (preventive) and
  violation detection (detective) across the access lifecycle
  — role design, provisioning, certification, and usage.
- Full transaction monitoring supplies evidence about actual
  control operation, which supports [[External Auditor]]
  reliance and reduces manual testing.
- Native embedding in Oracle Fusion Cloud avoids risky data
  exports and patchwork integrations, keeping the monitoring
  itself within a controlled [[IT General Controls]]
  environment.
- Continuous monitoring/audit of configurations and
  transactions operationalizes [[Continuous Controls Monitoring]] and helps avoid audit surprises such as a
  late-discovered [[Material Weakness]].

## Related concepts

- [[ICFR]]
- [[SOX Section 404]]
- [[Segregation of Duties]]
- [[Access Controls]]
- [[Continuous Controls Monitoring]]
- [[Audit Trail]]
- [[User Access Review]]
- [[User Access Review|Access Certification]]
- [[Internal Control]]
- [[Oracle]]
