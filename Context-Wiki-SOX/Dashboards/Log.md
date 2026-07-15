# SOX Audit Context-Wiki — Operational Log

Chronological changelog of additions, removals,
and structural changes.

## 2026-07-15

* Initialized wiki directory structure
  (Inbox, Raw, Wiki/{Concepts,Entities,Summaries},
  Dashboards) per d3_howto_context_wiki.md.
* Downloaded 28 source documents into Raw/
  (5 categories: 01_sox_basics, 02_regulatory,
  03_big_four, 04_coso_fei, 05_it_controls).
  All files verified (valid PDFs / substantive
  HTML); one duplicate (PCAOB AS 2201) removed
  at ingest. Source URLs recorded in
  Raw/sources.md, including known gaps
  (paywalled COSO volumes, bot-blocked NetSuite
  whitepapers).
* Converted all 28 Raw/ documents into
  structured OKF summaries (Wiki/Summaries/),
  each with frontmatter (type, title,
  description, resource, source_file, tags).
* Built the knowledge graph: 68 concept pages
  (Wiki/Concepts/) and 18 entity pages
  (Wiki/Entities/) in OKF format, extracted
  and deduplicated from the summaries
  (merged: Mitigating→Compensating Controls,
  IPE→Information Produced by the Entity,
  Access Certification→User Access Review,
  Internal Audit Function→Internal Audit).
* Link integrity verified: 2,463 wiki links,
  0 broken (fixed 14 files with line-split
  links and alias links).
* Generated Dashboards/Index.md from page
  frontmatter (114 pages indexed).
