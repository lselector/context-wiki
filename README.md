# context-wiki

Notes on how to create and maintain your own knowledge base wiki (context wiki) based on markdown files in OKF format

## Documents

- [d1_okf.md](d1_okf.md) — Open Knowledge Format (OKF):
  definition, frontmatter fields, conventions,
  and short example files.
- [d2_docs2okf.md](d2_docs2okf.md) — tutorial on converting
  an existing document into OKF format.
- [d3_howto_context_wiki.md](d3_howto_context_wiki.md) —
  how to create and maintain your own context wiki: topics →
  raw downloads → Markdown → interlinked OKF files.

- [d4_wiki_tools.md](d4_wiki_tools.md) — Python
  find / grep / read utilities for the wiki, usable
  from Python, the command line, Claude Code, or as
  claude-agent-sdk tools.

- [d5_wiki_server.md](d5_wiki_server.md) — local
  Wikipedia-style browsing UI for the wiki
  (`wiki_server.py`, port 8020): navigation, search,
  infoboxes, backlinks.

## Code

- [wiki_tools.py](wiki_tools.py) — stdlib-only find /
  grep / read module (see d4_wiki_tools.md).
- [wiki_server.py](wiki_server.py) — local wiki web
  server on port 8020 (see d5_wiki_server.md).
- `server_start.sh` / `server_stop.sh` /
  `server_restart.sh` — control scripts for the wiki
  server.

## Wikis

- [Context-Wiki-SOX/](Context-Wiki-SOX/) — context wiki
  about SOX (Sarbanes-Oxley) Audit, structured per
  d3_howto_context_wiki.md.
