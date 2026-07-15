---
type: concept
title: Compensating Controls
description: Controls that mitigate the risk left by a deficient or missing control; called "mitigating controls" in SAP GRC terminology.
tags: [compensating-controls, mitigating-controls, deficiency, sod]
---

Compensating controls are controls that achieve, or partially
achieve, a control objective when another control is deficient or
impractical — for example when full [[Segregation of Duties]] is
impossible in a small team. [[SAP]] GRC products call these
"mitigating controls"; the two terms describe the same idea.

Key facts:
- Under [[AS 2201]] and SEC guidance, deficiency severity is
  evaluated considering compensating controls; [[AU-C 940]]
  requires the auditor to test them before relying on them.
- [[FEI]] argued downstream compensating controls (account
  reconciliations, supervisory reviews) usually mitigate
  [[IT General Controls]] failures — a premise of the
  [[GAIT Methodology]] reliance chain.
- SAP Access Control assigns mitigating controls to users, roles,
  profiles, or HR objects with owners, monitors, and validity
  periods when SoD conflicts cannot be remediated.
- Practical examples: a CFO's documented weekly review of new
  vendors and payments (NetSuite small-team SoD); Oracle Advanced
  Financial Controls transaction monitoring deployed over accepted
  access conflicts.

## Related concepts
[[Material Weakness]], [[Significant Deficiency]],
[[Segregation of Duties]], [[IT General Controls]],
[[Key Controls]]

## Sources
[[pcaob_as_2201_audit_of_icfr_standard]],
[[sec_release_33-8810_mgmt_guidance_icfr]],
[[fei_comment_letter_pcaob_as5_icfr_audit_2007]],
[[sap_access_control_administration_guide]],
[[netsuite_roles_permissions_sod_audit_guide]],
[[oracle_advanced_access_controls_datasheet]]
