---
type: summary
title: NetSuite Roles & Permissions - SoD Setup and Audit Guide
description: Houseblend guide (May 2026) on designing NetSuite roles and permissions to enforce segregation of duties and on auditing those controls with saved searches, system notes, and login audit trails for SOX compliance.
resource: https://houseblend.io/articles/pdfs/netsuite-roles-permissions-sod-audit.pdf
source_file: Raw/05_it_controls/netsuite_roles_permissions_sod_audit_guide.pdf
tags:
  - netsuite
  - segregation-of-duties
  - roles
  - permissions
  - audit
  - sox
---

## Overview

This 10-page Houseblend guide examines how to design, restrict,
and audit roles and permissions in [[NetSuite]] (acquired by
[[Oracle]] in 2016; 40,000+ customers) to implement robust
[[Segregation of Duties]]. It notes that SoD is a foundational
[[Internal Control]] recognized in the [[Sarbanes-Oxley Act]]
and [[COSO]] frameworks, and that SoD violations are the most
common classification of [[Material Weakness]] findings in ERP
audits.

## NetSuite role and permission architecture

- Role-based [[Access Controls]]: every user is assigned one
  or more roles; each role is linked to a "center" (UI for a
  business area) and bundles granular permissions grouped by
  type (Transactions, Lists, Reports, Setup).
- NetSuite defines 630+ distinct permissions governing nearly
  5,000 tasks and records; each grantable at levels such as
  None, View, Create, Edit, Full.
- Standard roles (Administrator, CFO, etc.) cannot be edited
  and should never be assigned directly — best practice is to
  clone and tailor them, granting only needed privileges
  ([[Least Privilege]]).
- Role restrictions limit data visibility by subsidiary,
  department, or class in OneWorld multi-entity accounts.
- Only administrators can create or modify roles; the
  Administrator role grants virtually every permission, so its
  assignment should be tightly limited.

## Setting up segregation of duties

- Map each critical process (procure-to-pay, order-to-cash,
  financial close, payroll, system administration) and ensure
  no single role spans incompatible steps.
- Example role splits: a "Vendor Manager" role (vendor
  creation, bank details) separate from an "AP Specialist"
  role (bill entry, payments); "Order Entry" separate from
  "Cash Application"; GL posting separate from reconciliation
  and reporting; HR master-data changes separate from payroll
  processing; user-account creation separate from role
  granting.
- Where full separation is impossible (small teams), use
  [[Compensating Controls]]: e.g., a CFO's documented weekly
  review of new vendors alongside payments issued, supported
  by a saved search.
- SuiteFlow approval workflows encode oversight (multi-level
  PO approval, journal-entry review thresholds); period
  locking prevents backdated GL postings.
- Access provisioning should itself be segregated: request,
  approval, and granting handled by different people, with
  documented approvals.

## Auditing roles and permissions

- Saved searches on Role and Employee records list effective
  permissions per user/role and can flag conflicting
  combinations (e.g., a role holding both "Create Vendor" and
  "Issue Vendor Payment"); they can be scheduled and delivered
  to compliance officers.
- Login Audit Trail records every sign-in (user, timestamp,
  IP) to detect unauthorized or anomalous access.
- System Notes provide an automatic [[Audit Trail]] of all
  data and configuration changes (old/new values, user, date),
  including changes to roles themselves — essential forensic
  evidence.
- SuiteAnalytics dashboards and alerts enable [[Continuous Controls Monitoring]] of privilege counts and SoD-like
  anomalies.
- Periodic [[User Access Review]] (quarterly/annual) verifies
  role assignments still match job duties and prevents role
  bloat; role changes require logged approvals under formal
  [[Change Management]].

## SOX relevance and case examples

- Under [[SOX Section 404]], auditors explicitly test SoD in
  financial processes; poorly designed NetSuite roles are a
  frequent audit finding.
- Case studies: a Baker Tilly client's new NetSuite instance
  had roles "not set up to be compliant with proper
  segregation of duties" and required role/workflow redesign;
  a Moss Adams client's roles were found not SOX-compliant and
  were remediated with reconfigured roles plus mitigating
  workflow approvals; a Singapore manufacturer with no SoD
  framework had large numbers of violations until it built a
  rule-based SoD engine with scheduled violation queries.
- Two-factor authentication, IP restrictions, and session
  controls protect SoD boundaries against credential
  compromise — supporting the broader [[IT General Controls]]
  security domain relied on for [[ICFR]].

## Related concepts

- [[Segregation of Duties]]
- [[Access Controls]]
- [[Role-Based Access Control]]
- [[Least Privilege]]
- [[Compensating Controls]]
- [[Audit Trail]]
- [[User Access Review]]
- [[Change Management]]
- [[Material Weakness]]
- [[SOX Section 404]]
- [[COSO]]
- [[NetSuite]]
