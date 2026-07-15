---
type: concept
title: Role-Based Access Control
description: Granting system access through roles that bundle permissions aligned to job duties (RBAC) — the standard ERP mechanism for enforcing least privilege and segregation of duties.
tags:
  - rbac
  - access-controls
  - roles
  - erp
---

Role-Based Access Control (RBAC) grants system access through roles — named bundles of permissions aligned to job duties — rather than assigning permissions directly to users. It is the standard ERP mechanism for enforcing [[Least Privilege]] and [[Segregation of Duties]].

Key facts:

- [[NetSuite]]: every user is assigned one or more roles tied to a "center"; the platform defines **630+ distinct permissions governing nearly 5,000 tasks and records**, each grantable at levels (None, View, Create, Edit, Full). Standard roles cannot be edited and should never be assigned directly — best practice is to clone and tailor them; role restrictions limit data by subsidiary, department, or class; the Administrator role should be tightly limited.
- [[SAP]] Access Control's Business Role Management covers the role lifecycle: creation methodology, maintenance with built-in risk analysis, role mining, comparison, reaffirm, and mass maintenance.
- [[Oracle]] warns that coarse-grained SoD analysis of composite/enterprise roles becomes inaccurate over time; fine-grained analysis of full access paths (role → privilege) is needed, and identifying intra-role conflicts lets organizations design SoD-clean roles before go-live.
- Only administrators should create or modify roles, and role changes require logged approvals under formal [[Change Management]].

## Related concepts

[[Access Controls]], [[Least Privilege]], [[Segregation of Duties]], [[User Access Review]], [[Change Management]], [[NetSuite]], [[SAP]], [[Oracle]]

## Sources

- [[netsuite_roles_permissions_sod_audit_guide]]
- [[netsuite_grc_native_compliance_features]]
- [[sap_access_control_administration_guide]]
- [[oracle_advanced_access_controls_datasheet]]
