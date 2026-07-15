---
type: concept
title: Change Management
description: The ITGC discipline of controlling changes to programs, configurations, and roles — sandbox testing, documented approvals, and change logs — so systems keep operating as designed.
tags:
  - change-management
  - itgc
  - sdlc
  - sox
---

Change management is the [[IT General Controls]] discipline of controlling changes to programs, configurations, and security roles so financial systems keep operating as designed. "Program change" is one of the classic ITGC domains (SEC Release 33-8810), and weak change management over a financial application is a textbook ITGC deficiency assessed via the [[GAIT Methodology]].

Key facts:

- [[NetSuite]] best practices: SuiteCloud Development Framework, sandbox testing, a documented SDLC, and change logs; role changes require logged approvals under formal change management, and system notes record every configuration change (see [[Audit Trail]]).
- COSO's monitoring guidance embeds change in its baseline cycle: control baseline → change identification → change management → control revalidation/update; systems fail when the environment changes (risks, people, processes, technology) without corresponding design changes.
- [[GAIT Methodology]] explicitly considers unauthorized-change risk to data and the role of compensating business-process controls.
- [[SAP]] role management reports (PFCG change history, master-to-derived role relationships) support ITGC change-tracking assertions.
- Business change drives deficiencies: [[EY]] found new ERP implementations (37% of companies) and other transformations caused increased control deficiencies; [[Protiviti]] notes ERP implementations and upgrades introduce further access risk.

## Related concepts

[[IT General Controls]], [[Audit Trail]], [[GAIT Methodology]], [[Access Controls]], [[Monitoring of Internal Control]], [[Role-Based Access Control]]

## Sources

- [[netsuite_grc_native_compliance_features]]
- [[netsuite_roles_permissions_sod_audit_guide]]
- [[coso_guidance_on_monitoring_internal_control_systems]]
- [[iia_gait_itgc_deficiency_assessment]]
- [[sap_access_control_administration_guide]]
- [[ey_global_sox_survey_results]]
