---
type: concept
title: Least Privilege
description: The principle of granting users only the minimum access needed for their job duties, reducing fraud and error risk in financial systems.
tags:
  - least-privilege
  - access-controls
  - security
  - sox
---

Least privilege is the security principle of granting each user only the minimum access required for their job duties. In ERP-based SOX compliance it underpins role design and [[Access Controls]] over financial applications.

Key facts:

- [[NetSuite]] best practice: never assign broad standard roles (Administrator, CFO) directly — clone and tailor them, granting only needed privileges; define minimal-permission roles and run periodic role-access reports.
- Field-level permissions and role restrictions (by subsidiary, department, or class) narrow access further; the Administrator role, which grants virtually every permission, should be tightly limited.
- Least privilege supports [[Segregation of Duties]]: minimal roles make incompatible-duty combinations less likely, and [[User Access Review]] campaigns prevent "role bloat" as duties change.
- Alternatives to standing broad access include time-boxed elevated access with activity monitoring ([[Oracle]]) and firefighter IDs under [[Emergency Access Management]] ([[SAP]]).

## Related concepts

[[Access Controls]], [[Role-Based Access Control]], [[Segregation of Duties]], [[User Access Review]], [[Emergency Access Management]], [[IT General Controls]]

## Sources

- [[netsuite_roles_permissions_sod_audit_guide]]
- [[netsuite_grc_native_compliance_features]]
- [[oracle_advanced_access_controls_datasheet]]
- [[sap_access_control_administration_guide]]
