# Wiki Server (local browsing UI)

`wiki_server.py` serves a context wiki as a local,
human-readable website in the style of Wikipedia —
navigable wiki links, search, infoboxes, and
backlinks. Read-only: it never modifies wiki files.

## Running

Recommended — the control scripts (background run,
PID file `.wiki_server.pid`, log `wiki_server.log`):

```bash
./server_start.sh     # start on port 8020
./server_stop.sh      # stop (PID file, then any
                      #   process on the port)
./server_restart.sh   # stop + start
```

Or run in the foreground:

```bash
/Users/levselector/.venvs/standard/bin/python \
    wiki_server.py
# open http://localhost:8020
```

`server_start.sh` refuses to start if port 8020 is
already in use; `server_stop.sh` also cleans up any
stray process holding the port.

Serve a different wiki:

```bash
WIKI_ROOT=/path/to/wiki python wiki_server.py
```

Requires `flask`, `markdown`, `pyyaml` (all present
in the `standard` venv). Port: **8020** (constant
`PORT` in the script).

## Features

| Feature | Details |
|---------|---------|
| Main page | Renders `Dashboards/Index.md` |
| Wiki links | `[[Name]]` and `[[Name\|alias]]` become links; links to missing pages show in red |
| Sections | Sidebar navigation to Concepts, Entities, Summaries, Dashboards with page counts |
| Infobox | OKF frontmatter (type, description, resource, source_file, tags) rendered as a floating box; `resource` becomes a clickable source link |
| Backlinks | "What links here" at the bottom of every page |
| Search | Full-text, case-insensitive, ranked (title matches first, then hit count), with highlighted snippets |
| Live | Pages are re-read per request — edits to the wiki show up on refresh, no restart needed |

## URLs

| URL | Content |
|-----|---------|
| `/` | Main page (wiki index) |
| `/wiki/<Page Name>` | One page |
| `/section/<Section>` | Section listing |
| `/search?q=...` | Search results |

## See also

- [d4_wiki_tools.md](d4_wiki_tools.md) — programmatic
  find / grep access to the same wiki.
- [d3_howto_context_wiki.md](d3_howto_context_wiki.md)
  — the wiki structure being served.
