---
type: concept
title: Audit Trail
description: System-generated, tamper-evident logs of transactions, data changes, configuration changes, and logins — recording who did what and when — that provide forensic evidence for audits.
tags:
  - audit-trail
  - logging
  - evidence
  - itgc
  - sox
---

An audit trail is the system-generated record of transactions, data and configuration changes, and logins — capturing user, timestamp, and before/after values — that lets auditors reconstruct who did what and when. It is foundational evidence for [[ICFR]] testing and [[IT General Controls]].

Key facts:

- [[NetSuite]]: an always-on audit trail and "system notes" cover all transactions and configuration changes (user, timestamp, before/after values) with drill-down from summary reports to each record; the Login Audit Trail records every sign-in (user, timestamp, IP); system notes also log changes to roles themselves — essential forensic evidence.
- [[SAP]] Access Control: provisioning logs, firefighter session logs, and review reports (Consolidated Log Report, Transaction Log and Session Details) form the audit trail for [[Emergency Access Management]].
- [[Oracle]] Fusion RMC monitors audit trails for "risky drift" and logs superuser and nonhuman (API/integration) account activity.
- Detailed transaction logs and system notes let companies support management's [[SOX Section 404]] assertions with system documentation for the [[External Auditor]]; saved-search alerts on sensitive changes (large journal adjustments, employee record changes) turn the trail into [[Continuous Controls Monitoring]].

## Related concepts

[[IT General Controls]], [[Access Controls]], [[Change Management]], [[Emergency Access Management]], [[Continuous Controls Monitoring]], [[Journal Entry Controls]]

## Sources

- [[netsuite_grc_native_compliance_features]]
- [[netsuite_roles_permissions_sod_audit_guide]]
- [[sap_access_control_administration_guide]]
- [[oracle_fusion_risk_management_cloud_datasheet]]
