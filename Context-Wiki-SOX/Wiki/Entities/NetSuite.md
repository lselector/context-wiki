---
type: company
title: NetSuite
description: Oracle-owned cloud ERP (40,000+ customers) whose native audit trails, role-based security, and workflow controls support SOX 404 compliance.
tags: [netsuite, erp, grc, sox]
---

NetSuite is a cloud ERP acquired by [[Oracle]] in 2016, with
40,000+ customers. Its built-in GRC features map directly to
[[SOX Section 404]] control objectives over [[ICFR]].

Key facts:
- Always-on [[Audit Trail]] ("system notes") records user,
  timestamp, and before/after values for all transaction and
  configuration changes; a Login Audit Trail records every sign-in.
- Role-based security: 630+ permissions across nearly 5,000 tasks;
  standard roles should be cloned, not assigned, following
  [[Least Privilege]]; role restrictions scope data by subsidiary
  or department.
- SuiteFlow approval workflows, period locking, and saved-search
  alerts enforce [[Internal Control]] and flag
  [[Segregation of Duties]] conflicts — a form of
  [[Continuous Controls Monitoring]].
- Carries SOC 1 Type II / SOC 2 Type II attestations; auditors can
  rely on its [[SOC 1 Report]] to reduce direct
  [[IT General Controls]] testing.

## Related concepts
[[Oracle]], [[Audit Trail]], [[Segregation of Duties]],
[[Access Controls]], [[Role-Based Access Control]], [[SOC 1 Report]]

## Sources
[[netsuite_grc_native_compliance_features]],
[[netsuite_roles_permissions_sod_audit_guide]]
