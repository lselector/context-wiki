---
type: concept
title: Segregation of Duties
description: Dividing incompatible duties (e.g., creating vendors vs. paying them) among different people so no one person can both perpetrate and conceal errors or fraud.
tags:
  - sod
  - access-controls
  - fraud-prevention
  - sox
  - internal-control
---

Segregation of duties (SoD) divides incompatible duties among different people so no single person can execute an end-to-end financial transaction or both perpetrate and conceal errors or fraud. The [[COSO Internal Control Framework]] builds SoD into [[Control Activities]], with alternative controls where separation is not practical (per [[AS 2201]], smaller companies may use alternative controls).

Key facts:

- SoD violations are **the most common classification of [[Material Weakness]] findings in ERP audits** (Houseblend/NetSuite guide); under [[SOX Section 404]], auditors explicitly test SoD in financial processes.
- Classic conflicting-duty pairs (Oracle/SAP/NetSuite libraries): create suppliers vs. create payables invoices; maintain supplier bank accounts vs. create invoices; approve invoices vs. create payments; reconcile bank accounts vs. enter receipts; GL posting vs. reconciliation; HR master-data changes vs. payroll.
- Tooling: [[Oracle]] Advanced Access Controls (prebuilt SoD library over 6,000+ entitlements, fine-grained full-path scans, simulation); [[SAP]] Access Control's Access Risk Analysis engine (rules generated per conflicting action combination, preventive checks at provisioning, mitigating controls); [[NetSuite]] role design plus saved-search conflict detection.
- Where full separation is impossible (small teams), use [[Compensating Controls]] — e.g., a CFO's documented weekly review of new vendors alongside payments issued.
- [[Protiviti]]: hybrid work and shared services increase SoD challenges; visualization tools identify SoD violations at role and user level and support quantifying SoD deficiencies.

## Related concepts

[[Access Controls]], [[Role-Based Access Control]], [[Least Privilege]], [[User Access Review]], [[Compensating Controls]], [[Fraud Risk]], [[IT General Controls]], [[Control Activities]]

## Sources

- [[netsuite_roles_permissions_sod_audit_guide]]
- [[oracle_advanced_access_controls_datasheet]]
- [[oracle_fusion_risk_management_cloud_datasheet]]
- [[sap_access_control_administration_guide]]
- [[protiviti_2024_sox_compliance_survey]]
- [[coso_ic_framework_2013_executive_summary]]
- [[pcaob_as_2201_audit_of_icfr_standard]]
