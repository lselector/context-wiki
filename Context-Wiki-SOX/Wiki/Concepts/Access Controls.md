---
type: concept
title: Access Controls
description: Controls restricting who can access programs, data, and transactions — a core ITGC domain enforced through roles, permissions, provisioning workflows, and monitoring.
tags:
  - access-controls
  - security
  - itgc
  - sox
---

Access controls restrict who can access programs, data, and transactions. "Access to programs and data" is one of the classic [[IT General Controls]] domains (SEC Release 33-8810), and access controls are the primary enforcement mechanism for [[Segregation of Duties]] and [[Least Privilege]].

Key facts:

- [[Protiviti]]: **44%** of organizations say IT access controls and security is the SOX area with the most challenges or deficiencies — SoD conflicts, gaps in user access reviews, and untimely terminations.
- Lifecycle coverage: role design, provisioning (workflow-approved access requests), certification ([[User Access Review]]), usage monitoring, and emergency access ([[Emergency Access Management]]).
- [[Oracle]] Advanced Access Controls continuously monitors all access policies in ERP Cloud, scanning full access paths (role hierarchies, user assignments, privileges) with visualization, simulation, and time-boxed elevated access; Fusion RMC adds preventive SoD checks during provisioning and monitoring of superuser and nonhuman (API) accounts.
- [[SAP]] Access Control provides access requests, risk analysis, business role management, emergency access, and periodic reviews across SAP and non-SAP systems.
- [[NetSuite]] enforces role-based security and field-level permissions with MFA, IP restrictions, and a Login [[Audit Trail]]; all permission changes are logged for auditors.
- Auditing access privileges provides objective evidence for [[ICFR]] and [[SOX Section 404]] assessments.

## Related concepts

[[Role-Based Access Control]], [[Segregation of Duties]], [[Least Privilege]], [[User Access Review]], [[Emergency Access Management]], [[IT General Controls]], [[Audit Trail]]

## Sources

- [[oracle_advanced_access_controls_datasheet]]
- [[oracle_fusion_risk_management_cloud_datasheet]]
- [[sap_access_control_administration_guide]]
- [[netsuite_grc_native_compliance_features]]
- [[netsuite_roles_permissions_sod_audit_guide]]
- [[protiviti_2024_sox_compliance_survey]]
- [[sec_release_33-8810_mgmt_guidance_icfr]]
